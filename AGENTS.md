# Agent Instructions

This repository is a Markdown-based second brain and Obsidian vault. Treat the notes as the source of truth.

## Terminology

- `KB` or `kb` means the knowledge base: the Markdown files in this repository/vault.

## Core Principles

- Store knowledge in Markdown files.
- Preserve user-authored content unless explicitly asked to rewrite it.
- Prefer adding context over deleting context.
- Use relative Markdown links for internal references.
- Keep files readable in plain text and Obsidian.
- Avoid creating opaque databases, binary note formats, or tool-specific lock-in.
- When uncertain where something belongs, put it in `00-inbox/` and add enough context for later triage.

## Vault Structure

- `00-inbox/` - Unprocessed captures and temporary notes.
- `10-projects/` - Active outcomes with a finish line.
- `20-areas/` - Ongoing responsibilities and standards.
- `30-resources/` - Reference material organized by topic.
- `40-notes/` - Evergreen notes containing one durable idea per file.
- `50-archive/` - Inactive or completed material.
- `90-meta/` - Templates, indexes, workflows, and maintenance notes.

## How To Add Information

1. Decide whether the information is a capture, project, area, resource, evergreen note, or archive item.
2. Create or update the smallest useful Markdown file.
3. Add a short title, source/context if relevant, and links to related notes.
4. If the note creates a new important topic, update an index in `90-meta/indexes/`.
5. If the information is actionable, add it to the relevant project file or `TODAY.md`.

## Naming Conventions

- Use lowercase kebab-case filenames: `example-note-title.md`.
- Prefer descriptive names over dates unless the date is the main identifier.
- For daily notes, use ISO dates: `2026-05-16.md`.
- Keep folder names stable.

## Obsidian Compatibility

- Standard Markdown links are preferred: `[Note Title](../path/to/note.md)`.
- Wikilinks are allowed when useful: `[[note-title]]`.
- Do not require Obsidian plugins for core readability.
- Keep frontmatter optional and minimal.

## Search And Q&A Behavior

When asked to find or answer something from the vault:

1. Search filenames and content first.
2. Prefer evidence from existing notes over assumptions.
3. Cite the note paths used in the answer.
4. If the vault lacks an answer, say so clearly and suggest where the missing information should be captured.

## OpenSana

If the user mentions a ticket reference id in the format `ABC-123`, assume it is in OpenSana by default, not Linear or Jira. Use the configured MCP server to manage tickets in OpenSana.

### Personal Org Task Routing

For personal tasks in OpenSana, use the `Personal` organization (`organizationSlug: personal`) and route tasks by intent instead of asking the user where to put them.

Known personal projects:

- `DT` - `Daily Tasks` (`projectId: jn72s187qsp342xsxhk7ccbeyx84hce8`)
- `QT` - `Quick Tasks` (`projectId: jn71fymnsdyv01svx8b8jeq87n882z5j`)
- `PP` - `Personal Projects` (`projectId: jn7abt5a07c3ntpqw5hqexr6p18839tx`)
- `SD` - `Someday / Maybe` (`projectId: jn78daergmb9t3wzrgevydqe1h882wf4`)
- `PTB` - `Polymarket Trading Bot` (`projectId: jn7awtmg9gdb14f0zh1cksngc187zqnd`)

Each of these projects currently uses the default `Inbox` list (`ref: INBOX`).

Default routing rules:

- Put recurring habits, routines, and same-day maintenance tasks in `DT`, for example taking pills or cleaning the desk.
- Put one-off tasks that can be done in one sitting in `QT`, for example buying something, booking an appointment, sending a message, or doing a quick errand.
- Put multi-step outcomes that require planning or work across multiple sittings in `PP`, for example creating and printing a family photo album.
- Put inactive ideas, reminders, and "do this someday" items in `SD` when the user wants to remember them but is not committing to act soon.
- Put Polymarket trading bot work in `PTB`.

Do not create or use an "urgent tasks" project. Treat urgency as task metadata such as due date, status, or priority. If a task is ambiguous between `QT` and `PP`, choose `PP` when it likely needs research, sequencing, or more than one sitting; otherwise choose `QT`.
