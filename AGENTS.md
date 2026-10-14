# Repository Guidelines

## Project Structure

This repository collects concise reading notes about interesting research papers. Keep one Markdown file per paper under `notes/`, with source PDFs or other reference material under `papers/` when needed. Keep notes self-contained and link to the paper's canonical source (such as its arXiv page). Avoid duplicating a paper's full text.

## Note Naming and Structure

Name each note with the paper's arXiv identifier and a readable title, for example `notes/2101.03961-Switch-Transformer.md`. Use consistent, portable filenames: ASCII letters, digits, and hyphens; preserve the arXiv version when it matters to the note.

Use a clear title and organize the note for quick reading. A useful default structure is:

1. Paper metadata and source link
2. Problem and motivation
3. Main idea and method
4. Key results and evidence
5. Limitations, questions, and personal takeaways

Adapt the sections to the paper rather than filling them with generic summaries. Distinguish the authors' claims from your own interpretation, and cite page, section, figure, or table numbers for specific details where practical.

## Writing Style

Write notes in Markdown with descriptive headings, short paragraphs, and lists or tables when they make comparisons clearer. Explain technical terms on first use and preserve equations or notation only when they help explain the contribution. Write original summaries in your own words; quote sparingly and identify quoted material.

## Development and Validation

There is no build system or automated test suite. Inspect the repository with `rg --files` and review Markdown changes with `git diff --check` and `git diff`. Before adding a note, verify its paper identity and source link, ensure there is not already a note for that paper, and check that relative links resolve. No separate test command is required.

## Commits and Pull Requests

The Git history does not establish a commit convention. Use concise imperative subjects, such as `Add Switch Transformer reading note`. A pull request should identify the paper, link its source, summarize the note's focus, and mention any structural changes. Screenshots are unnecessary for text-only notes.

## Sources and Configuration

Prefer canonical publisher or preprint sources and record enough metadata to identify the paper and version. Do not commit credentials, temporary downloads, or unrelated personal data. Keep configuration changes narrowly scoped.
