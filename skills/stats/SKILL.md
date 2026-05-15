---
name: stats
description: >
  Detects statistical errors, logical fallacies, and methodological issues in research content.
  Checks for p-hacking, correlation/causation confusion, underpowered samples, multiple comparisons
  problems, overgeneralization, and other common fallacies. Use when the user asks to validate
  statistics, audit quantitative claims, check methodology, or find logical errors.
  Returns minimal output on purely theoretical content — most useful after empirical data is present.
license: MIT
metadata:
  author: archora
  version: "1.0"
  website: https://archora2026.com/
---

# Statistical Validator

Detect statistical errors and methodological fallacies in research content.

## Fallacy Types Detected

| Type | Description |
|------|-------------|
| `P_HACKING` | Selective reporting, post-hoc hypothesis changes, stopped when p<0.05 |
| `CORRELATION_CAUSATION` | Causal claims from correlational data |
| `SMALL_SAMPLE` | Sample size insufficient for claimed effect size |
| `MULTIPLE_COMPARISONS` | Multiple tests without Bonferroni/FDR correction |
| `OVERGENERALIZATION` | Results from specific sample applied to broader population |
| `CIRCULAR_REASONING` | Conclusion assumes what it claims to prove |
| `CHERRY_PICKING` | Selective evidence presentation |
| `EFFECT_SIZE_MISSING` | Statistical significance without practical effect size |
| `CONFOUND` | Alternative explanations not controlled for |

## Severity Levels

- **HIGH** — fatal flaw; invalidates the finding
- **MEDIUM** — significant concern; finding is weakened
- **LOW** — minor issue; addressable in discussion

## Output Format

### When issues are found:

```markdown
# 📐 Statistical Validation

> Found **3 issue(s)** requiring attention.

## Issues

### 🔴 HIGH — P_HACKING

**Post:** [reference to source]
**Claim:** "[exact statistical claim]"
**Issue:** [specific explanation of the problem]
**Suggestion:** [concrete fix]

---

### 🟡 MEDIUM — CORRELATION_CAUSATION
...

## Summary
[Overall assessment + priority order for fixes]
```

### When no issues are found:

```markdown
# 📐 Statistical Validation

> ✅ No statistical issues detected.

## Assessment
[Explanation: e.g., "This content is theoretical/conceptual and contains no quantitative claims to validate."]

## Proactive Checklist
When empirical data is added, watch for:
- [ ] [Domain-specific statistical concern 1]
- [ ] [Domain-specific statistical concern 2]
```

## When content has no statistics

If the content is purely theoretical or conceptual, note this explicitly and provide a domain-appropriate proactive checklist. Do NOT generate phantom issues.
