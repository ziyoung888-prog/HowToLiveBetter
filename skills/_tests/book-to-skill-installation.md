# book-to-skill installation smoke test

## Source integrity
- Upstream: `virgiliojr94/book-to-skill`
- Pinned commit: `c108d25b0cb58e1bdc361f3de02ed9f37075152f`
- License: MIT

## Required files
The installation is considered structurally complete only when all of these exist:

- `skills/book-to-skill/SKILL.md`
- `skills/book-to-skill/scripts/extract.py`
- `skills/book-to-skill/book_to_skill/cli.py`
- `skills/book-to-skill/book_to_skill/utils.py`
- `skills/book-to-skill/book_to_skill/parsers/pdf.py`
- `skills/book-to-skill/book_to_skill/parsers/epub.py`
- `skills/book-to-skill/tools/scan_generated_skill.py`
- `skills/book-to-skill/pyproject.toml`
- `skills/book-to-skill/LICENSE.md`
- `skills/book-to-skill/SECURITY-NOTICE.md`
- `skills/book-to-skill/UPSTREAM.md`

## Expected behavior
1. Agent can discover `book-to-skill` from `skills/book-to-skill/SKILL.md`.
2. When given a supported book/document path, it validates the source before conversion.
3. It distinguishes technical vs text-heavy extraction.
4. It performs a cost/size preflight before expensive generation.
5. Generated skills are scanned before promotion.
6. Generated skills entering this repository must also pass local review and regression tests.

## Security regression
- Never sync from unofficial repositories with the same name.
- Do not auto-install optional Python/system dependencies without user approval.
- Do not auto-merge generated skills directly to `main`.
