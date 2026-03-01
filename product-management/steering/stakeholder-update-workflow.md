# Stakeholder Update Workflow

Generate a stakeholder update tailored to the audience and cadence.

## When to Use
When the user needs to write a status update, progress report, launch announcement, or any stakeholder communication.

## Workflow

### 1. Determine Update Type

- **Weekly**: Regular cadence — progress, blockers, next steps
- **Monthly**: Higher-level — trends, milestones, strategic alignment
- **Launch**: Feature or product launch — details and impact
- **Ad-hoc**: One-off for a specific situation (escalation, pivot, major decision)

### 2. Determine Audience

- **Executives / leadership**: High-level, outcome-focused, strategic, brief
- **Engineering team**: Technical detail, implementation context, blockers, decisions needed
- **Cross-functional partners**: Context-appropriate, shared goals and dependencies
- **Customers / external**: Benefits-focused, clear timelines, no internal jargon
- **Board**: Metrics-driven, strategic, risk-focused, very concise

### 3. Pull Context from Connected Tools

If project tracker is connected: pull roadmap item statuses, completed items, at-risk/blocked items, sprint progress.

If chat is connected: search for team discussions, decisions, blockers raised in channels.

If meeting transcription is connected: pull recent meeting notes, decisions, action items.

If knowledge base is connected: search for meeting notes, decision documents, design reviews.

If no tools connected: ask the user for accomplishments, blockers/risks, key decisions, and what's coming next.

### 4. Generate the Update

Structure for the target audience using templates from the **stakeholder-comms** steering:

**For executives**: TL;DR, G/Y/R status, progress tied to goals, risks with mitigation, specific asks, next milestones. Under 300 words.

**For engineering**: What shipped (with links), in progress (with owners), blockers, decisions needed (with options and recommendation), what's next.

**For cross-functional partners**: What's coming that affects them, what you need from them (with deadlines), decisions impacting their team, areas open for input.

**For customers**: What's new (framed as benefits), coming soon, known issues with workarounds, feedback channels. No internal jargon.

**For launch announcements**: What launched, why it matters, key details (scope, availability, limitations), success metrics, rollout plan, feedback channels.

### 5. Review and Deliver

- Ask if user wants to adjust tone, detail level, or emphasis
- Offer to format for delivery channel (email, chat post, doc, slides)
- If chat is connected, offer to draft the message for sending

## Output Format

Scannable. Bold for key points, bullets for lists. Executive updates under 300 words. Engineering updates structured for skimming.

## Tips

- Don't bury the lead. Start with the most important thing.
- G/Y/R status should reflect reality, not optimism. Yellow is good risk communication.
- Asks should be specific and actionable.
- For executives, frame in terms of outcomes and goals, not activities.
- If there's bad news, lead with it.
- Match length to audience attention.
