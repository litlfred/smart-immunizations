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

**folio-assistant mounts no directories** of this repository (owner ruling B1,
2026-10-15). Its override lists `directories: []`, and `smart-immunizations.json`
declares none. Only the declaration, this file and the README reach the index,
the last two as declared assets. `library/`, `input/` and the rest stay in this
repository. An index that wants `library/` declares it again, and gives the
measles example (`library/l1-recommendation-scenarios/`) a home that is not
read as a library entry.
