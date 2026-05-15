---
name: hypothesis
description: >
  Generates falsifiable, testable research hypotheses from notes, documents, and research content.
  Use when the user asks to brainstorm hypotheses, generate research questions, identify testable
  predictions, or discover patterns across their notes.
  Do NOT use for general Q&A — only when structured hypothesis output is needed.
license: MIT
metadata:
  author: archora
  version: "1.0"
  website: https://archora2026.com/
---

# Hypothesis Generation

Generate falsifiable, testable research hypotheses from the user's notes and research content.

## Workflow

1. **Read available content** — scan the notes, documents, or files the user provides
2. **Identify themes** — find recurring concepts, claims, relationships, and open questions
3. **Generate hypotheses** — produce 4–6 specific, falsifiable hypotheses
4. **Assign confidence** — rate each hypothesis HIGH / MEDIUM / LOW based on evidence in the content
5. **Format output** — present in structured markdown

## Output Format

```markdown
# 🧪 Hypothesis Analysis

## Summary
[2–3 sentences describing the main themes and what the hypotheses cover]

## Generated Hypotheses

### 🔴 [Hypothesis Title] — HIGH confidence

**Hypothesis:** [Specific, falsifiable statement with measurable prediction]

**Rationale:** [Which sources/notes support this, with specific references]

**Testable:** Yes | **Confidence:** HIGH

---

### 🟡 [Hypothesis Title] — MEDIUM confidence
...
```

## Confidence levels

- 🔴 **HIGH** — directly supported by multiple sources in the content
- 🟡 **MEDIUM** — partially supported or requires inference across sources
- 🟢 **LOW** — speculative but worth investigating; limited direct support

## Quality criteria for good hypotheses

- **Falsifiable**: Can be proven wrong — avoid "X may affect Y"
- **Specific**: Mentions measurable variables, not vague concepts
- **Grounded**: Traceable to actual content provided, not general knowledge
- **Novel**: Connects ideas across sources rather than restating the obvious

## Example

**Input:** Notes on predictive coding and synaptic plasticity

**Good hypothesis:**
> "Precision-weighted prediction errors in the Rao and Ballard model are encoded through spike-timing-dependent plasticity (STDP) in the visual cortex, such that altering STDP timing windows disrupts receptive field formation."

**Poor hypothesis:**
> "Synaptic plasticity is important for learning." ← not falsifiable, too vague
