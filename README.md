# Quackback Documentation

This repository contains the documentation for [Quackback](https://github.com/QuackbackIO/quackback), the open-source customer feedback platform.

## Structure

```
docs/
├── index.mdx              # Documentation home
├── getting-started.mdx    # Getting started guide
├── self-hosting.mdx       # Self-hosting guide
└── [section]/             # Additional sections
    └── [page].mdx
```

## Writing Documentation

Each documentation page is an MDX file with frontmatter:

```mdx
---
title: "Page Title"
description: "A brief description for SEO and search"
order: 1
---

# Page Title

Your content here...
```

### Frontmatter Fields

| Field | Required | Description |
|-------|----------|-------------|
| `title` | Yes | Page title displayed in sidebar and browser |
| `description` | Yes | Meta description for SEO |
| `order` | No | Sort order within section (default: 99) |

### Components

You can use custom components in your MDX:

```mdx
<Callout type="info" title="Note">
  This is an informational callout.
</Callout>

<Callout type="warning" title="Warning">
  This is a warning callout.
</Callout>
```

Callout types: `info`, `warning`, `error`, `success`

## Contributing

1. Fork this repository
2. Create a new branch for your changes
3. Make your edits to the MDX files
4. Submit a pull request

## License

MIT License - see [Quackback](https://github.com/QuackbackIO/quackback) for details.
