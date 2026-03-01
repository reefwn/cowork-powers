# Call Prep

Get fully prepared for any sales call in minutes. Works with whatever context you provide, significantly better with connected tools.

## Triggers

"prep me for my call with [company]", "call prep [company]", "get me ready for [meeting]"

## How It Works

**Always (standalone)**: You provide company, meeting type, attendees. Web search for news, funding, leadership. Output: prep brief with agenda and questions.

**With CRM**: Account history, contacts, opportunities, activities.
**With Email**: Recent threads, open questions, commitments.
**With Chat**: Internal discussions, colleague insights.
**With Transcripts**: Prior call recordings, key moments.
**With Calendar**: Auto-find meeting, pull attendees.

## Output Format

```markdown
# Call Prep: [Company Name]
**Meeting:** [Type] — [Date/Time]
**Attendees:** [Names with titles]
**Your Goal:** [What you want to accomplish]

## Account Snapshot
| Field | Value |
|-------|-------|
| Company | [Name] |
| Industry | [Industry] |
| Size | [Employees / Revenue] |
| Status | [New prospect / Active opp / Customer] |
| Last Touch | [Date and summary] |

## Who You're Meeting
### [Name] — [Title]
- Background: [Career history]
- Role in Deal: [Decision maker / Champion / Evaluator]
- Talking Point: [Something to reference]

## Context & History
- [Key points from prior interactions]
- [Open commitments or action items]
- [Recent news about the company]

## Suggested Agenda
1. Open — [Reference last conversation or trigger event]
2. [Topic] — [Discovery question or value discussion]
3. [Topic] — [Address known concern]
4. Next Steps — [Propose clear follow-up]

## Discovery Questions
1. [Current situation]
2. [Pain points or priorities]
3. [Decision process and timeline]
4. [Success criteria]
5. [Other stakeholders]

## Potential Objections
| Objection | Suggested Response |
|-----------|-------------------|
| [Likely objection] | [How to address] |
```

## Execution Flow

1. **Gather context**: Calendar → CRM → Email → Chat → Transcripts (if connected), otherwise ask user
2. **Research supplement (always)**: Web search for company news, funding, leadership, attendee LinkedIn
3. **Synthesize**: Combine sources, identify gaps → discovery questions, anticipate objections, create agenda

## Meeting Type Variations

- **Discovery**: Focus on understanding their world. Questions > Talking. Output: qualification signals.
- **Demo**: Focus on their use case. Show relevant features. Output: technical requirements, timeline.
- **Negotiation**: Focus on addressing concerns. Handle objections. Output: path to agreement.
- **Check-in / QBR**: Focus on value delivered. Surface new needs. Output: renewal confidence, upsell pipeline.

## Tips

- More context = better prep. Paste emails, notes, anything.
- Name the attendees — even just titles help.
- State your goal — "I want to get them to agree to a pilot"
- Flag concerns — "They mentioned budget is tight"
