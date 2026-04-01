---
name: research-idea-benchmark
description: This skill should be used when the user asks to "evaluate my research idea", "benchmark my research", "score my paper idea", "assess research quality", "check if my idea is publishable", "review my research design", or wants to evaluate a research idea against top journal standards. Provides a systematic 7-dimension rubric distilled from patterns in JFQA, JCF, Review of Finance, and leading finance/economics journals.
version: 0.1.0
---

# Research Idea Benchmark

Evaluate research ideas against empirical standards distilled from 50+ papers published in top finance and economics journals (JFQA, JCF, Review of Finance, and leading ESG/sustainability venues).

## When to Use

- Evaluating a new research idea before committing resources
- Assessing whether a research design is strong enough for a target venue
- Identifying the weakest dimension of a research proposal to strengthen
- Comparing multiple research directions to prioritize

## Evaluation Workflow

### Step 1: Gather the Research Idea

Request the user to provide their research idea in any format: a paragraph description, an abstract draft, a structured outline, or a verbal explanation. At minimum, extract:

1. **Research question**: What is being asked?
2. **Proposed method**: How will it be investigated?
3. **Target venue**: Which journal or conference tier?
4. **Data availability**: What data exists or needs to be collected?

If any of these are missing, ask targeted questions to elicit them before proceeding.

### Step 2: Score Across 7 Dimensions

Evaluate the idea against each dimension using the detailed rubric in `references/evaluation-rubric.md`. The 7 dimensions and their weights:

| # | Dimension | Weight | What It Measures |
|---|-----------|--------|-----------------|
| 1 | Research Question Quality | 20% | Precision, gap significance, testability |
| 2 | Theoretical Foundation | 15% | Theory grounding, competing hypotheses |
| 3 | Identification Strategy | 25% | Causal inference credibility |
| 4 | Data & Variable Construction | 15% | Novelty, quality, proxy validity |
| 5 | Robustness Architecture | 10% | Alternative explanations, sensitivity |
| 6 | Contribution Clarity | 10% | Novelty, multi-dimensional impact |
| 7 | Narrative Quality | 5% | Logical flow, persuasiveness |

**Critical rule**: Identification Strategy (Dimension 3) is the single most important dimension for empirical finance journals. A score below 4 on this dimension is a near-certain rejection at top-5 finance journals.

### Step 3: Generate the Evaluation Report

Produce a structured report with the following sections:

```
## Research Idea Benchmark Report

### Overview
[1-2 sentence summary of the research idea]

### Target Venue Assessment
[Venue name] | Estimated fit: [Strong/Moderate/Weak]

### Dimension Scores

| Dimension | Score | Key Strength | Key Weakness |
|-----------|-------|-------------|-------------|
| 1. Research Question | X.X/5 | ... | ... |
| 2. Theoretical Foundation | X.X/5 | ... | ... |
| 3. Identification Strategy | X.X/5 | ... | ... |
| 4. Data & Variables | X.X/5 | ... | ... |
| 5. Robustness | X.X/5 | ... | ... |
| 6. Contribution | X.X/5 | ... | ... |
| 7. Narrative | X.X/5 | ... | ... |

**Weighted Total: X.XX / 5.00**

### Referee Red Flags
[List any items from the "Referee Red Flag Checklist" that apply]

### Actionable Improvements
[Rank-ordered list of specific, concrete steps to strengthen the weakest dimensions]

### Comparable Published Papers
[2-3 published papers with similar research designs that succeeded, 
with notes on what made them work]
```

### Step 4: Provide Targeted Guidance

Based on the lowest-scoring dimensions, provide specific improvement strategies:

**For weak Identification Strategy (< 4)**:
- Suggest specific natural experiments, policy shocks, or instrumental variables relevant to the topic
- Reference the identification arsenal in `references/evaluation-rubric.md`
- Recommend specific econometric techniques

**For weak Research Question (< 3.5)**:
- Help reframe the question as a paradox or puzzle
- Identify the specific gap in existing literature
- Suggest competing hypotheses to pit against each other

**For weak Data/Variables (< 3.5)**:
- Suggest novel data sources or creative proxy constructions
- Reference exemplary proxy innovations from `references/paper-patterns.md`
- Recommend validation approaches

**For weak Contribution (< 3.5)**:
- Help position the paper against multiple literature streams
- Identify which contribution types (empirical, methodological, theoretical, policy) are achievable
- Suggest the "contribution statement formula" from `references/paper-patterns.md`

## Research Design Patterns

Consult `references/paper-patterns.md` for 7 recurring research design patterns extracted from top journals:

1. **Black Box Opening** — identifying the mechanism in an established relationship
2. **Resolution Paper** — introducing a dimension that resolves contradictory findings
3. **Policy Shock** — exploiting government policy for DiD identification
4. **Unintended Consequences** — documenting surprising spillover effects
5. **Proxy Innovation** — creating a new way to measure the unmeasurable
6. **Cross-Country Variation** — leveraging institutional differences
7. **Mechanism Decomposition** — breaking a main effect into sub-channels

When evaluating an idea, identify which pattern(s) it most closely follows and assess whether the idea fulfills that pattern's requirements.

## Scoring Interpretation

| Score Range | Assessment | Action |
|-------------|-----------|--------|
| 4.5 - 5.0 | Exceptional | Proceed to execution |
| 4.0 - 4.4 | Very Strong | Minor refinements, then proceed |
| 3.5 - 3.9 | Strong | Strengthen 1-2 dimensions before proceeding |
| 3.0 - 3.4 | Moderate | Significant redesign in weak areas |
| 2.5 - 2.9 | Weak | Fundamental rethinking needed |
| < 2.5 | Not Ready | Return to ideation stage |

**Minimum thresholds** for top finance journals:
- Identification Strategy >= 4.0
- Research Question >= 3.5
- No single dimension below 2.5

## The "Prior-Changing" Test (from Edmans, RF Editor)

The single most important question for evaluating any research idea:

> **"Does this paper change the reader's prior?"**

If a reader spends hours going through the paper, they should learn something they didn't know or couldn't have guessed. Apply this test ruthlessly:

- If the result can be predicted by chaining two known findings → **Convex combination** → Reject
- If it adds "just another" item to a known list → **Marginal contribution** → Reject
- If extending to new country/period without institutional reason → **Context extension** → Reject
- If documenting only one side of a tradeoff → **Incomplete answer** → Reject

See `references/editor-insights.md` for the full taxonomy of rejection patterns with editor quotes.

## Additional Resources

### Reference Files

- **`references/evaluation-rubric.md`** — Full 7-dimension rubric with scoring anchors, diagnostic questions, examples from published papers, plus editor rejection taxonomy
- **`references/paper-patterns.md`** — Recurring research design patterns, data source catalog, contribution statement formulas, and section-by-section benchmarks
- **`references/editor-insights.md`** — Editor decision-making insights from Edmans (1,000 Rejections at RF), Cochrane (Writing Tips), Mitton (Methodological Variation, RFS), and Armstrong et al. (Causality Redux). Covers the 6 deadly contribution sins, IV pitfalls, p-hacking quantification, and exposition standards.

### Training Data

The rubric was built from analysis of papers and methodological guides:
- **Papers**: 50+ papers from JFQA, JCF, Review of Finance, ESG/sustainability venues in `/Users/yw/Desktop/001processing/60_github_mirrors/training_data/topjournal/`
- **Editorial wisdom**: Edmans "Learnings From 1,000 Rejections" (RF editor, 998 rejections analyzed)
- **Methodological standards**: Mitton "Methodological Variation" (RFS 2022), Armstrong et al. "Causality Redux" (2022)
- **Writing craft**: Cochrane "Writing Tips for PhD Students" (2005), Jackwerth "Tips for the PhD" (2022)
- **Topics**: political economy, corporate governance, ESG, executive compensation, innovation, causal inference methodology
