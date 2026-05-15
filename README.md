# archora-skills

Academic research agent skills for use with Claude Code and other [Agent Skills](https://agentskills.io)-compatible tools.

Built on [Archora](https://archora2026.com) — a knowledge archiving platform for researchers and educators.

## Installation

```bash
npx skills add https://github.com/archora/archora-skills
```

Or manually copy the `skills/` directory into your Claude Code project's `.claude/` folder.

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

[Archora](https://archora2026.com) is a research platform that runs these agents on your channels and wiki. Use the web app for team research workflows; use these skills for local file-based workflows with Claude Code.

## License

MIT
