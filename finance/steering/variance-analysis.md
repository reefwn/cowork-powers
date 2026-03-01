# /variance-analysis

Decompose variances into underlying drivers, provide narrative explanations for significant variances, and generate waterfall analysis.

> **Important**: This command assists with variance analysis workflows but does not provide financial advice. All analyses should be reviewed by qualified financial professionals before use in reporting.

## Usage

```
/variance-analysis [area] [period-comparison]
```

### Arguments
- `area` — `revenue`, `opex`, `capex`, `headcount`, `cogs`/`cost-of-revenue`, `gross-margin`, or any specific GL account/group
- `period-comparison` — e.g., `2024-12 vs 2024-11`, `2024-Q4 vs budget`, `2024-12 vs 2023-12`

## Workflow

### 1. Gather Data

If ~~erp or ~~data warehouse is connected:
- Pull actuals for both comparison periods at detail level
- Pull budget/forecast data if comparing to plan
- Pull supporting operational metrics

If no data source: prompt user for actual data, comparison data, and operational metrics.

### 2. Calculate Top-Level Variance

```
VARIANCE SUMMARY: [Area] — [Period 1] vs [Period 2]
                  Period 1    Period 2    Variance ($)    Variance (%)
Total [Area]      $XX,XXX     $XX,XXX     $X,XXX          X.X%
```

### 3. Decompose Variance by Driver

Use the appropriate decomposition method:
- **Revenue**: Volume effect, Price/rate effect, Mix effect, New vs existing, Currency effect
- **OpEx**: Headcount-driven, Compensation changes, Volume-driven, New programs, One-time items, Timing
- **CapEx**: Project-level, Timing, Scope changes, Cost overruns
- **Headcount**: Hiring pace, Attrition, Compensation mix, Contractor/temp

### 4. Waterfall Analysis

```
WATERFALL: [Area] — [Period 1] vs [Period 2]

[Period 2 Base]                              $XX,XXX
  |
  |--[+] [Driver 1 description]             +$X,XXX
  |--[+] [Driver 2 description]             +$X,XXX
  |--[-] [Driver 3 description]             -$X,XXX
  |
[Period 1 Actual]                            $XX,XXX

Variance Reconciliation:
  Driver 1:  +$X,XXX  (XX% of total variance)
  Driver 2:  +$X,XXX  (XX% of total variance)
  Driver 3:  -$X,XXX  (XX% of total variance)
  Unexplained: $X,XXX (XX% of total variance)
  Total:     $X,XXX   (100%)
```

### 5. Narrative Explanations

For each significant driver:
> **[Driver name]** — [Favorable/Unfavorable] variance of $X,XXX (X.X%)
> [2-3 sentence explanation with specific operational factors and quantification]
> *Outlook:* [Whether expected to continue, reverse, or change]

### 6. Identify Unexplained Variances

Flag residual with possible causes to investigate. Ask user for additional context.

### 7. Output

1. Top-level variance summary
2. Detailed variance decomposition by driver
3. Waterfall analysis
4. Narrative explanations for each significant driver
5. Unexplained variance flag with investigation suggestions
6. Trend context and suggested actions
