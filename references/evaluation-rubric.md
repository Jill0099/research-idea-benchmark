# Research Idea Evaluation Rubric — Top Journal Benchmark

This rubric is distilled from patterns observed across 50+ papers published in JFQA, JCF, Review of Finance, and leading ESG/sustainability venues. Each dimension is scored 1-5 with specific anchors.

---

## Dimension 1: Research Question Quality (Weight: 20%)

Evaluates whether the research question is precise, testable, and addresses a meaningful gap.

### Scoring Anchors

| Score | Description |
|-------|-------------|
| 5 | Question addresses a fundamental tension or paradox in the literature; fills a clearly documented gap; has broad implications beyond the immediate field |
| 4 | Question is well-motivated with a clear gap; testable and specific; contributes to an active debate |
| 3 | Question is reasonable but the gap is incremental; motivation relies on "limited evidence" rather than a clear void |
| 2 | Question is descriptive or confirmatory; gap is not clearly articulated; "me too" research |
| 1 | Question is trivial, already answered, or untestable |

### Diagnostic Questions
- Does the question arise from a genuine contradiction or puzzle in existing findings?
- Can the question be stated as a clear hypothesis with a predicted sign/direction?
- Would the answer change how we think about a broader phenomenon?
- Is there a clear "so what" for practitioners, policymakers, or subsequent researchers?

### Patterns from Top Journals
- **Paradox-driven**: "Why do similar firms adopt vastly different policies?" (Hutton et al., 2014, JFQA)
- **Resolution-seeking**: "Can distinguishing material vs. immaterial ESG resolve contradictory findings?" (Khan et al., HBS)
- **Policy-relevant**: "Does pay restriction reduce M&A activity as an unintended consequence?" (Lan & Pan, 2026, JCF)
- **Mechanism-revealing**: "Through what channels does corruption impede innovation?" (Ellis et al., 2020, JFQA)

---

## Dimension 2: Theoretical Foundation & Hypothesis Development (Weight: 15%)

Evaluates whether the hypotheses are grounded in established theory and logically derived.

### Scoring Anchors

| Score | Description |
|-------|-------------|
| 5 | Hypotheses derive from a clear theoretical framework; competing hypotheses explicitly stated; predictions are non-obvious and distinguishable |
| 4 | Solid theoretical grounding; main hypothesis clearly stated; at least one alternative hypothesis considered |
| 3 | Reasonable theoretical motivation but hypotheses are somewhat predictable; limited consideration of alternatives |
| 2 | Thin theoretical basis; hypotheses are intuitive but not formally derived; no competing predictions |
| 1 | No theoretical framework; hypotheses are ad hoc or post-hoc rationalizations |

### Diagnostic Questions
- Are competing theories explicitly pitted against each other?
- Do the hypotheses generate different empirical predictions that can be distinguished?
- Is the theoretical mechanism specific enough to guide empirical tests?

### Patterns from Top Journals
- **Competing hypotheses**: "Value creation vs. agency cost theory" in ESG literature (Gillan et al., 2021)
- **Behavioral consistency theory**: Political ideology → financial conservatism → corporate policies (Hutton et al., 2014)
- **Real options theory**: Geopolitical risk → labor investment inefficiency via option value of waiting (Ji et al., 2026)
- **Theoretical translation**: Carbon tax effects can be "translated" into capital cost equivalents (Pedersen, 2023)

---

## Dimension 3: Identification Strategy & Causal Inference (Weight: 25%)

The single most critical dimension for top empirical finance journals. Evaluates whether the research design can credibly establish causality.

### Scoring Anchors

| Score | Description |
|-------|-------------|
| 5 | Clean natural experiment or quasi-experiment with credible exogeneity; parallel trends validated; multiple identification strategies that converge; addresses all major endogeneity concerns |
| 4 | Strong quasi-experimental design (DiD, IV, RDD) with reasonable exclusion restriction arguments; placebo tests included |
| 3 | Standard identification approach with some endogeneity mitigation; acknowledges limitations but doesn't fully resolve them |
| 2 | Relies primarily on OLS with fixed effects; endogeneity concerns partially addressed |
| 1 | No causal identification; purely correlational analysis |

### Key Elements of a Score-5 Strategy
1. **Exogenous shock**: A policy change, natural disaster, regulatory reform, or institutional event that creates treatment/control variation
2. **Parallel trends**: Pre-treatment trends are indistinguishable between treatment and control groups
3. **Exclusion restriction**: The instrument affects the outcome ONLY through the proposed channel
4. **Multiple approaches**: Natural experiment + IV + additional robustness converge on same conclusion
5. **Placebo tests**: Falsification tests show no effect where none should exist

### Identification Arsenal (from Top Papers)

| Method | Example | Paper |
|--------|---------|-------|
| DiD with policy shock | China 2014 SOE pay restriction as treatment | Lan & Pan (2026), Cao et al. (2026) |
| Natural experiment (macro shock) | 9/11 attacks, Lehman bankruptcy as uncertainty shocks | Hutton et al. (2014) |
| Natural experiment (micro shock) | CEO death-induced turnover | Hutton et al. (2014) |
| Instrumental variables | Founder's home-state corruption as IV for local corruption | Ellis et al. (2020) |
| PSM-DiD | Propensity-score matched firms + DiD | Lan & Pan (2026), Mobbs & Zhang (2026) |
| Cross-country variation | Employment protection legislation as institutional variation | Ji et al. (2026) |
| Triple difference (DDD) | Pay-size elasticity interaction in DiD framework | Lan & Pan (2026) |
| Calendar-time portfolio | Long-short portfolios with factor model attribution | Khan et al. (HBS) |
| RDD | Shareholder proposal vote margin as discontinuity | Hong & Shore (2023) |

### Red Flags
- Claiming causality from panel regressions with only firm/year fixed effects
- IV with questionable exclusion restriction and no over-identification test
- DiD without parallel trends test or pre-treatment falsification
- "Natural experiment" that is actually anticipated or endogenous

---

## Dimension 4: Data & Variable Construction (Weight: 15%)

Evaluates novelty and quality of data sources, and creativity in constructing key variables.

### Scoring Anchors

| Score | Description |
|-------|-------------|
| 5 | Novel dataset or creative combination of existing data; key variable is a methodological contribution in itself; measurement validated through multiple approaches |
| 4 | Well-chosen data sources; key variable construction is thoughtful with validation checks; sample is comprehensive |
| 3 | Standard databases; variables follow established conventions; adequate sample |
| 2 | Limited data; key variable may have measurement issues; small or unrepresentative sample |
| 1 | Data quality concerns; key variable poorly justified; survivorship or selection bias |

### Diagnostic Questions
- Does the variable construction itself represent a contribution?
- Are proxy variables validated against direct measures?
- Is the sample large enough for the identification strategy?
- Are there multiple proxy measures for robustness?

### Exemplary Variable Construction
- **Republican Index (REP)**: FEC political donation records → manager-level ideology measure, validated against self-reported party affiliation and personal mortgage leverage (Hutton et al., 2014)
- **Materiality classification**: Hand-mapping SASB industry guidelines to KLD firm-level data, with signal purification via orthogonalization (Khan et al., HBS)
- **Pay-size elasticity**: Triple interaction measuring how pay responds to firm size, capturing "growth incentive" mechanism (Lan & Pan, 2026)
- **Abnormal labor investment**: Deviation from optimal labor investment predicted by economic fundamentals (Ji et al., 2026; Cao et al., 2026)

---

## Dimension 5: Robustness & Alternative Explanations (Weight: 10%)

Evaluates how systematically the paper addresses competing explanations and validates results.

### Scoring Anchors

| Score | Description |
|-------|-------------|
| 5 | Systematically addresses all plausible alternative explanations; multiple robustness checks (alternative measures, subsamples, specifications); falsification/placebo tests |
| 4 | Addresses major alternative explanations; reasonable set of robustness checks |
| 3 | Some robustness checks but gaps in addressing alternatives |
| 2 | Minimal robustness; obvious alternatives not discussed |
| 1 | No robustness analysis |

### Standard Robustness Architecture (from Top Papers)
1. **Alternative proxy variables**: Replace key independent variable with alternative measures
2. **Alternative specifications**: Add/remove controls, change fixed effects structure
3. **Subsample analysis**: Exclude special cases (e.g., financial firms, crisis periods)
4. **Competing hypotheses tests**: Design tests that can distinguish between your story and alternatives
5. **Placebo/falsification**: Show null effect where theory predicts none
6. **Matched samples**: PSM or entropy balancing to address selection bias
7. **Addressing concurrent events**: Control for contemporaneous policy changes or shocks

### Exemplary Robustness
- Hutton et al. (2014): Excluded "political connection" explanation by controlling for connection proxies, removing incumbent-party donations, and using IV
- Lan & Pan (2026): Controlled for concurrent anti-corruption campaign using provincial crime rates and corruption perception indices
- Khan et al. (HBS): Orthogonalized ESG scores against firm fundamentals to isolate pure sustainability signal

---

## Dimension 6: Contribution Clarity & Novelty (Weight: 10%)

Evaluates whether contributions are clearly articulated and genuinely advance knowledge.

### Scoring Anchors

| Score | Description |
|-------|-------------|
| 5 | Opens a new research area or provides a paradigm shift; contributions are multi-dimensional (empirical + methodological + theoretical); clear implications for practice and policy |
| 4 | Significant advancement within established area; at least one novel contribution beyond incremental findings |
| 3 | Incremental but solid contribution; extends existing work to new context or data |
| 2 | Contribution is marginal; mainly confirms existing findings in slightly different setting |
| 1 | No clear contribution beyond replication |

### Contribution Taxonomy (from Top Papers)

| Type | Example |
|------|---------|
| **Open new field** | First to bring political ideology into corporate finance (Hutton et al., 2014) |
| **Resolve paradox** | Materiality distinction resolves contradictory ESG findings (Khan et al., HBS) |
| **Methodological innovation** | Using FEC donations as ideology proxy; SASB-KLD hand-mapping |
| **Mechanism identification** | Pay-size elasticity as the channel for pay restriction → M&A decline (Lan & Pan, 2026) |
| **Framework creation** | "Seven tests" framework for CSR motivation evaluation (Hong & Shore, 2023) |
| **Policy evaluation** | Unintended consequences of SOE pay restriction on strategic decisions |
| **Theoretical bridge** | Unified model connecting carbon pricing and green finance (Pedersen, 2023) |

---

## Dimension 7: Narrative Quality & Paper Architecture (Weight: 5%)

Evaluates the logical flow and persuasiveness of the paper's argument.

### Scoring Anchors

| Score | Description |
|-------|-------------|
| 5 | Compelling narrative arc; each section builds naturally on the previous; reader never questions "why am I reading this"; abstract is a masterpiece of compression |
| 4 | Clear logical flow; well-organized; good transitions between sections |
| 3 | Adequate organization; some sections feel disconnected; motivation could be stronger |
| 2 | Disjointed flow; reader gets lost; weak motivation-to-method connection |
| 1 | No clear narrative; sections feel random |

### The Top-Journal Narrative Arc
1. **Hook**: Start with a broad, relatable tension or real-world observation
2. **Gap**: Narrow to the specific puzzle that existing literature cannot explain
3. **Preview**: Clearly state what this paper does and finds (in the abstract and intro)
4. **Theory**: Develop the theoretical basis for predictions
5. **Design**: Present identification strategy emphasizing credibility
6. **Results**: Present findings building from baseline to mechanism to robustness
7. **Implications**: End with what we now know that we didn't before

---

## Overall Scoring

| Total Score | Assessment | Publication Readiness |
|-------------|-----------|----------------------|
| 4.5 - 5.0 | Exceptional | Top 3 journal (JF, JFE, RFS) |
| 4.0 - 4.4 | Very Strong | Top field journal (JFQA, JCF, RF, RCFS) |
| 3.5 - 3.9 | Strong | Good field journal with revisions |
| 3.0 - 3.4 | Moderate | Needs significant strengthening in 1-2 dimensions |
| 2.5 - 2.9 | Weak | Fundamental redesign needed |
| < 2.5 | Not Ready | Back to ideation stage |

### Minimum Thresholds for Top Journals
- **Identification Strategy**: Must score >= 4 for any top-5 finance journal
- **Research Question**: Must score >= 3.5
- **No dimension below 2.5**: A single weak dimension can sink a paper

---

## Quick Diagnostic: The "Referee Red Flag" Checklist

These are common reasons top-journal referees recommend rejection:

- [ ] "The identification strategy is unconvincing" — endogeneity not addressed
- [ ] "The contribution is incremental" — extends to new country/period without new insight
- [ ] "The mechanism is unclear" — correlation without explanation
- [ ] "Alternative explanations not addressed" — obvious competing story ignored
- [ ] "The economic magnitude is small" — statistically significant but economically trivial
- [ ] "The sample is too narrow" — results may not generalize
- [ ] "The variable construction is questionable" — proxy validity not established
- [ ] "The paper is poorly positioned" — fails to engage with key related work
- [ ] "The results are not robust" — sensitivity analysis reveals fragility
- [ ] "The theoretical motivation is weak" — hypotheses feel post-hoc

---

## Editor's Rejection Taxonomy (from Edmans, "Learnings From 1,000 Rejections")

These are the most common rejection patterns from 998 rejections at Review of Finance, organized by category. Consult `references/editor-insights.md` for detailed extracts and examples.

### Contribution Rejections (~50% of desk rejections)

| Pattern | Description | Test |
|---------|-------------|------|
| **Convex combination** | X→Z and Z→Y are known, so X→Y is predictable | Can the result be derived by chaining existing papers? |
| **"Just another" determinant** | Adding one more variable to a well-populated list | Would a survey paper mention this result? |
| **Research by matrix** | Finding empty X-Y cells in literature, but the cell is empty because it's uninteresting | Is the question interesting, or just unstudied? |
| **Context extension** | Same result in new country/industry/period without new institutional insight | Would a reader Bayesian update after reading? |
| **One-sided tradeoff** | Documenting only benefits without costs (or vice versa) when the question is about overall value | Does the paper answer its own research question? |
| **Curiosum** | Finding something surprising but economically trivial or out-of-scope | Is this a "wrinkle" or a first-order finding? |

### Execution Rejections

| Pattern | Description |
|---------|-------------|
| **Invalid IV: peer group averages** | Industry/group averages soak up firm-level omitted variables |
| **Invalid IV: lagged X** | Within-system instrument affected by same endogeneity |
| **Statistical IV "proof"** | Over-identification tests cannot prove validity (unobservable error term) |
| **Undirected hypotheses** | Kitchen-sink regressions without predicted signs; "would the opposite result change anything?" |
| **Imprecise hypotheses** | Theory predicts effect on Y1 but paper tests Y2, with unclear Y1-Y2 link |
| **Uninformative channels** | Documenting which channel operates when all channels have the same implication |
| **log(1+Y) problem** | Arbitrary constant addition before log transform; use Poisson instead (Cohn, Liu, Wardlaw 2022) |

### Methodological Variation Risk (from Mitton, RFS 2022)

With discretion over 10 routine choices, **70%+ of random variables** appear significant at 5%. The most dangerous choices:

1. **Dependent variable selection**: 61 unique profitability measures in top-3 journals
2. **Variable transformation**: log vs. level vs. dummy
3. **Outlier treatment**: Winsorize/trim cutoff choice

When evaluating: Can the research idea survive alternative reasonable methodological choices?
