---
name: figure
description: >
  Generates complete, runnable visualization code for research figures. Produces matplotlib/seaborn
  Python scripts for quantitative data and Mermaid diagrams for conceptual relationships, workflows,
  and taxonomies. Use when the user asks for charts, graphs, visualizations, figures, or diagrams.
  Produces code only — does not render images directly.
license: MIT
metadata:
  author: archora
  version: "1.0"
  website: https://archora2026.com
---

# Figure Generator

Generate publication-quality visualization code for research figures.

## Figure Types

| Type | Use for | Format |
|------|---------|--------|
| **matplotlib** | Quantitative data: bar charts, scatter plots, line graphs, heatmaps, box plots | Python |
| **seaborn** | Statistical visualizations: distributions, regressions, pair plots | Python |
| **Mermaid** | Conceptual diagrams: workflows, taxonomies, hierarchies, timelines | Mermaid |

## Decision guide

- Numbers, measurements, time series → **matplotlib/seaborn**
- Concepts, relationships, processes → **Mermaid**
- When in doubt: generate both

## Output Format

````markdown
## Figure 1: [Title]

**Caption:** [Full figure caption as it would appear in a paper — what is shown and the key takeaway]

**Description:** [What this figure shows and why it matters for the research]

**Type:** Python (matplotlib/seaborn)

```python
import matplotlib.pyplot as plt
import numpy as np

# [Complete, runnable code with realistic placeholder data]
plt.tight_layout()
plt.savefig('figure1.png', dpi=300)
plt.show()
```
````

## Code requirements

- **Complete and runnable** — no placeholders like `your_data_here`
- **All imports included** — never reference a library without importing it
- **Realistic placeholder data** — use domain-appropriate values and ranges
- **Publication quality** — `dpi=300`, proper axis labels, legend, title
- **Accessible colors** — avoid red/green only distinctions

## How to run

**Python figures:**
```bash
pip install matplotlib seaborn numpy
python figure1.py
```

**Mermaid diagrams:**
- Paste into [mermaid.live](https://mermaid.live)
- Or use any Markdown renderer that supports Mermaid (Obsidian, GitHub, etc.)
