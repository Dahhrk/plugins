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
9. Default: EXIT + on-demand reclaim. Kill orphaned local agent children (node/chromium/playwright/watchers/Electron helpers) before you stop; cap parallel local agents; prefer remote for heavy verify (`leave-machine-clean`). Agents apply on close when the session started local processes; `/leave-machine-clean` runs a mid-session reclaim.
10. Default: when an ask is recurring, scheduled, "let me know when", or about to be re-asked, create or update a routine/automation (`routine-by-default`). Agents start here automatically; `/routine-by-default` names the contract.
11. Default: capability / agent / bot / AI product work ships harnesses, evals, and delivery paths, not frontier training (`harness-not-training`). Train only when Dark explicitly asks. Agents start here automatically; `/harness-not-training` names the contract.
12. Default: falsifiable "done" claims and substance merge claims need fresh `verify-this` evidence before ship. Recap is not evidence.
13. Default: non-trivial multi-file feature work passes `software-factory-gates` (Product, Architecture, Program Design, Build Order) with explicit user approval at each gate before implementation. Trivial one-liners skip. Agents start here automatically; `/software-factory-gates` names the contract.
14. Default: UI and animation work applies `design-eng` taste and runs `review-animations` before ship. Vague motion feedback applies `animation-vocabulary` first. Agents start here automatically; the skill names the contract.
15. Default: new agent loop, overnight automation, or feedback-driven system applies `design-control-loop` (sensor/controller/actuator/disturbances) before implementation. Agents start here automatically; `/design-control-loop` names the contract.
16. Default: AGENTS.md drift or rewrite applies `improve-agents-md` for structured instruction blocks. Agents start here automatically; `/improve-agents-md` names the contract.
17. Default: non-trivial behavior changes in existing modules follow refactor-first (behavior-preserving cleanup with tests green, then the change on the clean structure). Never both in one unverifiable diff. Agents start here automatically; `/refactor-first` names the contract.
- Default: designing or reviewing public APIs, libraries, component props, CLI flags, or SDK surfaces applies `progressive-disclosure` (zero-config default, complexity opt-in, call-site-first, four layers). Agents start here automatically; `/progressive-disclosure` names the contract.
- Default: when a correction or convention must survive the next agent, encode it in the repo (CODEOWNERS, AGENTS.md, skills, BUGBOT.md, lint/CI) rather than chat memory (`encode-in-codebase`). Agents start here automatically; `/encode-in-codebase` names the contract.
- Default: public seams apply `pit-of-success` (obvious call correct; misuse hard; footgun test on the seam). Agents start here automatically; `/pit-of-success` names the contract.
- Default: reshaping existing code toward a known target applies `zero-tech-debt` (delete dead compatibility; rework from the intended end state). Overlap with `refactor-first`: that skill owns work order; this skill owns end-state reshape. Agents start here automatically; `/zero-tech-debt` names the contract.
- Default: user-facing feature work applies `ux-flow-plan` (current vs desired UX flow trees, then file/function anchors). Overlap with `figma-from-system` / `design-eng`: those own Figma/system and taste; this owns flow trees before code. Agents start here automatically; `/ux-flow-plan` names the contract.
17. Gate: `node scripts/validate-plugins.mjs` (ajv schema check on marketplace.json + plugin.json files).
18. One verifiable unit per PR. Author does not merge on own verdict.
12. Respect `.cursor/dune.md` and `BUGBOT.md`.
13. Never commit secrets. Never Autopilot until doctor/launch/drive evidence works.
14. Storage: kitchen `docs/storage-layout.md` + this repo `PRIVATE.md`.
