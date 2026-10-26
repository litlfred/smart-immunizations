# AGENTS.md — smart-immunizations

This file is agent-generic: Claude Code, Gemini CLI, Cursor, Copilot and others
read it natively. What binds everywhere is the harness's
[`AGENTS.md`](https://github.com/litlfred/cat-harness/blob/HEAD/AGENTS.md); what
this repository *is* is [`README.md`](README.md).

## What this instance is

The WHO SMART Guidelines immunizations implementation guide: FHIR IG source
under `input/`, built by the IG Publisher. It takes the smart-hiv shape (owner,
2026-10-14). It has no harness of its own: `index.config.json` mounts
`smart-base` and the layers below it, and `smart-immunizations.json` declares
what an index may mount from here.

## The one rule

**The declaration names only what an index mounting this instance has.** A
directory declared here but not mounted is the `dh4f` defect: a consumer scans
nothing and reports a clean run over it. So when you add a directory to an
index's override, declare it here in the same change, and when you remove one,
drop it from both.

## What an index mounts from here

**folio-assistant mounts three directories** of this repository: `library/`
(the L1 library), `examples/l1-recommendation-scenarios/` (the measles
worked example, smart-base's `l1-extraction` kind) and `document-kinds/` (this
IG's DAK coverage report, moved here from smart-base by wrong-direction move
M13). Its override lists exactly those three ids, and
`smart-immunizations.json` declares exactly those three (owner ruling B1,
2026-10-15; "Mount it everywhere", the same day; M13 added the third, and the
index re-pin that mounts it adds `smart-immunizations-document-kinds` to the
override). The measles
example sits outside `library/` so it is not read as a library entry.
`input/` and the rest stay in this repository.

**The web annexes (bean folio-assistant-fm9n, 2026-10-24) add two more**:
`annexes/` (`smart-immunizations-annexes`, fhir-harness's `ig-annex` page
hook: `annexes.json` places each annex on its page) and `web-annexes/`
(`smart-immunizations-web-annexes`, smart-base's `web-annex` kind: the data
dictionary, Web Annex A of the DAK). `annexes/` also holds the two swimlane
annexes (litlfred/aai-programme#28): `personas-swimlanes.md` on
`personas.md` and `processes-swimlanes.md` on `business-processes.md`, written
by smart-base's `dak-swimlanes.ts` from the personas page, the process figures
and `input/business-processes/swimlanes.json`; regenerate them, never edit
them. They are declared here with the
folio-assistant override change that mounts them, and need fhir-harness and
smart-base pins that know both kinds: a declaration naming a kind the pinned
layers do not register is refused when it is read.
