# Cursor Team Kit plugin

Internal-style workflows for CI, code review, shipping, and test reliability. The kit is designed to be plug and play without requiring third-party service integrations.

**Default:** every non-trivial ask is a one-shot task. Agents start on that route automatically (vague → `poteto-prompt` → `poteto-mode`; structured → `poteto-mode` with Done means + Keep; until-X on Cursor → autonomous-run + built-in `/loop`). Typing `/one-shot-task` is optional; the skill names the contract.

**Default (prose):** every docs, PR, commit, chat report, and landing line runs through `orwell-prose` (rules 1-12) before delivery. Agents apply automatically; do not wait to be asked. Typing `/orwell-prose` is optional; the skill names the contract. Same shape as one-shot-task. `unslop` and no-em-dash stay secondary.

**Default (UI / Figma):** every `ui:yes` / Figma ask starts from the existing design system plus one approved keyframe, expands the full flow in Figma, proves visual parity, gets a frontend look, then encodes. Fail closed without system, keyframe, or Figma access. Typing `/figma-from-system` is optional; the skill names the contract.

**Default (new product idea):** every new product idea opens a temporary product/design/engineering debate room (plain product name), captures requirements and the decision in writing, then closes the room before encode. Typing `/product-debate` is optional; the skill names the contract.


**Default (repeat-back):** before any non-trivial ask, restate Goal / Constraints / Done means / Keep in plain words, then act. Typing `/outcome-repeat-back` is optional; the skill names the contract.

**Default (exit):** leave a mergeable artifact (PR, brief, scorecard, verified claim). Never end with a "you should…" homework list. Typing `/results-not-homework` is optional; the skill names the contract.

**Default (multi-workstream):** when an ask spans multiple workstreams, run parent + specialists with clear ownership, an ordered plate with merge holds, and parent waits on children. Verify before merge. Typing `/fleet-orchestrate` is optional; the skill names the contract.

**Default (post-pass):** if the same manual flow recurred twice, offer skill-authoring / learn-from-demonstration once; drop if declined. Typing `/teach-to-skill` is optional; the skill names the contract.

**Default (leave clean):** kill orphaned local agent children before you stop; mid-session `/leave-machine-clean` reclaims session orphans only. Cap parallel local workstreams; prefer remote for heavy verify. Typing `/leave-machine-clean` is optional; the skill names the contract.

**Default (verify):** falsifiable "done" and substance merge claims need fresh `verify-this` evidence before ship.

## Installation

```bash
/add-plugin cursor-team-kit
```

## Components

### Skills

| Skill | Description |
|:------|:------------|
| `one-shot-task` | Default entry for every non-trivial ask (named contract; agents start here automatically) |
| `orwell-prose` | Default writing system for every prose surface (named contract; agents apply automatically, same shape as one-shot-task) |
| `figma-from-system` | Default for ui:yes / Figma work (design system + approved keyframe, fail closed; named contract) |
| `product-debate` | Default for every new product idea before encode (temporary debate room; named contract) |
| `outcome-repeat-back` | Default preamble: restate Goal / Constraints / Done means / Keep, then act (named contract) |
| `results-not-homework` | EXIT check: leave a mergeable artifact; never end with homework (named contract) |
| `fleet-orchestrate` | Default when an ask spans multiple workstreams (parent + specialists; named contract) |
| `teach-to-skill` | Post-pass: after the same manual flow twice, offer skill-authoring once (named contract) |
| `leave-machine-clean` | EXIT + on-demand reclaim: tear down local agent children; mid-session census kill (named contract) |
| `factory-init` | Onboard a repo into the dark factory (AGENTS, close-loop, gates, then seat kits) |
| `seat-kit` | Detect languages and seat matching language kits (repo gates + plugin) |
| `factory-status` | One-table health sweep across factory repos and runners |
| `merge-queue` | Merge every mergeable open PR across the factory repos (invocation is authorization) |
| `loop-on-ci` | Watch CI runs and iterate on failures until checks pass |
| `review-and-ship` | Run a structured review, commit changes, and open a PR |
| `pr-review-canvas` | Generate an interactive HTML PR walkthrough with annotated, categorized diffs |
| `verify-this` | Prove or disprove claims with baseline/treatment artifacts and a clear verdict |
| `control-cli` | Build or adapt a local harness to drive and profile interactive CLIs or TUIs |
| `control-ui` | Build or adapt a local browser/CDP harness for web or Electron UIs |
| `make-pr-easy-to-review` | Clean noisy PR history, improve descriptions, and add reviewer guidance |
| `run-smoke-tests` | Run Playwright smoke tests and triage failures |
| `fix-ci` | Find failing CI jobs, inspect logs, and apply focused fixes |
| `new-branch-and-pr` | Create a fresh branch, complete work, and open a pull request |
| `get-pr-comments` | Fetch and summarize review comments from the active pull request |
| `check-compiler-errors` | Run compile and type-check commands and report failures |
| `what-did-i-get-done` | Summarize authored commits over a given time period into a concise status update |
| `weekly-review` | Generate a weekly recap of shipped work with bug fix/tech-debt/net-new highlights |
| `fix-merge-conflicts` | Resolve merge conflicts, validate build/tests, and summarize decisions |
| `deslop` | Remove AI-generated code slop and clean up code style |
| `workflow-from-chats` | Extract durable working preferences from chats into skills, rules, or docs |
| `thermo-nuclear-code-quality-review` | Run an unusually strict maintainability review (code-judo, 1k-line rule, spaghetti, boundaries) |

### Agents

| Agent | Description |
|:------|:------------|
| `ci-watcher` | Monitor GitHub Actions runs and return concise pass/fail summaries |
| `thermo-nuclear-code-quality-review` | Task subagent that runs the thermo-nuclear code quality rubric against a diff |

### Rules

| Rule | Description |
|:-----|:------------|
| `typescript-exhaustive-switch` | Require exhaustive switch handling for unions/enums |
| `no-inline-imports` | Keep imports at module top-level for readability and consistency |

## License

MIT
