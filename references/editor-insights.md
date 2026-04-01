# Editor & Methodological Insights for Research Evaluation

Distilled from PhD advice literature by Edmans (2023), Cochrane (2005), Jackwerth (2022), Mitton (2022, RFS), and Armstrong et al. (2022). These insights inform the evaluation rubric with real editorial decision-making criteria.

---

## From Alex Edmans: "Learnings From 1,000 Rejections" (Review of Finance)

### The Contribution Bar

The core principle: **A paper must change the reader's prior.** If a reader spends hours going through a paper, they should learn something they didn't know or couldn't have guessed beforehand. A strictly positive contribution is insufficient; it must be **significant**.

**Litmus test**: Would this finding likely be included in a survey paper on the topic?

### The 6 Deadly Contribution Sins

#### Sin 1: "Convex Combination" Result
> "We already know that X affects Z, and Z affects Y. Thus, your paper is a convex combination of results already known."

If the result can be predicted by chaining existing findings, the contribution is near-zero.

#### Sin 2: "Just Another" Determinant/Outcome
> "X seems to be 'just another' determinant of Y to add to the long list... It is unlikely that a survey paper will mention the effect of X."

Adding one more row to a well-populated matrix of known relationships is insufficient.

#### Sin 3: "Research by Matrix" Trap
Scouring literature to find that X1→Y1, X1→Y2, X2→Y1 are known but X2→Y2 is not. The empty cell may be empty because the question is uninteresting, not because it's unexplored.

#### Sin 4: "Extension to Another Context" Without New Insight
> "You are clear that you are the first to study the effect of X on Y in the UK. However, unless there are plausible reasons for why the US results would not automatically extend to the UK, a reader would not Bayesian update much."

Extending to another country, industry, crisis, or time period needs a reason why results might differ.

#### Sin 5: "One-Sided Tradeoff"
> "The big question is whether the increase in Y is worth it compared to the cost of X... You don't actually answer the question of whether X creates value."

Documenting only benefits (or only costs) when the research question is about overall value.

#### Sin 6: "Curious but Unimportant"
> "Your paper risks being seen as a 'curiosum' — finding a consequence of X that's curious... but not important compared to all the other effects."

The "wrinkle" problem: finding something surprising but economically trivial.

### Hypothesis Requirements

**Strength**: Must be strong enough that a significant correlation is unlikely to be spurious. Researchers can always reverse-engineer a hypothesis after finding a result.

**Precision**: Hypothesis must match what is actually tested. If theory predicts effects on Y1 but you test Y2, the link between Y1 and Y2 must be clear and unambiguous.

**Directionality**: Kitchen-sink regressions without directional predictions are unpublishable. "Would our view of the world be any different if you found the opposite result?"

**Conflicting ≠ Unclear**: Having two theories predict opposite signs is fine (the data can adjudicate). Having no theory predict any sign is not.

### Instrumental Variable Pitfalls (Editor's Perspective)

1. **Peer group averages as IV**: "Nearly never valid since any omitted variable at the individual firm level is simply soaked up at the group level" (citing Gormley & Matsa, 2013)
2. **Lagged X as IV**: "Valid instruments come from outside the system; this instrument is within the system" — affected by same endogeneity concerns
3. **Statistical tests cannot prove validity**: "An instrument is invalid if correlated with the error term. Since the error term is unobservable, this correlation cannot be tested."
4. **Appealing to prior papers**: "Just because other papers used the same instrument does not mean that it is valid" — methods evolve and standards rise

### Channel Identification

Documenting channels is publishable only when the channel **changes the interpretation**:
- If all channels through which X→Y are efficiency-consistent, showing which channel dominates doesn't change our view of desirability
- But if channels differ in sign (one is efficiency, another is myopia), identifying which matters is important

### Economic Significance

> "One guideline is that the abstract should contain one number of economic significance that the reader can take away, remember, and cite."

Examples of memorable numbers:
- Gompers, Ishii, and Metrick (2003): 8.5% abnormal returns to governance-sorted portfolios
- Holderness (2009): 96% of firms have blockholders

### Exposition Red Lines

- **Introduction max**: ~6 pages (11 pages is "far in the right tail")
- **No "clearing your throat"**: Don't start with philosophy or importance of the broad topic
- **Abstract must be concrete**: Say what you find, not what you look for
- **"Change" is vague**: Use "increase" or "decrease" — finance involves directional relationships
- **Footnotes signal disorganization**: "Having lots of footnotes gives the impression that the authors are not really sure what is central"

---

## From Todd Mitton: "Methodological Variation in Empirical Corporate Finance" (RFS, 2022)

### The P-Hacking Risk Quantification

**Key finding**: Given discretion over just 10 routine methodological decisions, a researcher could report that **over 70% of randomly generated variables** are statistically significant determinants of leverage at the 5% level.

### Top 3 P-Hacking Dimensions (by impact on t-statistics)

1. **Dependent variable selection**: 61 unique profitability measures found in top-3 journals, including 26 unique definitions of ROA alone. Median correlation among top-10 alternatives = 0.33
2. **Variable transformation**: log vs. level, continuous vs. dummy, log(1+Y) vs. Poisson
3. **Outlier treatment**: Winsorize vs. retain vs. trim; 1%/5%/other cutoffs

### How Often Are Choices Explained?

| Decision | % of papers that explain the choice |
|----------|-------------------------------------|
| Dependent variable selection | 22% |
| Outlier treatment | 6% |
| Continuous-to-dummy conversion | 19% |
| Control variable inclusion | Varies widely |

### Implications for Evaluation

When evaluating a research idea, assess whether:
- The dependent variable choice is theoretically motivated or cherry-picked
- The paper is robust to alternative standard measures
- Outlier treatment is justified, not just conventional
- Discretization of continuous variables has economic rationale

---

## From Armstrong et al.: "Causality Redux" (2022)

### Key Framework: Theory Must Guide Causal Inference

> "Without knowledge of the underlying data generating process, it is hard to say which econometric specification is the 'better identified specification.' This is where domain expertise and theory fits in."

It is NOT sufficient to just "find a setting" and "argue as-if randomness" and "run a canned DiD."

### Three Pillars of Causal Inference

1. **Theory and institutional knowledge** — not just econometric technique
2. **Triangulation** — across multiple research designs, specifications, and measures
3. **Complementarity** — quasi-experimental and non-experimental evidence together

### "Exogenous" vs. "As-if Random"

These are NOT synonyms. An event can be exogenous (e.g., a natural disaster) without providing as-if random variation in the treatment of interest. The variation must be in the **treatment**, not just in the **timing**.

### Non-Experimental Evidence Has Value

When quasi-experiments are impractical, causal inference can still be strengthened through:
- Economic theory ruling out alternatives
- Developing and falsifying alternative explanations
- Triangulating across multiple settings and measures
- Appropriate caveating

---

## From John Cochrane: "Writing Tips for Ph.D. Students" (2005)

### The One-Contribution Rule

> "Figure out the one central and novel contribution of your paper. Write this down in one paragraph."

Everything in the paper exists to support this one contribution. If a section doesn't help the reader understand or believe the main result, it should be cut.

### "Triangular/Newspaper" Style vs. "Joke/Novel" Style

- **Good**: Start with the punchline (main result), then fill in details for readers who want more
- **Bad**: Long windup, literature review, model, preliminary results, finally Table 12 with the main finding

> "There should be nothing before the main result that a reader does not need to know in order to understand the main result."

### Practical Benchmarks

- Abstract: 100-150 words, concrete, say what you **find** not what you **look for**
- Introduction: 3 pages max
- Literature review: Separate section, focus on 2-3 closest papers, not JEL-style survey
- Theory: "Work out only the specialized model that you actually take to data"
- Conclusion: Short, don't restate all findings

---

## From Jackwerth: "Tips for the PhD in Empirical Financial Economics" (2022)

### Research Question Development

1. **Start close to existing work** for first paper — add a factor, condition on a new variable
2. **Job market paper must stand out** — break conventions, think broadly about what's puzzling
3. **Use simplest econometric technique** that gets the job done — "Start with OLS unless you really need a nonparametric kernel regression"
4. **Develop questions by reading recent survey articles** — Annual Review of Financial Economics

### The Research Continuum

- **Safe end**: Stay close to conventions, incremental methods, established rules
- **Bold end**: Break from existing paradigm, require new methods
- First paper: safe end. Job market paper: bold end.

---

## Synthesis: The Editor's Decision Framework

Based on Edmans, the typical editorial workflow for evaluating a paper:

```
1. Read abstract → Is there one memorable, concrete finding?
2. Read introduction → Does it change my prior? Is the identification clear?
3. Skim tables → Is the economic magnitude meaningful?
4. Check bibliography → Is it primarily finance journals? (fit check)
5. Read referee reports → Weigh contribution vs. execution vs. exposition
```

**The key insight**: Editors typically decide by the end of the introduction. The rest of the paper either confirms or overturns that initial assessment.
