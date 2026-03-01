# /income-statement

Generate an income statement with period-over-period comparison and variance analysis. Highlight material variances for investigation.

> **Important**: This command assists with financial statement workflows but does not provide financial advice. All statements should be reviewed by qualified financial professionals before use in reporting or filings.

## Usage

```
/income-statement [period-type] [period]
```

### Arguments
- `period-type` — `monthly`, `quarterly`, `annual`, `ytd`
- `period` — The period to report (e.g., `2024-12`, `2024-Q4`, `2024`)

## Workflow

### 1. Gather Financial Data

If ~~erp or ~~data warehouse is connected:
- Pull trial balance or income statement data for the specified period
- Pull comparison period data (prior period, prior year, budget/forecast)
- Pull account hierarchy for presentation

If no data source: prompt user for current and comparison period data.

### 2. Generate Income Statement

Present in standard multi-column format with Current Period, Prior Period, Variance ($), Variance (%), Budget, and Budget Variance columns. Include:
- Revenue (by stream)
- Cost of Revenue
- Gross Profit and Gross Margin %
- Operating Expenses (R&D, S&M, G&A)
- Operating Income and Operating Margin %
- Other Income/Expense
- Income Before Taxes, Tax Expense
- Net Income and Net Margin %

### 3. Variance Analysis

Flag material variances using thresholds (dollar and percentage). For each flagged variance provide:
- Direction and magnitude
- Possible drivers
- Questions to investigate
- Favorable or unfavorable classification

### 4. Key Metrics Summary

```
Revenue growth (%), Gross margin (%), Operating margin (%),
Net margin (%), OpEx as % of revenue, Effective tax rate (%)
```

### 5. Material Variance Summary

| Line Item | Variance ($) | Variance (%) | Direction | Preliminary Driver | Action |
|-----------|-------------|-------------|-----------|-------------------|--------|

### 6. Output

1. Formatted income statement with comparisons
2. Key metrics summary
3. Material variance listing with investigation flags
4. Suggested follow-up questions for unexplained variances
5. Offer to drill into any specific variance with `/variance-analysis`
