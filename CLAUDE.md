# CLAUDE.md

This file provides guidance to Claude Code when working in this repository.

## What this repo is

A personal recipe collection (`jojo-kocht`) — markdown files originally exported from Google Keep. Language is German throughout.

## Structure

Each recipe or note is a standalone `.md` file in the repo root. There is no subdirectory structure.

## Common style guide

All recipes share the same skeleton, in this order:

1. `# Titel` (H1, one per file).
2. `*Bearbeitet: <Datum>*` — optional italic edit date, only if known. Never invent one.
3. `*Kurzbeschreibung.*` — optional italic intro. Longer background prose stays in this italic block too.
4. `*Portionen: ...*` or `*Für 500 g ...*` — optional italic meta line (yield, times). Not inside a heading.
5. `## Zutaten` — bullet list with `-`. Group with `### Untertitel` (e.g. `### Dip`, `### Füllung`) where needed. Tables are allowed when they read better (see the matcha recipe).
6. `## Zubereitung` — numbered list `1.`, steps in the `**Stichwort:** Text` form where it fits. Multi-phase recipes may add a second phase heading such as `## Backen (Am Morgen)`.
7. `## Profi-Tipp` — optional, singular. Further optional sections (e.g. `## Gerätehinweis`, `## Eiskalt-Variante`) may follow.

Non-recipe notes (shopping lists, how-tos) use the same H1 + optional italic date/intro, then a materials section (`## Zutaten` or `## Material`) and a steps section (`## Anleitung`), without the cooking sections.

## Conventions when adding or editing content

- Write in German.
- Keep the common style guide above: `## Zutaten` then `## Zubereitung` for recipes.
- Use `-` for bullet lists and `1.` for ordered steps. No `*` bullets, no `---` horizontal rules, no blockquotes.
- Add new recipes as a new `.md` file and link it in `README.md` under the appropriate section (Rezepte or Sonstiges). Every file in the repo must be linked there.
- File names are lowercase, hyphenated, descriptive (`my-recipe-name.md`).
- No frontmatter, no tags, no YAML — plain markdown only.
- When restyling an existing recipe, change only structure and formatting. Never alter ingredient amounts or step wording.
- After committing changes, always push to the remote.
