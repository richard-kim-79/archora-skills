---
name: validation
description: >
  Designs detailed experimental protocols to validate research hypotheses. Each protocol includes
  independent variable, dependent variable, controls, sample size with power analysis, timeline,
  and expected outcome. Use when the user asks to design experiments, plan a study, propose
  validation methods, or test a specific hypothesis. Works best after hypothesis generation.
license: MIT
metadata:
  author: archora
  version: "1.0"
  website: https://archora2026.com/
---

# Experiment Design

Design rigorous experimental protocols to validate research hypotheses.

## Protocol Components

For each hypothesis, produce a complete protocol with:

| Field | Description |
|-------|-------------|
| **Design** | Experimental design type (RCT, quasi-experimental, longitudinal, in silico, etc.) |
| **Independent Variable (IV)** | What is manipulated |
| **Dependent Variable (DV)** | What is measured |
| **Controls** | Variables held constant |
| **Sample Size** | N per condition + power analysis (α=0.05, β=0.80, effect size) |
| **Timeline** | Phase-by-phase schedule |
| **Protocol** | Step-by-step procedure |
| **Expected Outcome** | What would confirm vs. refute the hypothesis |

## Power Analysis

Always include a power analysis. Standard parameters:
- α (Type I error rate): 0.05
- Power (1−β): 0.80
- Effect size: use domain-specific estimates or Cohen's conventions (small=0.2, medium=0.5, large=0.8)

Example: `30 simulations per condition (90 total, power analysis: α=0.05, β=0.80, η²=0.25)`

## Output Format

```markdown
# 🧫 Experiment Design

## Strategy Overview
[2–3 sentences: how the experiments collectively test the hypotheses]

## Proposed Experiments

### Experiment 1: [Design Type]

**Tests Hypothesis:** [Exact hypothesis being tested]

| Parameter | Detail |
|-----------|--------|
| **Design** | [Design type] |
| **Sample Size** | [N per condition with power analysis] |
| **Timeline** | [X months: phase breakdown] |

**Independent Variables:** [What is manipulated]
**Dependent Variables:** [What is measured]
**Control Variables:** [What is held constant]

**Protocol:**
1. [Step 1]
2. [Step 2]
...

**Expected Outcome:** [What confirms the hypothesis. What would refute it.]

---
```

## Feasibility check

Before finalizing a protocol, consider:
- Can the required equipment/resources be co-located?
- Is the timeline realistic for the sample size?
- Are controls sufficient to rule out confounds?
- Does the analysis plan address multiple comparisons if >1 DV?
