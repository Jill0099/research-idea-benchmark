# Patterns Extracted from Top Finance Journal Papers

This reference documents recurring structural and methodological patterns observed across papers from JFQA, JCF, Review of Finance, and leading ESG/sustainability venues.

---

## Pattern 1: The "Black Box Opening" Research Design

**Frequency**: Very common in JFQA and JCF

**Structure**: An established relationship exists (X → Y), but the mechanism is unknown. The paper identifies and tests the specific channel.

**Examples**:
- Manager characteristics → corporate policies: what specific characteristic? Political ideology (Hutton et al., 2014)
- Pay restriction → firm behavior: through what channel? Pay-size elasticity weakening (Lan & Pan, 2026)
- Corruption → economic harm: through what? Innovation reduction (Ellis et al., 2020)

**Template**:
1. Establish that X affects Y (baseline)
2. Propose a specific mechanism M
3. Show X → M → Y (mediation)
4. Show that blocking M attenuates X → Y

---

## Pattern 2: The "Resolution Paper"

**Frequency**: High in review/framework papers

**Structure**: Existing literature has contradictory findings. The paper introduces a new dimension that resolves the contradiction.

**Examples**:
- ESG → firm value: contradictory results → introduce "materiality" distinction (Khan et al.)
- CSR motivation: pecuniary vs. non-pecuniary → systematic "seven tests" framework (Hong & Shore, 2023)

**Template**:
1. Document the contradiction in existing literature
2. Argue that a missing dimension explains the divergence
3. Introduce the dimension and re-test
4. Show that the contradiction disappears

---

## Pattern 3: The "Policy Shock" Empirical Design

**Frequency**: Dominant in JCF China-related papers

**Structure**: A government policy creates exogenous variation → DiD design comparing treated vs. untreated firms.

**Examples**:
- China 2014 SOE pay restriction: SOEs (treated) vs. non-SOEs (control) (Lan & Pan, 2026; Cao et al., 2026)
- Employment protection legislation across countries (Ji et al., 2026)

**Key Requirements**:
1. Policy must be plausibly exogenous to firm-level outcomes
2. Parallel trends must hold pre-treatment
3. No contaminating concurrent policies (or must be controlled for)
4. Treatment intensity variation adds power (e.g., more affected SOEs vs. less affected)

---

## Pattern 4: The "Unintended Consequences" Framing

**Frequency**: Common, especially for policy evaluation papers

**Structure**: A policy designed for purpose A has an unexpected effect B. The paper documents and explains this spillover.

**Examples**:
- Pay restriction intended to reduce inequality → reduces M&A activity (Lan & Pan, 2026)
- Pay restriction intended to curb excess → improves labor investment efficiency (Cao et al., 2026)

**Why Editors Love This**:
- Inherently surprising → high novelty
- Policy-relevant → broad readership
- Natural identification → the policy itself provides the shock

---

## Pattern 5: The "Proxy Innovation" Contribution

**Frequency**: A hallmark of highly cited papers

**Structure**: The paper's key methodological contribution is a novel way to measure a previously unmeasurable concept.

**Examples**:
- Political ideology measured via FEC donation records (Hutton et al., 2014)
- ESG materiality measured via SASB-KLD hand-mapping (Khan et al.)
- Growth incentive measured via pay-size elasticity (Lan & Pan, 2026)

**Validation Requirements**:
1. Correlate proxy with direct measures where available
2. Show proxy captures the intended construct (construct validity)
3. Show proxy does NOT capture confounding constructs (discriminant validity)
4. Demonstrate robustness to alternative proxy definitions

---

## Pattern 6: The "Cross-Country Institutional Variation" Design

**Frequency**: Growing, especially in JCF and Review of Finance

**Structure**: Exploit cross-country differences in institutions (laws, regulations, culture) as sources of variation.

**Examples**:
- Employment protection legislation stringency across countries (Ji et al., 2026)
- Legal origin and investor protection (many papers)

**Strengths**: Large variation in institutional features
**Weaknesses**: Harder to establish causality; many confounders

---

## Pattern 7: The "Mechanism Decomposition"

**Frequency**: Expected in all top-journal papers

**Structure**: After establishing the main effect, decompose it into sub-channels and test each.

**Examples**:
- Lan & Pan (2026): Pay restriction → M&A decline, decomposed into:
  - Direct pay channel
  - Perk channel
  - Pay-size elasticity (growth incentive) channel
  
- Cao et al. (2026): Pay restriction → labor efficiency, decomposed into:
  - Internal governance strengthening
  - Social comparison mitigation

**Template**:
1. Establish main effect: X → Y
2. Identify 2-3 potential channels: M1, M2, M3
3. Test each: X → Mi and Mi → Y
4. Show which channel dominates

---

## Common Data Sources in Top Finance Papers

| Database | Content | Use |
|----------|---------|-----|
| Compustat | Financial statements | Firm fundamentals, accounting variables |
| CRSP | Stock prices, returns | Return volatility, abnormal returns |
| ExecuComp | Executive compensation | CEO pay, incentive structure |
| FEC | Political donations | Political ideology proxy |
| MSCI KLD | ESG ratings | Sustainability performance |
| Thomson Reuters SDC | M&A transactions | Deal characteristics |
| IBES | Analyst forecasts | Earnings expectations |
| BoardEx | Board composition | Director characteristics |
| SASB | Materiality standards | Industry-specific ESG materiality |

---

## The "Contribution Statement" Formula

Top papers follow a remarkably consistent pattern when stating contributions:

### Formula
> "To our knowledge, this is the **first study** that [specific action] and shows that [specific finding]. Our study contributes to [Literature Stream 1] by [how], and to [Literature Stream 2] by [how]."

### Real Examples
- "To our knowledge, this is the first study that directly measures political preferences of a large, comprehensive sample of corporate managers and shows that political preferences help explain leverage choices and investment policies." (Hutton et al., 2014)

### Contribution Categories to Hit
1. **Empirical contribution**: New finding or fact
2. **Methodological contribution**: New variable, dataset, or technique
3. **Theoretical contribution**: New mechanism or framework
4. **Policy contribution**: Implications for regulation or practice

Top papers typically claim 2-3 of these four categories.

---

## Abstract Structure Template (from Top Papers)

1. **Context** (1 sentence): Set the scene
2. **Gap/Question** (1 sentence): What we don't know
3. **Method** (1-2 sentences): How we investigate
4. **Key findings** (2-3 sentences): What we find
5. **Implication** (1 sentence): Why it matters

**Total**: ~150-200 words for most finance journals

---

## Section-by-Section Length Benchmarks

Based on typical 30-40 page empirical papers:

| Section | Pages | % of Paper |
|---------|-------|-----------|
| Introduction | 4-6 | 12-15% |
| Literature / Theory | 3-5 | 8-12% |
| Data & Variables | 4-6 | 10-15% |
| Methodology | 2-4 | 5-10% |
| Main Results | 6-8 | 15-20% |
| Mechanism / Channels | 4-6 | 10-15% |
| Robustness | 4-6 | 10-15% |
| Conclusion | 1-2 | 3-5% |
| Tables & Figures | 8-12 | 20-30% |

---

## The "Limitation to Opportunity" Bridge

Top papers convert their limitations into future research directions in a specific pattern:

1. **Acknowledge honestly**: "Our study has several limitations..."
2. **Convert to opportunity**: "These limitations suggest fruitful avenues for future research..."
3. **Be specific**: Name exact follow-up studies, not vague gestures

### Common Limitation-to-Opportunity Pairs
- "Our sample is US-only" → "Cross-country comparison in different institutional settings"
- "We use a proxy variable" → "Future work with direct measures when data becomes available"
- "We document correlation" → "Future natural experiments for causal identification"
- "Two-period model" → "Dynamic multi-period extension"
