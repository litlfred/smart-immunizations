# Library — the immunizations DAK's L1 sources

The WHO guidance this DAK operationalises, ingested, and the L1 knowledge graph
that records how the DAK cites it. Built with
[folio-assistant](https://github.com/litlfred/folio-assistant)'s
`dak-l1-library` skill: **every library built for a DAK starts from the DAK's
own Component 1** ("Health interventions and recommendations"), because that is
where a DAK names the guidelines it rests on.

## Two L1 graphs, and the rule between them

The library is **upstream** of L1 (owner, 2026-10-07: *"L1 can point upstream
but not downstream"*). An L1 node may name the library node it was read from;
nothing in the library names L1. Both graphs are
[WHO smart-kg](https://github.com/WorldHealthOrganization/smart-kg) **L1 3.0**
documents (main `3f5e477`) using the `l1-library` layer from
[litlfred/smart-base](https://github.com/litlfred/smart-base) `kg/`, and both
pass smart-base's Zod validator, which checks property values too.

### Leave no one behind, as L1 — the source itself

[`9789240016514-eng/smart-kg-l1-library.json`](9789240016514-eng/smart-kg-l1-library.json):
the guidance's publication, 21 sections and 15 printed elements (1 figure,
7 boxes, 7 tables), each `specializationOf` the library node it was read from
(the entry, a section, a block). The sections are the library's own — the
ingest's inferred contents, mean confidence 0.92 — and each node's note carries
its confidence. Section IRIs use the number as the contents page prints it
(`Section 1`, `Annex 3`).

| node | count | edge | count |
|---|---|---|---|
| `publication` | 1 | `specializationOf library-node` | 37 |
| `publication-section` | 21 | `contains` | 36 |
| `publication-element` | 15 | | |
| `library-node` | 31 | | |

Six element types L1 3.0 defines are not extracted by the library yet (table
rows, footnotes, charts, images, flowcharts, lists); the publication's note
names them.

### The DAK's citations — Component 1 §1.2

[`9789240099456-eng/smart-kg-l1-dak-references.json`](9789240099456-eng/smart-kg-l1-dak-references.json),
read from the [Digital adaptation kit for immunizations](https://iris.who.int/handle/10665/380303)
(ISBN 978-92-4-009945-6). The DAK is not L1 (it is L2), so it has no
publication node: only what it prints and what that resolves to.

| node | count | edge | count |
|---|---|---|---|
| `citation` | 12 | `citation numberedAs reference-entry` | 11 |
| `reference-entry` | 8 | `reference-entry resolvesTo publication` | 7 |
| `publication` | 7 | `reference-entry resolvesTo library-node` | 1 |
| `library-node` | 1 | | |

(31) resolves to the **same** publication node as the graph above
(`…/publication/isbn-9789240016514`). (28), DDCC, resolves to its **library
entry**: it is held but not L1.

### L1 or not — recorded on each intake

| entry | declared | context (§1.2) | inferred (IRIS record) | result |
|---|---|---|---|---|
| Leave no one behind | L1, implementation-guidance | L1 | L1, implementation-guidance | **L1** |
| DAK for immunizations | not L1 | — | not L1 (Smart guidelines series) | not L1 |
| DDCC 2021 | not L1 | L1 | not L1 (technical specification) | not L1; context's disagreement reported every run |

### What needs a person

- **Fidelity is not checked.** Five citations resolve by their printed number
  while their wording differs from the reference title: the four cards citing
  (29), and (24). Each `numberedAs` note says so.
- **Context makes every §1.2 source L1**, including two that are hardly
  guidance: (24) the immunization dashboard and (30) the WHO/UNICEF joint
  report form, a spreadsheet. Neither is held, so neither has an intake a
  person could declare on; they are recorded as context left them.
- **§1.1's "WHO universal health coverage list of essential interventions"** is
  unnumbered and left `unresolved`; its best title match is named in the note.
- **§1.1's interventions are not emitted.** An L1 3.0 `health-intervention` is
  a catalogue entry keyed by its code, which the DAK's list does not print.

## The entries

| entry | what | cited as | source |
|---|---|---|---|
| [`9789240099456-eng/`](9789240099456-eng/) | Digital adaptation kit for immunizations (2024) | — (the DAK) | [IRIS 10665/380303](https://iris.who.int/handle/10665/380303) |
| [`9789240016514-eng/`](9789240016514-eng/) | Leave no one behind: guidance for planning and implementing catch-up vaccination (2021) | (31) | [IRIS 10665/340749](https://iris.who.int/handle/10665/340749) |
| [`who-2019-ncov-digital-certificates-vaccination-20211-eng/`](who-2019-ncov-digital-certificates-vaccination-20211-eng/) | Digital documentation of COVID-19 certificates: vaccination status (2021) | (28) | [IRIS 10665/343361](https://iris.who.int/handle/10665/343361) |

All three are CC BY-NC-SA 3.0 IGO (each entry's `licence.json` says where that
is stated). None has a PDF outline; each was ingested from its **inferred
contents**, which passed the ingest's trust tests (issue #2302): LNOB 22
sections, the DAK 8, DDCC 41. The extracted images are not yet described, so
the entries are **staged, not promoted**.

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
# the DAK's citations; --record-context writes §1.2's context record onto held sources' intakes
bun run smart-base/scripts/extract-dak-l1-references.ts \
  --entry ../smart-immunizations/library/9789240099456-eng --record-context --validate-zod <smart-base checkout>
# each L1 source as L1 (a non-L1 entry is reported and skipped)
bun run smart-base/scripts/l1-specialise.ts \
  --entry ../smart-immunizations/library/9789240016514-eng --validate-zod <smart-base checkout>
# both have --check
```
