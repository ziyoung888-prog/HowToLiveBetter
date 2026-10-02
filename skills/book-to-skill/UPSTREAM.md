# Upstream metadata

- Project: `virgiliojr94/book-to-skill`
- Official repository: https://github.com/virgiliojr94/book-to-skill
- License: MIT
- Imported version: 1.4.0
- Pinned upstream commit: `c108d25b0cb58e1bdc361f3de02ed9f37075152f`
- Import date: 2026-10-02

## Why pinned

This copy is intentionally pinned to a specific upstream commit so the local Skill library is reproducible and auditable. Do not silently replace it with the current upstream `master`.

## Security note

The upstream maintainer published a warning about malicious unofficial re-uploads using the same project name. Only sync from `virgiliojr94/book-to-skill`.

## Local integration policy

- Keep upstream files under `skills/book-to-skill/` unchanged where possible.
- Put local behavior overrides in repository-level `AGENTS.md` or shared protocols.
- Generated skills must also comply with this repository's `GLOBAL_AGENT_PROTOCOL.md` and `GROWTH_PROTOCOL.md`.
- Before promoting a generated skill to `main`, inspect it, run the upstream generated-skill scanner where available, add regression tests, and use a PR.
- When updating, compare upstream changes from the pinned commit to the new target commit before replacing files.
