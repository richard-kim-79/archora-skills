---
name: wiki-sync
description: >
  Organizes research notes into a structured wiki knowledge base with wikilinks ([[slug]] syntax),
  cross-references, and an auto-generated index. Use when the user asks to build a wiki, organize
  notes into a knowledge base, create an index, or sync notes into a structured format.
license: MIT
metadata:
  author: archora
  version: "1.0"
  website: https://archora2026.com
---

# Wiki Sync

Organize research notes into a structured wiki knowledge base.

## Wiki Conventions

- **Slugs**: lowercase kebab-case (`protein-folding`, `hypothesis-1`)
- **Wikilinks**: `[[slug]]` for internal links, `[[slug|Display Text]]` for custom labels
- **Index**: always maintain a `index.md` with a table of all pages
- **One concept per page**: each page should focus on a single entity, concept, or topic
- **Sources section**: every page ends with a `## Sources` section listing where the info came from

## Workflow

1. **Audit existing notes** — list all files, identify what already has wiki structure
2. **Identify concepts** — extract key entities, topics, and relationships from unstructured notes
3. **Create/update pages** — one page per concept, with cross-links
4. **Build index** — generate or update `index.md`
5. **Report** — list new pages created, pages updated, links added

## Page Template

```markdown
# [Page Title]

[1–2 sentence summary of this concept]

## Overview
[Detailed content about this concept]

## Related Concepts
- [[related-slug-1]] — [brief description of relationship]
- [[related-slug-2]] — [brief description of relationship]

## Sources
- [Source name/file]
- [Source URL if applicable]

*Last updated: [date]*
```

## Index Template

```markdown
# Wiki Index

> Auto-maintained index of all wiki pages.

| Page | Summary | Updated |
|------|---------|---------|
| [[slug-1]] Page Title | One-line summary | YYYY-MM-DD |
| [[slug-2]] Page Title | One-line summary | YYYY-MM-DD |
```

## Rules

- Maximum 8 pages created per sync run (avoid overwhelming the user)
- Prefer updating existing pages over creating new ones for incremental syncs
- Never delete existing content — append or update sections
- Always rebuild the index after adding pages
