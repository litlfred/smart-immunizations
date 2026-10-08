# Library — the immunizations DAK and the L1 sources it cites

The library behind the WHO Digital adaptation kit for immunizations. It was built with
[folio-assistant](https://github.com/litlfred/folio-assistant)'s
`dak-l1-library` skill:

1. **The DAK is ingested, and stays library-only.** A DAK is L2, not L1, so it
   has no L1 knowledge graph.
2. **Component 1 §1.2** ("WHO guidelines, recommendations and guidance") is
   read for the sources the DAK draws on.
3. **Each L1 source is fetched, ingested on its own, and given its own L1
   graph**: `smart-kg-l1-library.jsonld` beside its entry.

The graphs are [WHO smart-kg](https://github.com/WorldHealthOrganization/smart-kg)
**L1 3.0** documents (main `3f5e477`) using the `l1-library` layer from
[litlfred/smart-base](https://github.com/litlfred/smart-base) `kg/`. All of them
pass smart-base's Zod validator.

## They are JSON-LD

Each graph names `http://smart.who.int/kg/l1-library.context.jsonld`, generated
in litlfred/smart-base `kg/` from the same source as the FHIR models. The URL
is the layer's identity and is never fetched: smart-base's `src/loader.ts`
serves the context offline.

```ts
import jsonld from "jsonld";
import { documentLoader } from "<smart-base>/kg/src/loader.ts";
const nquads = await jsonld.toRDF(graph, { format: "application/n-quads", documentLoader });
```

Every node keeps its class, every property its name (Dublin Core where L1
inherits it), and each specialisation is a `prov:specializationOf` statement.
Leave no one behind alone gives 1,508 triples.

## The rule between library and L1

The library is **upstream** of L1 (owner, 2026-10-07):
- An L1 publication, its sections and its printed elements are each
  `specializationOf` the library node they were read from: the entry, a
  section, a block.
- Nothing in the library points at L1.
- L1 inherits whatever sectioning the ingest produced.

## The L1 graphs

| ref | source | fetched from | sectioning | sections | elements |
|---|---|---|---|---|---|
| (31) | [Leave no one behind: guidance for planning and implementing catch-up vaccination](9789240016514-eng/) (2021), implementation guidance | WHO IRIS 10665/340749 | inferred contents | 21 | 1 figure, 7 boxes, 7 tables |
| (15) | [Electronic Immunization Registry: practical considerations…](9789275119532-eng/) (PAHO, 2018) | PAHO IRIS 10665.2/34865 | inferred contents | 18 | 14 figures, 21 tables |
| (26) | [Analysis and use of health facility data: guidance for immunization programme managers](facilityanalysisguide-immunization/) (2018), implementation guidance | who.int item page | PDF outline | 57 | 1 figure |
| (29) | [Table 1: Summary of WHO position papers – recommendations for routine immunization](immunization-summary-table-1/), summary table | who.int item page | PDF outline | 2 | 1 table |
| (29) | [Table 2: … recommended routine immunizations for children](immunization-summary-table-2/), summary table | who.int item page | PDF outline | 3 | 1 table |
| (29) | [Table 3: Recommendations for interrupted or delayed routine immunization](immunization-summary-table-3/), summary table | who.int item page | PDF outline | 1 | 1 table |
| (29) | [Table 4: … immunization of health care workers](immunization-summary-table-4/), summary table | who.int item page | PDF outline | 1 | 1 table |
| (32) | [Monitoring metrics related to the global COVID-19 vaccination strategy in a changing world: July 2022 update](monitoring-metrics-related-to-the-global-covid-19-vaccinatio/) | who.int item page | pages (its inferred contents failed the trust tests) | 7 | 2 tables |

Each source's `uploads/<doc_id>/intake.json` records **why it is L1**.
§1.2 calls everything it cites "WHO guidelines and guidance", so each source
carries a `context` classification naming its reference number. LNOB also
carries the owner's `declared` one.

## Not L1, held or not

| | why |
|---|---|
| [`9789240099456-eng/`](9789240099456-eng/), the DAK itself | L2. Library only. |
| [`who-2019-ncov-digital-certificates-vaccination-20211-eng/`](who-2019-ncov-digital-certificates-vaccination-20211-eng/), (28) DDCC | Owner ruling, 2026-10-07. §1.2's context says L1; the declaration wins, and the run reports the disagreement. |
| (24) WHO Immunization Data Portal | A website, not a publication. Not fetched. |
| (30) Sample WHO/UNICEF joint reporting form | A blank spreadsheet form. Not fetched; data.unicef.org also refuses this environment. |

## What needs a person

- **(29) is a newer edition than the one cited.** The DAK (2024) cites the
  tables "updated in 2024". who.int now serves the editions dated
  **1 December 2025**, and those are what was ingested. Each table's intake
  says so.
- **Licences are `unknown`** for the who.int and PAHO items:
  - a who.int item page states copyright, not a licence;
  - PAHO's record names no licence this recognises.

  The licence each PDF prints on its imprint page is not read automatically.
- **Element types the library does not extract yet:** table rows, footnotes,
  charts, images, flowcharts and lists. Each publication's note names them.
- **Table cells are not modelled.** Each summary table is one `table` element;
  its rows are the next step (`pdf-tables.py`).

`../uploads/<doc_id>/` holds each fetched item's `intake.json` and its Dublin
Core record. The PDFs are pinned there by sha256 and not committed.

## Regenerating

From a folio-assistant checkout beside this one:

```sh
# fetch (an IRIS handle, or a who.int item page)
bun run folio-assistant-core/scripts/fetch-dspace-item.ts <handle URL> --out ../smart-immunizations/uploads
bun run folio-assistant-core/scripts/fetch-who-publication.ts <who.int item URL> --out ../smart-immunizations/uploads
# Component 1: record section 1.2's L1 context on each held source; writes nothing beside the DAK
bun run smart-base/scripts/extract-dak-l1-references.ts \
  --entry ../smart-immunizations/library/9789240099456-eng --context-only --record-context
# each L1 source as L1 (a non-L1 entry is reported and skipped); --check to verify
bun run smart-base/scripts/l1-specialise.ts --entry ../smart-immunizations/library/<entry> --validate-zod <smart-base checkout>
```
