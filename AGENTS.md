# Agents - plug-factory

Public plugin marketplace (`Dahhrk/plugins`). Kitchen is `dark-factory` - do not invent product work there. Everything in this repo is public: no secrets, no private Feature Maps.

1. Start non-trivial work with `/poteto-mode`. Done means a checkable validation or test result.
2. Default: every prose surface is orwell-prose (docs, PRs, commits, chat reports, landing copy; rules 1-12). Agents apply before delivery; do not wait to be asked. `/orwell-prose` names the contract. `unslop` and no-em-dash stay secondary.
3. Default: every `ui:yes` / Figma ask starts from the existing design system plus one approved keyframe, expands the full flow in Figma, proves visual parity, gets a frontend look, then encodes. Fail closed without system, keyframe, or Figma access. `/figma-from-system` names the contract.
4. Default: every new product idea opens a temporary product/design/engineering debate room (plain product name), captures requirements and the decision in writing, then closes the room before encode. `/product-debate` names the contract.
5. Default: before any non-trivial ask, restate Goal / Constraints / Done means / Keep in plain words, then act (`outcome-repeat-back`). Cuts dump→wrong-build. `/outcome-repeat-back` names the contract.
6. Default: exit with a mergeable artifact (PR, brief, scorecard, verified claim). Never end with a "you should…" homework list (`results-not-homework`). `/results-not-homework` names the contract.
7. Default: when an ask spans multiple workstreams (frontend, backend, research, docs, CI, review, QA), run parent + specialists with clear ownership, an ordered plate with merge holds, and parent waits on children (`fleet-orchestrate`). Shared box filesystem OK; memory stays per-agent. Verify before merge. Plain workstream names only. `/fleet-orchestrate` names the contract. Opt-in poteto playbook: `playbooks/fleet-orchestrate.md`.
8. Default: after a pass, if the same manual flow recurred twice, offer skill-authoring / learn-from-demonstration once; drop if declined (`teach-to-skill`). `/teach-to-skill` names the contract.
9. Default: falsifiable "done" claims and substance merge claims need fresh `verify-this` evidence before ship. Recap is not evidence.
10. Gate: `node scripts/validate-plugins.mjs` (ajv schema check on marketplace.json + plugin.json files).
11. One verifiable unit per PR. Author does not merge on own verdict.
12. Respect `.cursor/dune.md` and `BUGBOT.md`.
13. Never commit secrets. Never Autopilot until doctor/launch/drive evidence works.
14. Storage: kitchen `docs/storage-layout.md` + this repo `PRIVATE.md`.
