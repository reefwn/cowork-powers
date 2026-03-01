# Pipeline Review Workflow

Analyze pipeline health — prioritize deals, flag risks, get a weekly action plan.

## When to Use
When the user wants to review their pipeline, identify at-risk deals, get prioritized actions, or audit pipeline hygiene.

## Input Options

- **Upload CSV**: Pipeline export (deal name, account, amount, stage, close date, created date, last activity, owner, contact)
- **Paste deals**: "Acme Corp - $50K - Negotiation - closes Jan 31 - last activity Jan 20"
- **Describe pipeline**: "12 deals. Two big ones in negotiation. Three stuck in discovery for over a month."

## Output

```markdown
# Pipeline Review: [Date]
**Deals Analyzed:** [X] | **Total Pipeline Value:** $[X]

## Pipeline Health Score: [X/100]
| Dimension | Score | Issue |
|-----------|-------|-------|
| Stage Progression | [X]/25 | [X] deals stuck 30+ days |
| Activity Recency | [X]/25 | [X] deals no activity 14+ days |
| Close Date Accuracy | [X]/25 | [X] deals with past close date |
| Contact Coverage | [X]/25 | [X] deals single-threaded |

## Priority Actions This Week
### 1. [Highest Priority Deal]
**Why:** [Reason] | **Action:** [Next step] | **Impact:** $[X]

## Deal Prioritization Matrix
### Close This Week | Close This Month | Nurture

## Risk Flags
### Stale Deals (No Activity 14+ Days)
### Stuck Deals (Same Stage 30+ Days)
### Past Close Date
### Single-Threaded (Only One Contact)

## Hygiene Issues
| Issue | Count | Deals | Action |
(Missing close date, amount, next step, primary contact)

## Pipeline Shape
By Stage | By Close Month | By Deal Size

## Recommendations
### This Week: [3 specific actions]
### This Month: [Strategic actions]

## Deals to Consider Removing
| Deal | Amount | Reason | Recommendation |
```

## Prioritization Framework

| Factor | Weight | What to Look For |
|--------|--------|-----------------|
| Close Date | 30% | Deals closing soonest |
| Deal Size | 25% | Bigger deals = more focus |
| Stage | 20% | Later stage = more focus |
| Activity | 15% | Active deals prioritized |
| Risk | 10% | Lower risk = safer bet |

User can adjust: "Focus on big deals over soon deals" or "I need quick wins."

## With CRM Connected

Pull pipeline automatically, update records, create follow-up tasks, track hygiene improvements over time.

## Tips

- Review weekly — pipeline health decays fast
- Kill dead deals — stale opportunities inflate pipeline and distort forecasts
- Multi-thread everything — if one person goes dark, you need a backup
- Close dates should mean something — when you expect signature, not when you hope
