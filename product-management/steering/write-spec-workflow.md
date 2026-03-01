# Write Spec Workflow

Write a feature specification or product requirements document (PRD).

## When to Use
When the user wants to spec a new feature, write a PRD, or document product requirements from a problem statement or feature idea.

## Workflow

### 1. Understand the Feature

Accept any starting point:
- A feature name ("SSO support")
- A problem statement ("Enterprise customers keep asking for centralized auth")
- A user request ("Users want to export their data as CSV")
- A vague idea ("We should do something about onboarding drop-off")

### 2. Gather Context

Ask conversationally (don't dump all questions at once):
- **User problem**: What problem does this solve? Who experiences it?
- **Target users**: Which user segment(s)?
- **Success metrics**: How will we know this worked?
- **Constraints**: Technical, timeline, regulatory, dependencies
- **Prior art**: Attempted before? Existing solutions?

### 3. Pull Context from Connected Tools

If project tracker is connected: search for related tickets, epics, existing requirements, dependencies.

If knowledge base is connected: search for related research, prior specs, design docs, user research findings, meeting notes.

If design tool is connected: pull related mockups, wireframes, design system components.

If tools are not connected, work from what the user provides. Do not ask the user to connect tools.

### 4. Generate the PRD

Produce a structured PRD following the **feature-spec** steering guidance:

- **Problem Statement**: User problem, who is affected, impact of not solving it (2-3 sentences)
- **Goals**: 3-5 specific, measurable outcomes tied to user or business metrics
- **Non-Goals**: 3-5 things explicitly out of scope with rationale
- **User Stories**: Standard format grouped by persona
- **Requirements**: Must-Have (P0), Nice-to-Have (P1), Future Considerations (P2) with acceptance criteria
- **Success Metrics**: Leading and lagging indicators with specific targets
- **Open Questions**: Tagged with who needs to answer
- **Timeline Considerations**: Hard deadlines, dependencies, phasing

### 5. Review and Iterate

After generating:
- Ask if any sections need adjustment
- Offer to expand specific sections
- Offer to create follow-up artifacts (design brief, engineering ticket breakdown, stakeholder pitch)

## Output Format

Markdown with clear headers. Keep scannable — busy stakeholders should get the gist from headers and bold text alone.

## Tips

- Be opinionated about scope. Tight and well-defined beats expansive and vague.
- If the idea is too big, suggest breaking into phases and spec the first phase.
- Success metrics should be specific and measurable, not vague.
- Non-goals are as important as goals.
- Open questions should be genuinely open.
