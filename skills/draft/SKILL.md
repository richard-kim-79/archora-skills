---
name: draft
description: >
  Writes a complete IMRaD-structured academic paper draft (Abstract, Introduction, Related Work,
  Methods, Results, Discussion, Conclusion, References) from the user's notes, documents, and
  wiki content. Use when the user asks to write a paper, create a manuscript, generate a draft,
  or produce academic writing. Do NOT use for short summaries — only for full paper-length output.
license: MIT
metadata:
  author: archora
  version: "1.0"
  website: https://archora2026.com/
---

# Paper Draft Generation

Generate a complete IMRaD-structured academic paper draft from research notes and documents.

## IMRaD Structure

| Section | Purpose | Length |
|---------|---------|--------|
| **Abstract** | Background, objective, methods, findings, conclusions | 250–300 words |
| **Introduction** | Problem, motivation, gap, contribution | 400–600 words |
| **Related Work** | Prior literature organized by theme | 500–800 words |
| **Methods** | How the research was/will be conducted | 400–600 words |
| **Results** | What was found (or projected findings) | 300–500 words |
| **Discussion** | Interpretation, implications, limitations | 400–600 words |
| **Conclusion** | Summary, contributions, future work | 200–300 words |
| **References** | All cited sources | As needed |

## Workflow

1. **Gather content** — read all provided notes, wiki pages, and documents
2. **Identify the core contribution** — what is new and why does it matter?
3. **Map citations** — track which sources support which claims
4. **Draft section by section** — follow IMRaD order
5. **Add inline citations** — use `[Author, Year]` or `[Source Title]` format
6. **Flag gaps** — mark sections needing real data with `> ⚠️ [PROJECTED — add empirical data]`

## Citation format

Use the actual title or author of notes/documents you read:

```markdown
Predictive coding theory proposes... [Rao & Ballard, 1999]
```

At the end, add a References section listing all cited sources.

## Handling missing data

When the research doesn't have empirical results yet, write projected results based on the hypotheses — but clearly mark them:

```markdown
> ⚠️ **Projected Results** — Replace with actual experimental data before submission.

Based on the experimental design, we expect...
```

## Quality checklist

- [ ] Abstract covers all 5 components (background, objective, methods, findings, conclusions)
- [ ] Introduction ends with a clear statement of contribution
- [ ] Every major claim has an inline citation
- [ ] Methods section is specific enough to reproduce
- [ ] Discussion addresses alternative interpretations
- [ ] Limitations section is honest, not defensive
