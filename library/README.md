# Library — the immunizations DAK's L1 sources

The WHO guidance this DAK operationalises, ingested, and the L1 knowledge graph
that records how the DAK cites it. Built with
[folio-assistant](https://github.com/litlfred/folio-assistant)'s
`dak-l1-library` skill: **every library built for a DAK starts from the DAK's
own Component 1** ("Health interventions and recommendations"), because that is
where a DAK names the guidelines it rests on.

## The graph

[`9789240099456-eng/smart-kg-l1-dak-references.json`](9789240099456-eng/smart-kg-l1-dak-references.json)
— a [WHO smart-kg](https://github.com/WorldHealthOrganization/smart-kg) L1
graph document (ontology `1.0`, main `66a9b13`), read from Component 1 of the
[Digital adaptation kit for immunizations](https://iris.who.int/handle/10665/380303)
(ISBN 978-92-4-009945-6, PDF pp. 26–27).

| node | count | from |
|---|---|---|
| `citation` | 12 | each printed `(n)` in §1.2, verbatim; plus §1.1's unnumbered mention |
| `publication` | 8 | the reference each number points at |
| `health-intervention` | 30 | §1.1: 7 vaccine administration practices, 23 vaccinations |
| `external-artifact` | 2 | the DAK pages doing the citing (§1.1, §1.2) |

| edge | count |
|---|---|
| `citation appearsIn external-artifact` | 12 |
| `citation resolvesTo publication` | 11 |
| `health-intervention implementedBy external-artifact` | 30 |

It passes both **smart-kg `tools/validate.mjs`** (WHO main) and the **Zod
validator in smart-base `kg/`**, which also checks property values.

### What needs a person

- **Fidelity (T3) is not checked.** Five citations resolve by their printed
  number while their wording differs from the reference title: the four cards
  citing (29), which describe the summary tables rather than name them, and
  (24), which calls the immunization dashboard the "Immunization Data Portal".
  Each edge's note says so.
- **§1.1's "WHO universal health coverage list of essential interventions"** is
  unnumbered and left `unresolved`; its best title match, reference 22 (UHC
  compendium), is named in the note, not asserted.

## The entries

| entry | what | cited as | source |
|---|---|---|---|
| [`9789240099456-eng/`](9789240099456-eng/) | Digital adaptation kit for immunizations (2024) | — (the DAK) | [IRIS 10665/380303](https://iris.who.int/handle/10665/380303) |
| [`9789240016514-eng/`](9789240016514-eng/) | Leave no one behind: guidance for planning and implementing catch-up vaccination (2021) | (31) | [IRIS 10665/340749](https://iris.who.int/handle/10665/340749) |
| [`who-2019-ncov-digital-certificates-vaccination-20211-eng/`](who-2019-ncov-digital-certificates-vaccination-20211-eng/) | Digital documentation of COVID-19 certificates: vaccination status (2021) | (28) | [IRIS 10665/343361](https://iris.who.int/handle/10665/343361) |

All three are CC BY-NC-SA 3.0 IGO (each entry's `licence.json` says where that
is stated). Each was ingested by page; the extracted images are not yet
described, so the entries are **staged, not promoted**.

**Cited but not held**, each recorded in the graph with its URL: (15) PAHO
*Electronic immunization registry* (PAHO IRIS refused the fetch), (26) and (32)
on who.int, (29) the routine-immunization summary tables and (24) the
immunization dashboard (web pages), and (30) the WHO/UNICEF joint report form
(a spreadsheet).

`../uploads/<doc_id>/` holds each fetched item's `intake.json` and its IRIS
Dublin Core record. The PDFs are pinned there by sha256 and not committed.

## Regenerating

From a folio-assistant checkout beside this one:

```sh
bun run smart-base/scripts/extract-dak-l1-references.ts \
  --entry ../smart-immunizations/library/9789240099456-eng \
  --validate <smart-kg checkout> --validate-zod <smart-base checkout>
bun run smart-base/scripts/extract-dak-l1-references.ts \
  --entry ../smart-immunizations/library/9789240099456-eng --check
```
