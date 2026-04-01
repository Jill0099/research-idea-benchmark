# Research Idea Benchmark

A Claude Code skill that evaluates research ideas against standards distilled from 50+ papers published in top finance and economics journals.

## What It Does

Scores research ideas across **7 weighted dimensions** before you commit months of work:

| # | Dimension | Weight | What It Measures |
|---|-----------|--------|-----------------|
| 1 | Research Question Quality | 20% | Precision, gap significance, testability |
| 2 | Theoretical Foundation | 15% | Theory grounding, competing hypotheses |
| 3 | **Identification Strategy** | **25%** | Causal inference credibility |
| 4 | Data & Variable Construction | 15% | Novelty, proxy validity, measurement |
| 5 | Robustness Architecture | 10% | Alternative explanations, sensitivity |
| 6 | Contribution Clarity | 10% | Novelty, multi-dimensional impact |
| 7 | Narrative Quality | 5% | Logical flow, persuasiveness |

Outputs a structured report with scores, referee red flags, and actionable improvements.

## Sources

### Published Papers (50+)
- **JFQA** — 20 papers (political economy, corporate governance, innovation)
- **JCF** — 9 papers (executive compensation, labor investment, geopolitical risk)
- **ESG/Sustainability venues** — 21 papers (green finance, sustainable investing, climate policy)
- **Review of Finance** — bibliography coverage

### Editorial & Methodological Wisdom
- **Edmans (2023)** — "Learnings From 1,000 Rejections" — 998 rejection patterns from Review of Finance editor
- **Mitton (2022, RFS)** — "Methodological Variation in Empirical Corporate Finance" — p-hacking quantification
- **Armstrong et al. (2022)** — "Causality Redux" — causal inference evolution in accounting/finance
- **Cochrane (2005)** — "Writing Tips for PhD Students" — paper organization principles
- **Jackwerth (2022)** — "Tips for the PhD in Empirical Financial Economics"

## Key Features

### Editor Rejection Taxonomy
6 deadly contribution sins from Edmans' 998 rejections:
- **Convex combination** — result predictable by chaining known findings
- **"Just another" determinant** — adding to a well-populated list
- **Research by matrix** — filling empty cells that are empty for a reason
- **Context extension** — same result in new country without institutional insight
- **One-sided tradeoff** — documenting only benefits without costs
- **Curiosum** — surprising but economically trivial

### 7 Research Design Patterns
Recurring structures from top-journal papers:
1. Black Box Opening — identifying mechanisms in established relationships
2. Resolution Paper — introducing a dimension that resolves contradictions
3. Policy Shock — exploiting government policy for DiD identification
4. Unintended Consequences — documenting surprising spillover effects
5. Proxy Innovation — creating new ways to measure the unmeasurable
6. Cross-Country Variation — leveraging institutional differences
7. Mechanism Decomposition — breaking main effects into sub-channels

### P-Hacking Risk Assessment
From Mitton (RFS 2022): with 10 routine methodological choices, **70%+ of random variables** appear significant at 5%. The skill flags vulnerable dimensions.

## Installation

### As a Claude Code Skill
Copy to your Claude Code skills directory:

```bash
cp -r . ~/.claude/skills/research-idea-benchmark/
```

### Trigger Phrases
- "evaluate my research idea"
- "benchmark my research"
- "score my paper idea"
- "assess research quality"
- "check if my idea is publishable"
- "review my research design"

## File Structure

```
research-idea-benchmark/
├── SKILL.md                              # Main skill (workflow + triggers)
└── references/
    ├── evaluation-rubric.md              # 7-dimension rubric with scoring anchors
    ├── paper-patterns.md                 # Research design patterns + templates
    └── editor-insights.md               # Editorial decision-making criteria
```

## Scoring Interpretation

| Score | Assessment | Venue |
|-------|-----------|-------|
| 4.5 - 5.0 | Exceptional | Top 3 (JF, JFE, RFS) |
| 4.0 - 4.4 | Very Strong | Top field (JFQA, JCF, RF) |
| 3.5 - 3.9 | Strong | Good field journal |
| 3.0 - 3.4 | Moderate | Needs strengthening |
| < 3.0 | Weak | Fundamental redesign needed |

**Hard rule**: Identification Strategy must score ≥ 4 for any top-5 finance journal.

## Related Skills

- [`top-journal-writing-mentor`](https://github.com/Jill0099/Finance-top-journal-writing-mentor) — Writing style mentor for the same journals (downstream: after idea is validated)
- `research-ideation` — Research startup workflow (upstream: generates candidate ideas)
- `paper-self-review` — Post-execution quality checklist (downstream: checks finished papers)

## License

All rights reserved.
