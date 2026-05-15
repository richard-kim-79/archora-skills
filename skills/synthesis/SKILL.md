---
name: synthesis
description: >
  Synthesizes research notes and documents to surface cross-cutting themes, unexpected connections,
  and high-level insights not visible in individual pieces. Use when the user asks for an overview,
  thematic analysis, synthesis across notes, or to find patterns in their research collection.
license: MIT
metadata:
  author: archora
  version: "1.0"
  website: https://archora2026.com/
---

# Research Synthesis

Surface cross-cutting themes and insights by synthesizing across the full collection of notes.

## Workflow

1. **Read all provided content** — notes, documents, wiki pages
2. **Identify recurring themes** — concepts that appear across multiple sources
3. **Find unexpected connections** — links between sources that aren't explicitly stated
4. **Surface gaps** — important questions the content doesn't yet address
5. **Synthesize insights** — produce observations that go beyond any single source

## Output Format

```markdown
# 🔭 Research Synthesis

## Overview
[3–4 sentences: what this research is fundamentally about and its current state]

## Core Themes

### Theme 1: [Title]
[2–3 sentences describing the theme and which sources contribute to it]
*Sources: [list of relevant notes/docs]*

### Theme 2: [Title]
...

## Unexpected Connections
- **[Concept A] ↔ [Concept B]**: [Why this connection is interesting and what it might mean]
- ...

## Research Gaps
- [Important question not yet addressed by any source]
- ...

## Key Insights
1. [Cross-cutting insight that requires reading multiple sources together]
2. ...
```

## Quality criteria

- Insights must require **multiple sources** — don't just summarize individual documents
- Connections should be **non-obvious** — don't flag things already explicitly linked
- Gaps should be **specific** — not "more research needed" but "no source addresses X"
