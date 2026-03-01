# Forecast Workflow

Generate a weighted sales forecast with best/likely/worst scenarios, commit vs upside breakdown, and gap analysis.

## When to Use
When the user wants to forecast revenue for a period, analyze pipeline coverage, or prepare for a forecast call.

## Input Options

- **Upload CSV**: Pipeline export from CRM (minimum: deal name, amount, stage, close date)
- **Paste deals**: "Acme Corp - $50K - Negotiation - closes Jan 31"
- **Describe territory**: "8 deals totaling $400K. Two in negotiation ($120K)..."

Also need: quota, timeline (period end date), amount already closed.

## Output

```markdown
# Sales Forecast: [Period]

## Summary
| Metric | Value |
|--------|-------|
| Quota | $[X] |
| Closed to Date | $[X] ([X]% of quota) |
| Open Pipeline | $[X] |
| Weighted Forecast | $[X] |
| Gap to Quota | $[X] |
| Coverage Ratio | [X]x |

## Forecast Scenarios
| Scenario | Amount | % of Quota | Assumptions |
|----------|--------|------------|-------------|
| Best Case | $[X] | [X]% | All deals close as expected |
| Likely Case | $[X] | [X]% | Stage-weighted probabilities |
| Worst Case | $[X] | [X]% | Only commit deals close |

## Pipeline by Stage
| Stage | # Deals | Total Value | Probability | Weighted Value |
|-------|---------|-------------|-------------|----------------|

## Commit vs. Upside
### Commit (High Confidence)
| Deal | Amount | Stage | Close Date | Why Commit |
### Upside (Lower Confidence)
| Deal | Amount | Stage | Close Date | Risk Factor |

## Risk Flags
| Deal | Amount | Risk | Recommendation |
(Close date passed, no activity 14+ days, close date this week still in discovery)

## Gap Analysis
**To hit quota, you need:** $[X] more
Options: accelerate deals, revive stalled deals, new pipeline needed.

## Recommendations
1. [Specific action for highest-impact deal]
2. [Action for at-risk deal]
3. [Pipeline generation if gap exists]
```

## Default Stage Probabilities

| Stage | Probability |
|-------|-------------|
| Closed Won | 100% |
| Negotiation / Contract | 80% |
| Proposal / Quote | 60% |
| Evaluation / Demo | 40% |
| Discovery / Qualification | 20% |
| Prospecting / Lead | 10% |

User can provide custom probabilities.

## With CRM Connected

Pull pipeline automatically, use historical win rates, factor in activity recency for risk scoring, track forecast changes over time.

## Tips

- Be honest about commit — only deals you'd bet on
- Update close dates — stale dates kill forecast accuracy
- 3x pipeline coverage is healthy, below 2x is risky
- Activity = signal — no recent activity means higher risk than stage suggests
