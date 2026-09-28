# Agents - plug-factory

Public plugin marketplace (`Dahhrk/plugins`). Kitchen is `dark-factory` - do not invent product work there. Everything in this repo is public: no secrets, no private Feature Maps.

1. Start non-trivial work with `/poteto-mode`. Done means a checkable validation or test result.
2. Default: every prose surface is orwell-prose (docs, PRs, commits, chat reports, landing copy; rules 1-12). Agents apply before delivery; do not wait to be asked. `/orwell-prose` names the contract. `unslop` and no-em-dash stay secondary.
3. Default: every `ui:yes` / Figma ask starts from the existing design system plus one approved keyframe, expands the full flow in Figma, proves visual parity, gets a frontend look, then encodes. Fail closed without system, keyframe, or Figma access. `/figma-from-system` names the contract.
4. Default: every new product idea opens a temporary product/design/engineering debate room (plain product name), captures requirements and the decision in writing, then closes the room before encode. `/product-debate` names the contract.
5. Gate: `node scripts/validate-plugins.mjs` (ajv schema check on marketplace.json + plugin.json files).
6. One verifiable unit per PR. Author does not merge on own verdict.
7. Respect `.cursor/dune.md` and `BUGBOT.md`.
8. Never commit secrets. Never Autopilot until doctor/launch/drive evidence works.
9. Storage: kitchen `docs/storage-layout.md` + this repo `PRIVATE.md`.
