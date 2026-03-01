# Call Summary Workflow

Process call notes or a transcript — extract action items, draft follow-up email, generate internal summary.

## When to Use
When the user has call notes, a transcript, or wants to describe a call and needs structured output: internal summary, action items, and customer follow-up email.

## Input Options

- **Paste notes**: Bullet points, rough notes, stream of consciousness
- **Paste transcript**: Full transcript from video conferencing or conversation intelligence tool
- **Describe the call**: "Had a discovery call with Acme Corp. Met with their VP Eng and CTO..."

## Output

### Internal Summary

```markdown
## Call Summary: [Company] — [Date]
**Attendees:** [Names and titles]
**Call Type:** [Discovery / Demo / Negotiation / Check-in]

### Key Discussion Points
1. [Topic] — [What was discussed, decisions made]

### Customer Priorities
- [Priority they expressed]

### Objections / Concerns Raised
- [Concern] — [How addressed / status]

### Competitive Intel
- [Competitor mentions, what was said]

### Action Items
| Owner | Action | Due |
|-------|--------|-----|
| [You] | [Task] | [Date] |
| [Customer] | [Task] | [Date] |

### Next Steps
- [Agreed next step with timeline]

### Deal Impact
- [How this affects the opportunity]
```

### Customer Follow-Up Email

Plain text, no markdown formatting. Concise but informative. Structure: thank you → key points discussed → commitments made → clear next step with timeline.

## If Connectors Available

- **Transcripts (Gong, Fireflies)**: Search for and pull the call automatically
- **CRM**: Offer to update opportunity stage, log activity, create tasks
- **Email**: Offer to create draft or send directly

## Email Style Guidelines

- No markdown formatting — plain text only
- Short paragraphs, line breaks between sections
- Simple dashes or numbers for lists, not fancy formatting

## Tips

- More detail = better output. Even rough notes help.
- Name the attendees for better structure and action item assignment.
- Flag what matters: "The big thing was..."
- Tell me the deal stage for tailored follow-up tone.
