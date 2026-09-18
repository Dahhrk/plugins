# Agents - plug-factory

Public plugin marketplace (`Dahhrk/plugins`). Kitchen is `dark-factory` - do not invent product work there. Everything in this repo is public: no secrets, no private Feature Maps.

1. Start non-trivial work with `/poteto-mode`. Done means a checkable validation or test result.
2. Gate: `node scripts/validate-plugins.mjs` (ajv schema check on marketplace.json + plugin.json files).
3. One verifiable unit per PR. Author does not merge on own verdict.
4. Respect `.cursor/dune.md` and `BUGBOT.md`.
5. Never commit secrets. Never Autopilot until doctor/launch/drive evidence works.
6. Storage: kitchen `docs/storage-layout.md` + this repo `PRIVATE.md`.
