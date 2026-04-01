---
name: benchmark-idea
description: Evaluate a research idea against top journal standards using the 7-dimension rubric
args:
  - name: idea
    description: Research idea description or file path (optional, will ask interactively)
    required: false
  - name: venue
    description: Target venue (e.g., JF, JFE, RFS, JFQA, JCF, RF)
    required: false
tags: [Research, Evaluation, Finance, Top Journal]
---

# /benchmark-idea - Research Idea Benchmark

Evaluate a research idea against empirical standards distilled from 50+ top finance journal papers.

## Usage

```bash
/benchmark-idea
```

Interactive mode — asks for research idea and target venue.

```bash
/benchmark-idea "idea description or file path"
```

Evaluate a specific research idea.

```bash
/benchmark-idea "idea description" JFQA
```

Evaluate against a specific target venue's standards.

## Workflow

This command activates the `research-idea-benchmark` skill and executes the following steps:

### Step 1: Gather Research Idea
- Accept idea as argument, file path, or interactive input
- Extract: research question, proposed method, target venue, data availability
- Ask targeted follow-up questions if key elements are missing

### Step 2: Score Across 7 Dimensions
Using the rubric from `research-idea-benchmark` skill:

| Dimension | Weight |
|-----------|--------|
| Research Question Quality | 20% |
| Theoretical Foundation | 15% |
| **Identification Strategy** | **25%** |
| Data & Variable Construction | 15% |
| Robustness Architecture | 10% |
| Contribution Clarity | 10% |
| Narrative Quality | 5% |

### Step 3: Generate Evaluation Report

Output a structured report:

```markdown
## Research Idea Benchmark Report

### Overview
[Summary of the research idea]

### Target Venue Assessment
[Venue] | Estimated fit: [Strong/Moderate/Weak]

### Dimension Scores
| Dimension | Score | Key Strength | Key Weakness |
|-----------|-------|-------------|-------------|
| ... | X.X/5 | ... | ... |

**Weighted Total: X.XX / 5.00**

### Referee Red Flags
[Items from the rejection taxonomy that apply]

### Actionable Improvements
[Ranked list of concrete steps to strengthen weakest dimensions]

### Comparable Published Papers
[2-3 similar papers that succeeded, with notes on what worked]
```

### Step 4: Provide Targeted Guidance
- For each dimension scoring below 4.0, provide specific improvement strategies
- Reference editor rejection patterns (Edmans' 6 deadly sins)
- Suggest identification strategies from the arsenal of 9 methods
- Flag p-hacking risks (Mitton's methodological variation concerns)

## Output Files

```
benchmark-output/
└── benchmark-report.md    # Complete evaluation report
```

## Examples

### Example 1: Quick evaluation

```bash
/benchmark-idea "Does AI adoption in SOEs affect labor investment efficiency?"
```

### Example 2: With target venue

```bash
/benchmark-idea "Effect of climate policy uncertainty on green bond pricing" JCF
```

### Example 3: From file

```bash
/benchmark-idea research-proposal.md JFQA
```

## Integration

- **Skill**: `research-idea-benchmark` — provides the evaluation rubric and patterns
- **Upstream**: Use after `/research-init` or brainstorming to filter candidate ideas
- **Downstream**: Strong ideas proceed to `/plan` for implementation planning

## Related Commands

- `/research-init` — Start research ideation workflow (generates ideas)
- `/plan` — Create implementation plan (after idea is validated)
- `/analyze-results` — Analyze experimental results (after execution)
