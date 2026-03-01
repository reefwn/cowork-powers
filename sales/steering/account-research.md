# Account Research

Get a complete picture of any company or person before outreach. Works standalone with web search, supercharged with enrichment and CRM data.

## Triggers

"research [company]", "look up [person]", "intel on [prospect]", "who is [name] at [company]", "tell me about [company]"

## How It Works

**Always (web search)**: Company overview, recent news, hiring signals, key people, product/service info.

**With enrichment tools**: Verified emails, phone, tech stack, org chart, funding details.

**With CRM**: Prior relationship, past opportunities, contacts, notes.

## Output Format

```markdown
# Research: [Company or Person Name]

## Quick Take
[2-3 sentences: Who they are, why they might need you, best angle for outreach]

## Company Profile
| Field | Value |
|-------|-------|
| Company | [Name] |
| Website | [URL] |
| Industry | [Industry] |
| Size | [Employee count] |
| Headquarters | [Location] |
| Founded | [Year] |
| Funding | [Stage + amount] |

### What They Do
[1-2 sentence description]

### Recent News
- [Headline] — [Date] — [Why it matters for outreach]

### Hiring Signals
- [X] open roles in [Department]
- Notable: [Relevant roles]

## Key People
### [Name] — [Title]
- Background: [Prior companies, education]
- Talking Points: [Personal/professional hooks]

## Tech Stack [If Enrichment Connected]
| Category | Tools |
|----------|-------|
| Cloud | [AWS, GCP, etc.] |
| CRM | [Salesforce, HubSpot, etc.] |

## Prior Relationship [If CRM Connected]
| Field | Detail |
|-------|--------|
| Status | [New / Prior prospect / Customer / Churned] |
| Last Contact | [Date and type] |
| Previous Opps | [Won/Lost and why] |

## Qualification Signals
- ✅ [Positive signal and evidence]
- ⚠️ [Concern and what to watch]
- ❓ [Unknown — ask in discovery]

## Recommended Approach
**Best Entry Point:** [Person and why]
**Opening Hook:** [What to lead with]
**Discovery Questions:** [3 key questions]
```

## Execution Flow

1. **Parse request**: Company research, person + company, role-based search, or domain lookup
2. **Web search (always)**: Company homepage, news, funding, careers, person LinkedIn, product info, customers
3. **Enrichment (if connected)**: Firmographics, org chart, verified contact info, tech stack, intent data
4. **CRM check (if connected)**: Account by domain, related contacts, opportunity history, activity timeline
5. **Synthesize**: Combine sources, prioritize enrichment over web, add CRM context, identify qualification signals, generate talking points

## Research Variations

- **Company Research**: Business overview, news, hiring, leadership
- **Person Research**: Background, role, LinkedIn activity, talking points
- **Competitor Research**: Product comparison, positioning, win/loss patterns
- **Pre-Meeting Research**: Attendee backgrounds, recent news, relationship history

## Tips

- Include the domain for precision ("research acme.com")
- Specify the person ("look up Jane Smith, VP Sales at Acme")
- State your goal ("research Stripe before my demo call")
