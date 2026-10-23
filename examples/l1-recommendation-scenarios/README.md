# The measles scenarios — `examples/l1-recommendation-scenarios/measles/`

The worked example of smart-base's `recommendation-extraction` skill (Part 2,
"An authored L1, scenario half only"): the 75 recommendations of the WHO
measles position paper (WER 92(17), 2017) mapped against this guide's own
personas and processes. One user scenario per recommendation, every link a
candidate.

| file | what it is |
|---|---|
| `measles-position-paper-2017.l1.yaml` | the 75 recommendations, authored |
| `immz-vocabulary.json` | this guide's personas and processes, read from `input/pagecontent/` at `86898e6` |
| `measles-immz-mapping.yaml` | per recommendation: persona, process, act, outcome, domain, each with its source and basis |
| `candidates/` | the output: `scenario-candidates.l2.json` (an L2 graph document) and `scenario-warnings.md` (37 warnings) |

It moved here from smart-base on 2026-10-14. The owner ruled (Q2 of the
folio-assistant#2529 reference-direction review: "Move it") that a guide's
example lives in that guide's repository, because smart-base sits below the
guides and may not name them. The generic rung (`DAK.Persona.*`) is
smart-base's own, so the run reads it from the smart-base mount. Run it from
this repository's root, with the layers in `index.config.json` mounted:

```sh
bun run l1-scenarios:measles:check   # fails when the candidates are not current with their inputs
bun run l1-scenarios:measles         # regenerate
```

It sat under `library/` until 2026-10-15, when folio-assistant began mounting
`library/` (owner: "Mount it everywhere"). It moved here so the library's
readers do not take it for a library entry.
