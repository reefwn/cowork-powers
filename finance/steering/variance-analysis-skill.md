# Variance Analysis

Techniques for decomposing variances, materiality thresholds, narrative generation, waterfall chart methodology, and budget vs actual vs forecast comparisons.

> **Important**: All analyses should be reviewed by qualified financial professionals before use in reporting.

## Decomposition Techniques

### Price / Volume
```
Volume Effect = (Actual Volume - Budget Volume) × Budget Price
Price Effect  = (Actual Price - Budget Price) × Actual Volume
```

### Rate / Mix
Rate Effect: Change in unit economics at actual volumes
Mix Effect: Shift between segments with different unit economics

### Headcount / Compensation
Headcount variance + Rate variance + Mix variance + Timing variance + Attrition impact

### Spend Category (OpEx)
Headcount-driven → Volume-driven → Discretionary → Contractual/fixed → One-time → Timing/phasing

## Materiality Thresholds

| Comparison Type | Dollar Threshold | % Threshold |
|----------------|-----------------|-------------|
| Actual vs Budget | Org-specific | 10% |
| Actual vs Prior Period | Org-specific | 15% |
| Actual vs Forecast | Org-specific | 5% |
| Sequential (MoM) | Org-specific | 20% |

Set dollar thresholds at 0.5%-1% of revenue for income statement items.

### Investigation Priority
1. Largest absolute dollar variance
2. Largest percentage variance
3. Unexpected direction
4. New variance (was on track, now off)
5. Cumulative/trending variance

## Narrative Generation

### Structure
```
[Line Item]: [Favorable/Unfavorable] variance of $[amount] ([%]) vs [basis] for [period]
Driver: [Primary driver]
[2-3 sentences explaining business reason with quantification]
Outlook: [One-time / Expected to continue / Improving / Deteriorating]
Action: [None / Monitor / Investigate / Update forecast]
```

### Quality Checklist
- Specific (names actual driver)
- Quantified (dollar and percentage impact)
- Causal (explains WHY, not just WHAT)
- Forward-looking (will it continue?)
- Actionable (required follow-up)
- Concise (2-4 sentences)

### Anti-Patterns to Avoid
- Circular explanations ("Revenue was higher due to higher revenue")
- Vague descriptions ("Expenses were elevated")
- "Timing" without specifics
- "One-time" without explanation
- "Various small items" for material variances

## Waterfall Methodology

```
[Base]                    $XX,XXX
  |--[+] Driver 1        +$X,XXX
  |--[-] Driver 2        -$X,XXX
[Actual]                  $XX,XXX
```

Best practices: 5-8 drivers max, verify reconciliation, order by magnitude or business logic.

## Budget vs Actual vs Forecast

- **Actual vs Budget**: Annual performance measurement, board reporting
- **Actual vs Forecast**: Operational management, emerging issues
- **Forecast vs Budget**: Planning accuracy, expectation changes
- **Actual vs Prior Year**: YoY growth, seasonality-adjusted comparison

### Forecast Accuracy
```
Accuracy = 1 - |Actual - Forecast| / |Actual|
MAPE = Average of |Actual - Forecast| / |Actual| across periods
```
