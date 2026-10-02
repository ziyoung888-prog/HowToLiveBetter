# Source Manifest

- Source repository: `ziyoung888-prog/HowToLiveBetter`
- Source directory: `book/`
- Source chapter count at generation: 34
- Generation date: 2026-10-02
- Generator basis: `book-to-skill 1.4.0`, pinned upstream `c108d25b0cb58e1bdc361f3de02ed9f37075152f`
- Conversion mode: text-heavy / project-local
- Architecture: lightweight chapter routing with authoritative source retained in `book/`

## Authority rule

The files in `chapters/` are derived navigation aids. They are never authoritative for exact numeric claims, evidence grades, statutes, policy dates, study results, or exceptions. Always read the corresponding source chapter.

## Why this is intentionally different from a standalone book-to-skill export

The upstream converter normally packages chapter material because the generated Skill may live separately from the source book. Here the source book and generated Skill live in the same repository, so duplicating the source would reduce maintainability without improving retrieval.
