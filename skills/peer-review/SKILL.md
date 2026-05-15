---
name: peer-review
description: >
  Simulates a full academic journal peer review with EIC decision and 3 independent reviewers
  (Methodology Expert, Domain Specialist, Devil's Advocate). Scores 1–10, provides major/minor
  comments, and issues a final verdict: Accept, Minor Revision, Major Revision, or Reject.
  Use when the user asks for a peer review, journal-quality feedback, readiness assessment,
  or to simulate reviewer responses before submission.
license: MIT
metadata:
  author: archora
  version: "1.0"
  website: https://archora2026.com/
---

# Peer Review Simulation

Simulate a rigorous journal peer review process with multiple independent reviewers.

## Reviewers

| Role | Focus |
|------|-------|
| **Editor-in-Chief (EIC)** | Overall fit, quality, editorial decision |
| **Reviewer 1 — Methodology Expert** | Research design, statistical rigor, reproducibility |
| **Reviewer 2 — Domain Specialist** | Theoretical framework, literature coverage, contribution |
| **Reviewer 3 — Devil's Advocate** | Weaknesses, alternative interpretations, ethical concerns |

## Scoring

- **1–4**: Reject
- **5–6**: Major revision needed
- **7–8**: Minor revision; publishable with changes
- **9–10**: Accept; exceptional work

## Verdicts

- `ACCEPT` — publishable as-is
- `MINOR_REVISION` — small changes needed; likely accepted after revision
- `MAJOR_REVISION` — significant work required; re-review needed
- `REJECT` — fundamental issues; not suitable for this venue

## Output Format

```markdown
# 🔬 Peer Review Simulation

> **Final Decision: 🟠 Major Revision** | Overall Score: **6/10**

## Editor-in-Chief Decision

**Decision:** 🟠 Major Revision
**Score:** 6/10

[3–4 sentence editorial summary]

---

## Reviewer Reports

### 🔬 Reviewer 1: Methodology Expert

**Recommendation:** 🟠 Major Revision | **Score:** 6/10

[Overall impression]

**Major Concerns:**
- [Critical issue 1]
- [Critical issue 2]

**Minor Suggestions:**
- [Minor suggestion 1]

---
[... repeat for each reviewer ...]

## 🟠 Final Decision: Major Revision

### Priority Action Items

- [ ] [Most important revision 1]
- [ ] [Most important revision 2]
- [ ] [Most important revision 3]

| Reviewer | Score | Recommendation |
|----------|-------|----------------|
| Editor-in-Chief | 6/10 | 🟠 Major Revision |
| Methodology Expert | 6/10 | 🟠 Major Revision |
| Domain Specialist | 7/10 | 🟡 Minor Revision |
| Devil's Advocate | 5/10 | 🟠 Major Revision |
```

## Guidelines for honest reviews

- Score calibration: theoretical-only papers without original data should score 5–7 max
- Reviewers must disagree sometimes — a spread of 5–7 across reviewers is healthy
- Major concerns must reference specific claims or sections in the paper
- Minor suggestions must be genuinely minor — not disguised major concerns
- Devil's Advocate must find real weaknesses, not be contrarian for its own sake
