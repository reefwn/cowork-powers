# Metrics Review Workflow

Review and analyze product metrics, identify trends, and surface actionable insights.

## When to Use
When the user wants to review product metrics for a time period, analyze trends, or generate a metrics report with recommendations.

## Workflow

### 1. Gather Metrics Data

If product analytics is connected: pull key metrics for the relevant period, comparison data (previous period, same period last year, targets), and segment breakdowns.

If no analytics tool is connected, ask the user to provide: metrics and values (paste a table, screenshot, or describe), comparison data, context on recent changes.

Ask the user:
- What time period? (last week, month, quarter)
- What metrics to focus on? Or full product metrics suite?
- Specific targets or goals to compare against?
- Known events that might explain changes? (launches, outages, campaigns, seasonality)

### 2. Organize the Metrics

Structure using the metrics hierarchy from the **metrics-tracking** steering: North Star at top, L1 health indicators (acquisition, activation, engagement, retention, revenue, satisfaction), L2 diagnostic metrics for drill-down.

If the user hasn't defined their hierarchy, help identify North Star and key L1 metrics first.

### 3. Analyze Trends

For each key metric:
- **Current value**: What is it today?
- **Trend**: Up, down, or flat vs previous period?
- **vs Target**: How does it compare to the goal?
- **Rate of change**: Accelerating or decelerating?
- **Anomalies**: Sudden changes, spikes, or drops?

Identify correlations, leading indicators, and segment-driven aggregate trends.

### 4. Generate the Review

#### Summary
2-3 sentences: overall health, most notable changes, key callout.

#### Metric Scorecard

| Metric | Current | Previous | Change | Target | Status |
|--------|---------|----------|--------|--------|--------|
| [Metric] | [Value] | [Value] | [+/- %] | [Target] | [On track / At risk / Miss] |

#### Trend Analysis
For each notable metric: what happened, why (attribution), whether one-time or sustained.

#### Bright Spots
Metrics beating targets, positive trends, strong-performing segments or features.

#### Areas of Concern
Metrics missing targets, early warning signals, metrics lacking visibility.

#### Recommended Actions
Specific next steps: investigations, experiments, investments, alerts to set.

#### Context and Caveats
Data quality issues, events affecting comparability, metrics not yet tracked.

### 5. Follow Up

- Offer deeper investigation on any metric
- Offer dashboard spec for ongoing monitoring
- Offer experiment proposals for areas of concern
- Offer metrics review template for recurring use

## Output Format

Tables for the scorecard. Clear status indicators. Keep summary tight — essential story in 30 seconds.

## Tips

- Start with the "so what" — lead with the most important thing.
- Always show comparisons (vs previous period, vs target, vs benchmark).
- Be careful about attribution — correlation is not causation.
- Segment analysis often reveals that aggregate metrics mask important differences.
- Not all movements matter. Focus on meaningful changes.
- If a metric misses its target, recommend what to do about it.
- Metrics reviews should drive decisions. If no action results, it wasn't useful.
