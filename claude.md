# Base Documentation

Technical documentation for Base (Ethereum L2). Built with Mintlify.

| Command | Description |
|---------|-------------|
| `mintlify dev` | Starts a local development server so you can preview your documentation changes live in your browser. Useful for checking layout, styling, and interactive components before publishing. |
| `/lint` | Runs a linter on your MDX files to detect formatting or syntax issues. Automatically fixes problems where possible to ensure consistent style across all documentation pages. |
| `/doc-feedback` | Generates a report on content quality, such as clarity, consistency, and adherence to writing guidelines. Helps contributors improve documentation before submitting a PR. |



## Structure

```
docs/
├── get-started/      # Intro, quickstarts
├── base-chain/       # Network, nodes, tools
├── base-account/     # Smart Wallet SDK
├── base-app/         # Agent development
├── mini-apps/        # MiniKit guides
├── onchainkit/       # React components (versioned)
├── cookbook/         # Tutorials
├── learn/            # Solidity, Ethereum basics
├── images/           # Assets by topic
├── snippets/         # Reusable MDX components
└── docs.json         # Navigation config
```

## Content Rules

**Frontmatter** (required):
```yaml
---
title: "Keyword-rich title"
description: "Value description"
---
```

**Writing**: American English, sentence case headings, second person ("you"), active voice.

**Code blocks**: Always specify language. Add filename or title. Use `highlight={}` for emphasis.

**Components**: See [mintlify-reference.md](mintlify-reference.md) for syntax.

**Images**: Wrap in `<Frame>`, include `alt` attribute.

## Navigation

Edit `docs.json` to add/remove pages. Add redirects when removing pages.

## References

| File | Purpose |
|------|---------|
| [content-instructions.md](content-instructions.md) | Writing guidelines |
| [mintlify-reference.md](mintlify-reference.md) | Component syntax |
| [scripts/README.md](scripts/README.md) | Linter usage |

## Before Committing

1. Run `/lint` and fix errors
2. Add redirects for removed pages
3. Verify links work
