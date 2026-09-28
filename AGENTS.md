# Agents - plug-factory

Public plugin marketplace (`Dahhrk/plugins`). Kitchen is `dark-factory` - do not invent product work there. Everything in this repo is public: no secrets, no private Feature Maps.

1. Start non-trivial work with `/poteto-mode`. Done means a checkable validation or test result.
2. Prose: every docs, PR, commit, chat report, and landing line runs through `orwell-prose` (rules 1-12) before delivery. Positive writing rules, not a ban list. `unslop` and no-em-dash stay secondary.
3. Gate: `node scripts/validate-plugins.mjs` (ajv schema check on marketplace.json + plugin.json files).
4. One verifiable unit per PR. Author does not merge on own verdict.
5. Respect `.cursor/dune.md` and `BUGBOT.md`.
6. Never commit secrets. Never Autopilot until doctor/launch/drive evidence works.
7. Storage: kitchen `docs/storage-layout.md` + this repo `PRIVATE.md`.
