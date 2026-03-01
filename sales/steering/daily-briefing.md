# Daily Sales Briefing

Start your day with a prioritized sales briefing. Works standalone when you describe your meetings and priorities, supercharged with calendar, CRM, and email.

## Triggers

"morning briefing", "daily brief", "what's on my plate today", "prep my day", "start my day"

## How It Works

**Always (standalone)**: You tell me today's meetings, key deals, priorities. I organize into a prioritized action plan.

**With Calendar**: Auto-pull today's meetings with attendees.
**With CRM**: Pipeline alerts, tasks, deal health.
**With Email**: Unread from key accounts, waiting on replies.
**With Enrichment**: Overnight signals on your accounts.

## Output Format

```markdown
# Daily Briefing | [Day, Month Date]

## #1 Priority
**[Most important thing today]**
[Why it matters and what to do]

## Today's Numbers
| Open Pipeline | Closing This Month | Meetings Today | Action Items |
|---------------|-------------------|----------------|--------------|
| $[X] | $[X] | [N] | [N] |

## Today's Meetings
### [Time] — [Company] ([Meeting Type])
**Attendees:** [Names]
**Context:** [Deal status, last touch, what's at stake]
**Prep:** [Quick action before this meeting]

## Pipeline Alerts
### Needs Attention
| Deal | Stage | Amount | Alert | Action |
|------|-------|--------|-------|--------|

### Closing This Week
| Deal | Close Date | Amount | Confidence | Blocker |
|------|------------|--------|------------|---------|

## Email Priorities
### Needs Response
| From | Subject | Received |
|------|---------|----------|

### Waiting On Reply
| To | Subject | Sent | Days Waiting |
|----|---------|------|--------------|

## Suggested Actions
1. [Action] — [Why now]
2. [Action] — [Why now]
3. [Action] — [Why now]
```

## Priority Ranking

1. URGENT: Deal closing today/tomorrow not yet won
2. HIGH: Meeting today with high-value opportunity
3. HIGH: Unread email from decision-maker
4. MEDIUM: Deal closing this week
5. MEDIUM: Stale deal (7+ days no activity)
6. LOW: Tasks due this week

## Quick Mode

Say "quick brief" or "tldr my day":

```markdown
# Quick Brief | [Date]
**#1:** [Priority action]
**Meetings:** [N] — [Company 1], [Company 2]
**Alerts:** [Alert 1], [Alert 2]
**Do Now:** [Single most important action]
```

## End of Day Mode

Say "wrap up my day" or "end of day summary":

```markdown
# End of Day | [Date]
**Completed:** [Meeting outcomes]
**Pipeline Changes:** [Stage movements]
**Tomorrow's Focus:** [Top priorities]
**Open Loops:** [Unfinished items]
```
