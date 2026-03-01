# Competitive Intelligence

Research competitors and generate an interactive HTML battlecard for use in deals.

## Triggers

"competitive intel", "research competitors", "how do we compare to [competitor]", "battlecard for [competitor]"

## How It Works

**Always (web search)**: Competitor product deep-dive (features, pricing, positioning), recent releases (last 90 days), your company releases, differentiation matrix, sales talk tracks, landmine questions.

**Output**: Interactive HTML battlecard with comparison matrix overview, clickable tabs per competitor, dark theme professional styling, self-contained HTML file.

**With CRM**: Win/loss data, competitor mentions in closed deals.
**With Docs**: Existing battlecards, competitive playbooks.
**With Chat**: Internal intel, field reports from colleagues.
**With Transcripts**: Competitor mentions in customer calls.

## Getting Started

Required: Your company name, main competitors (1-5).
Optional: Specific competitor to focus on, deals where you're competing, customer pain points about competitors.

## HTML Battlecard Structure

### 1. Comparison Matrix (Landing View)
Feature comparison grid, pricing comparison, market positioning, win rate indicators (if CRM connected).

### 2. Competitor Tabs (Click to Expand)
Each competitor card shows: company profile, product positioning, recent releases, where they win vs where you win, pricing intelligence, talk tracks, objection handling, landmine questions.

### 3. Your Company Card
Your releases (last 90 days), key differentiators, proof points and customer quotes.

## Data Structure Per Competitor

```yaml
competitor:
  name: "[Name]"
  profile:
    founded, funding, employees, target_market, pricing_model, market_position
  what_they_sell: "[Product summary]"
  their_positioning: "[How they describe themselves]"
  recent_releases:
    - date, release, impact
  where_they_win:
    - area, advantage, how_to_handle
  where_you_win:
    - area, advantage, proof_point
  pricing:
    model, entry_price, enterprise, hidden_costs, talk_track
  talk_tracks:
    early_mention, displacement, late_addition
  objections:
    - objection, response
  landmines:
    - "[Question that exposes their weakness]"
```

## Execution Flow

1. **Gather seller context**: Company, product, competitors (persist for future sessions)
2. **Research your company**: Product, pricing, news, releases, comparisons
3. **Research each competitor**: Features, pricing, news, releases, reviews, customers, careers
4. **Pull connected sources**: CRM win/loss, docs, chat intel, transcript mentions
5. **Build HTML artifact**: Structure data, build matrix, generate battlecards, compile talk tracks, render self-contained HTML

## Refresh Cadence

| Trigger | Action |
|---------|--------|
| Monthly | Quick refresh — releases, news, pricing changes |
| Before major deal | Deep refresh for specific competitor |
| After win/loss | Update patterns with new data |
| Competitor announcement | Immediate update on that competitor |

## Tips

- Be honest about weaknesses — credibility comes from acknowledging competitor strengths
- Focus on outcomes, not features
- Best intel comes from actual customer conversations
- Plant landmines, don't badmouth — ask questions that expose weaknesses
- Track releases religiously — what they ship tells you their strategy
