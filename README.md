# archora-skills

[![Visit Archora](https://img.shields.io/badge/🌐%20archora2026.com-Visit%20Now-4f46e5?style=for-the-badge)](https://archora2026.com/)
[![GitHub](https://img.shields.io/badge/GitHub-archora--skills-181717?style=for-the-badge&logo=github)](https://github.com/richard-kim-79/archora-skills)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

Academic research agent skills for [Claude Code](https://claude.ai/code) and other [Agent Skills](https://agentskills.io)-compatible tools.

> Built on **[Archora](https://archora2026.com/)** — a knowledge archive & social network for researchers and educators.
> Run these same agents in your browser at **[archora2026.com](https://archora2026.com/)** ✨

## Installation

```bash
npx skills add https://github.com/richard-kim-79/archora-skills
```

Or manually copy the `skills/` directory into your project's `.agents/skills/` folder.

## Skills

| Skill | Description |
|-------|-------------|
| [hypothesis](skills/hypothesis) | Generate falsifiable research hypotheses from notes and documents |
| [validation](skills/validation) | Design experimental protocols to test each hypothesis |
| [draft](skills/draft) | Write an IMRaD-structured paper draft |
| [figure](skills/figure) | Generate matplotlib / Mermaid visualization code |
| [stats](skills/stats) | Detect statistical errors and logical fallacies |
| [counterargument](skills/counterargument) | Generate devil's advocate critiques |
| [peer-review](skills/peer-review) | Simulate journal peer review (EIC + 3 reviewers) |
| [synthesis](skills/synthesis) | Surface cross-cutting themes and insights |
| [wiki-sync](skills/wiki-sync) | Sync notes into a structured wiki knowledge base |

## Usage

Once installed, these skills activate automatically when you ask Claude to perform research tasks:

```
"Generate hypotheses from my notes"
"Write a paper draft based on this research"
"Give me a peer review of this draft"
"What are the weaknesses in my argument?"
```

## Recommended Workflow

Skills are designed to chain together across a full research pipeline:

```
┌─────────────┐
│  Raw Notes  │  (your Markdown files, PDFs, clippings)
└──────┬──────┘
       │
       ▼
┌─────────────┐     ┌──────────────┐
│  wiki-sync  │────▶│  synthesis   │  Organize & surface cross-cutting themes
└─────────────┘     └──────────────┘
       │
       ▼
┌─────────────┐
│ hypothesis  │  Generate falsifiable research questions
└──────┬──────┘
       │
       ▼
┌──────────────┐    ┌────────┐
│  validation  │───▶│ figure │  Design experiments + visualize data
└──────────────┘    └────────┘
       │
       ▼
┌───────┐    ┌───────┐
│ stats │    │ draft │  Validate claims + write IMRaD paper
└───────┘    └───┬───┘
                 │
                 ▼
    ┌─────────────────────┐
    │ counterargument      │  Stress-test before submission
    │ peer-review          │
    └─────────────────────┘
```

**Quick start chain (copy-paste into Claude):**

```
1. "wiki-sync 해줘" — organize notes into wiki
2. "이 노트들로 가설 생성해줘" — generate hypotheses
3. "각 가설에 대한 실험 설계 제안해줘" — design experiments
4. "통계 오류 확인해줘" — validate any stats
5. "논문 초안 작성해줘" — write the draft
6. "peer review 해줘" — simulate review
7. "반론 생성해줘" — stress-test before submission
```

## About Archora

**[→ archora2026.com](https://archora2026.com/)**

Archora is a research platform for academics and educators. Create channels, build wiki knowledge bases, and run AI research agents collaboratively in the browser.

| | Web App | Claude Code Skills |
|---|---|---|
| **Best for** | Team workflows, shared channels | Local files, personal research |
| **Setup** | Sign up at archora2026.com | `npx skills add` |
| **Agents** | Runs on your wiki & posts | Runs on local Markdown files |
| **Collaboration** | Multi-user, real-time | Single user |

Both use the same agent logic — pick whichever fits your workflow.

## License

MIT
