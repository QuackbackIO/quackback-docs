# CLAUDE.md

Documentation source for Quackback. Pure MDX content repo — no build tooling. Fetched by `QuackbackIO/website` at build time via GitHub API.

**Published at**: https://quackback.io/docs

## Structure

```
├── getting-started/       admin/            auth/
├── self-hosting/          integrations/     api/
├── users/                 developers/       mcp/
├── reference/             snippets/
├── docs.json              # Tab navigation manifest
├── STYLE_GUIDE.md         # Writing guide
```

## Frontmatter

```yaml
---
title: "Organize feedback with boards"           # Imperative for guides, noun for reference. <50 chars.
description: "Organize feedback into categories." # One sentence, <160 chars, starts with verb.
icon: "layout-grid"
---
```

## MDX Components

`<Tip>`, `<Note>`, `<Warning>`, `<Info>` — place at point of decision, not page end. API docs use multi-language code blocks (curl > JS > Python).

## Writing Style

See `STYLE_GUIDE.md`. Short sentences, direct address ("you"), present tense, no passive voice, no superlatives, no hedging. Imperative titles for guides, nouns for reference. Link concepts inline when first mentioned.

## Conventions

- Files: kebab-case. Links: absolute paths without extension (`/admin/boards`).
- Never add co-author trailers to commits
