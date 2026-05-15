---
name: counterargument
description: >
  Generates rigorous devil's advocate critiques from methodological, theoretical, and practical
  perspectives. Use when the user asks to challenge their own work, find weaknesses, stress-test
  assumptions, anticipate reviewer objections, or argue against their research claims.
  Run BEFORE writing a draft for stronger papers.
license: MIT
metadata:
  author: archora
  version: "1.0"
  website: https://archora2026.com/
---

# Counterargument Generation

Generate adversarial critiques to stress-test research claims before writing or submitting.

## Perspectives

| Perspective | Icon | Focus |
|-------------|------|-------|
| **Methodological** | 🔬 | Study design, measurement validity, statistical approach, reproducibility |
| **Theoretical** | 📚 | Conceptual framework, alternative explanations, literature gaps |
| **Practical** | ⚙️ | Feasibility, generalizability, real-world applicability, ethical concerns |

## Workflow

1. **Identify the core claims** — extract the main hypotheses or arguments
2. **Generate 4–6 critiques** — at least one per perspective, more for weaker claims
3. **Rate severity** — HIGH (fatal flaw), MEDIUM (significant concern), LOW (minor point)
4. **Provide rebuttal strategy** — for each critique, suggest how to respond or strengthen the research

## Output Format

```markdown
# ⚔️ Counterargument Analysis

## Summary
[2–3 sentences: overall assessment of the research's vulnerability to critique]

## Counterarguments

### 📚 Theoretical Critique — [SHORT TITLE]

**Challenged Claim:** [Exact claim being challenged]

**Critique:** [Specific, evidence-grounded critique. Reference timescales, measurement limits,
alternative frameworks, or published contradictory evidence where possible.]

**Rebuttal Strategy:** [Concrete suggestion: what experiment, analysis, or argument would
address this critique]

---

### 🔬 Methodological Critique — [SHORT TITLE]
...
```

## Quality criteria

- **Specific**: Reference exact claims, timescales, measurements — not vague "this is uncertain"
- **Grounded**: Connect to actual limitations in the content, not generic criticism
- **Expert-level**: Write as a senior reviewer at a top journal would
- **Constructive**: Every critique ends with a path forward (rebuttal strategy)

## Examples of strong vs weak critiques

**Weak:** "The sample size might be too small."

**Strong:** "The proposed sample of n=15 animals achieves 80% power only for effect sizes of η²≥0.25. Given the typical effect sizes in STDP studies (η²=0.10–0.15, e.g., Bi & Poo 1998), this is underpowered. A power analysis targeting η²=0.12 would require n=38 per condition."
