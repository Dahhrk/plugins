# plug-factory

Cursor pack twin. Shared conventions and overlapping packs live here for the Cursor lane.

- Twin: `Dahhrk/devin-factory-plugins` (Devin editions under `plugins/`)
- Kitchen: `Dahhrk/dark-factory` (recipes and keep-up docs)
- Do not put product secrets here
- Autopilot stays gated
- Default: every non-trivial ask is a one-shot task (vague → poteto-prompt → poteto-mode; structured → poteto-mode with Done means + Keep; until-X on Cursor → autonomous-run + `/loop`). Agents start here automatically; `/one-shot-task` names the contract.
- Default: every prose surface is orwell-prose (docs, PRs, commits, chat reports, landing copy; rules 1-12). Agents apply before delivery; do not wait to be asked. `/orwell-prose` names the contract. `unslop` and no-em-dash stay secondary. Project `AGENTS.md` / `CLAUDE.md` may override voice.
- Default: every `ui:yes` / Figma ask starts from the existing design system plus one approved keyframe, expands the full flow in Figma, proves visual parity, gets a frontend look, then encodes. Fail closed without system, keyframe, or Figma access. Agents start here automatically; `/figma-from-system` names the contract.
- Default: every new product idea opens a temporary product/design/engineering debate room (plain product name), captures requirements and the decision in writing, then closes the room before encode. Agents start here automatically; `/product-debate` names the contract.
- Default: before any non-trivial ask, restate Goal / Constraints / Done means / Keep in plain words, then act (`outcome-repeat-back`). Cuts dump→wrong-build. Agents start here automatically; `/outcome-repeat-back` names the contract.
- Default: exit with a mergeable artifact (PR, brief, scorecard, verified claim). Never end with a "you should…" homework list (`results-not-homework`). Agents apply on close; `/results-not-homework` names the contract.
- Default: when an ask spans multiple workstreams (frontend, backend, research, docs, CI, review, QA), or when driving other agents on a desk (prompt / wait / loop / hand-off / review; never answer for the human), run parent + specialists with clear ownership, an ordered plate with merge holds, and parent waits on children (`fleet-orchestrate`). Shared box filesystem OK; memory stays per-agent. Verify before merge. Plain workstream names only. Agents start here automatically; `/fleet-orchestrate` names the contract. Opt-in poteto playbook: `playbooks/fleet-orchestrate.md`.
- Default: after a pass, if the same manual flow recurred twice, offer skill-authoring / learn-from-demonstration once; drop if declined (`teach-to-skill`). Agents apply as a post-pass; `/teach-to-skill` names the contract.
- Default: EXIT + on-demand reclaim. Kill orphaned local agent children (node/chromium/playwright/watchers/Electron helpers) before you stop; cap parallel local agents; prefer remote for heavy verify (`leave-machine-clean`). Agents apply on close when the session started local processes; `/leave-machine-clean` runs a mid-session reclaim.
- Default: when an ask is recurring, scheduled, "let me know when", or about to be re-asked, create or update a routine/automation (`routine-by-default`). Agents start here automatically; `/routine-by-default` names the contract.
- Default: capability / agent / bot / AI product work ships harnesses, evals, and delivery paths, not frontier training (`harness-not-training`). Train only when Dark explicitly asks. Agents start here automatically; `/harness-not-training` names the contract.
- Default: falsifiable "done" claims and substance merge claims need fresh `verify-this` evidence before ship. Recap is not evidence.
- Default: non-trivial multi-file feature work passes `software-factory-gates` (Product, Architecture, Program Design, Build Order) with explicit user approval at each gate before implementation. Trivial one-liners skip. Agents start here automatically; `/software-factory-gates` names the contract.
- Default: UI and animation work applies `design-eng` taste and runs `review-animations` before ship. Vague motion feedback applies `animation-vocabulary` first. Agents start here automatically; the skill names the contract.
- Default: new agent loop, overnight automation, or feedback-driven system applies `design-control-loop` (sensor/controller/actuator/disturbances) before implementation. Agents start here automatically; `/design-control-loop` names the contract.
- Default: AGENTS.md drift or rewrite applies `improve-agents-md` for structured instruction blocks. Agents start here automatically; `/improve-agents-md` names the contract.
- Default: non-trivial behavior changes in existing modules follow refactor-first (behavior-preserving cleanup with tests green, then the change on the clean structure). Never both in one unverifiable diff. Agents start here automatically; `/refactor-first` names the contract.
- Default: designing or reviewing public APIs, libraries, component props, CLI flags, or SDK surfaces applies `progressive-disclosure` (zero-config default, complexity opt-in, call-site-first, four layers). Agents start here automatically; `/progressive-disclosure` names the contract.
- Default: when a correction or convention must survive the next agent, encode it in the repo (CODEOWNERS, AGENTS.md, skills, BUGBOT.md, lint/CI) rather than chat memory (`encode-in-codebase`). Agents start here automatically; `/encode-in-codebase` names the contract.

- Default: public seams apply `pit-of-success` (obvious call correct; misuse hard; footgun test on the seam). Agents start here automatically; `/pit-of-success` names the contract.
- Default: reshaping existing code toward a known target applies `zero-tech-debt` (delete dead compatibility; rework from the intended end state). Overlap with `refactor-first`: that skill owns work order; this skill owns end-state reshape. Agents start here automatically; `/zero-tech-debt` names the contract.
- Default: user-facing feature work applies `ux-flow-plan` (current vs desired UX flow trees, then file/function anchors). Overlap with `figma-from-system` / `design-eng`: those own Figma/system and taste; this owns flow trees before code. Agents start here automatically; `/ux-flow-plan` names the contract.
- Default: box / worktree / session / port / desk-config asks apply `desk-boxes`. Agents start here automatically; `/desk-boxes` names the contract.
- Default: UI or page preview asks apply `local-preview` when a desk is present (reserved port + desk UI); otherwise fall back to `control-ui`. Agents start here automatically; `/local-preview` names the contract.
- Default: event-hook or before-gate automation applies `event-hooks` (distinct from `software-factory-gates`). Agents start here automatically; `/event-hooks` names the contract.
- Default: multi-workstream and desk agent drive (prompt / wait / loop / hand-off / review; never answer for the human) stay on `fleet-orchestrate`. Do not add a second orchestrate skill.
- Available: `agent-cli-lanes` documents install and hooks for Cursor, Claude Code, Codex, Gemini CLI, OpenCode, and Devin. Invoke when seating lanes; not Day-1 auto.
- After kit mirror/export to Devin, every kit needs `plugins/<kit>/.devin-plugin/plugin.json` (`node scripts/export-devin-plugin-manifests.mjs --assert` in the Devin twin). Cursor-only on Devin is a defect.
- Tracked kit `*.sh` must be git mode `100755`. After adding shell templates: `git update-index --chmod=+x -- <paths>`.
