# Local runtime notes

This directory contains the upstream `book-to-skill` Agent Skill and its runtime extraction engine.

## What is installed in this repository

- `SKILL.md`
- `scripts/extract.py`
- Python package under `book_to_skill/`
- `tools/scan_generated_skill.py`
- `pyproject.toml`
- upstream Chinese README, license and security notice

## Runtime dependencies

The repository copy makes the Skill available to project-local agents that scan `skills/`. Actual document conversion still depends on the local machine.

Basic text/Markdown paths have minimal requirements. Better support for PDF, EPUB, DOCX, HTML, RTF and technical PDFs may require the optional dependencies declared in `pyproject.toml`, plus system tools such as Poppler or Calibre for some formats.

Use the upstream preflight:

```bash
python skills/book-to-skill/scripts/extract.py --check
```

Do not automatically install missing packages without user approval.

## Output policy for this repository

When using book-to-skill inside this repository, generated Skills should be written under `skills/<slug>/` only when they are intended to become part of this Skill library. Otherwise keep generated output outside the repository until reviewed.
