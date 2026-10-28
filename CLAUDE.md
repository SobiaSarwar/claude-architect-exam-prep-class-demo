# Claude Instructions

This repository holds study notes for the Claude Architect exam. It is public.

## Rule 1: Markdown only

Every file in this repo must be a Markdown file (`.md`).

- Create notes, outlines, flashcards, practice questions and summaries as `.md` files only.
- Do not add images, PDFs, spreadsheets, code files, JSON, text files or any other format. If the user asks for one, explain the rule and offer a Markdown alternative (for example, a table instead of a spreadsheet, a Mermaid code block instead of an image).
- Allowed non-Markdown exceptions, kept minimal:
  - `.gitignore`
  - `.github/workflows/*.yml` (the CI check that enforces this rule)
- A GitHub Actions check (`check-files`) fails any PR that contains other file types. Do not edit the check or its allowlist to get around it.

## Rule 2: Everything goes through a pull request

- Never commit or push directly to `main`.
- Work on a short-lived branch, push it and open a PR into `main`.
- Wait for `check-files` to pass before asking for a merge.
- Do not merge a PR unless the user explicitly tells you to. Merging is their review step.

## Conventions

- File names: lowercase, hyphenated, e.g. `prompt-caching.md`.
- One topic per file. Link related notes with relative links.
- Start each note with a single `#` title.
- Keep `README.md` as the index: add a link to each new note.
- End commit messages with the `Co-Authored-By` line supplied by the Claude Code session.
