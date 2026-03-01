# Sprint Planning Workflow

Plan a sprint by scoping work, estimating capacity, and setting clear goals.

## When to Use
When the user wants to plan a sprint — define goals, estimate capacity, scope backlog items, and produce a sprint plan.

## What I Need From You

- **Team**: Who's on the team and their availability this sprint?
- **Sprint length**: How many days/weeks?
- **Backlog**: What's prioritized? (Pull from tracker, paste, or describe)
- **Carryover**: Anything unfinished from last sprint?
- **Dependencies**: Anything blocked on other teams?

## Workflow

### 1. Gather Inputs

If project tracker is connected: pull backlog, create sprint, assign items.

If calendar is connected: account for PTO and meetings in capacity.

If chat is connected: share sprint plan with the team.

Otherwise, gather all inputs from the user directly.

### 2. Estimate Capacity

Account for PTO, on-call, meetings, and other overhead. Use the capacity planning guidance from the **roadmap-management** steering (60-70% of time on planned work).

### 3. Scope and Prioritize

Define one clear sprint goal. Prioritize backlog items as P0 (must ship), P1 (should ship), P2 (stretch). Ensure total load fits within capacity (target 70-80%).

### 4. Identify Risks and Dependencies

Flag cross-team dependencies, items with unclear scope, and anything that could block progress.

## Output

```markdown
## Sprint Plan: [Sprint Name]
**Dates:** [Start] — [End] | **Team:** [X] engineers
**Sprint Goal:** [One clear sentence about what success looks like]

### Capacity
| Person | Available Days | Allocation | Notes |
|--------|---------------|------------|-------|
| [Name] | [X] of [Y] | [X] points/hours | [PTO, on-call, etc.] |
| **Total** | **[X]** | **[X] points** | |

### Sprint Backlog
| Priority | Item | Estimate | Owner | Dependencies |
|----------|------|----------|-------|--------------|
| P0 | [Must ship] | [X] pts | [Person] | [None / Blocked by X] |
| P1 | [Should ship] | [X] pts | [Person] | [None] |
| P2 | [Stretch] | [X] pts | [Person] | [None] |

### Planned Capacity: [X] points | Sprint Load: [X] points ([X]% of capacity)

### Risks
| Risk | Impact | Mitigation |
|------|--------|------------|
| [Risk] | [What happens] | [What to do] |

### Definition of Done
- [ ] Code reviewed and merged
- [ ] Tests passing
- [ ] Documentation updated (if applicable)
- [ ] Product sign-off

### Key Dates
| Date | Event |
|------|-------|
| [Date] | Sprint start |
| [Date] | Mid-sprint check-in |
| [Date] | Sprint end / Demo |
| [Date] | Retro |
```

## Tips

1. **Leave buffer** — Plan to 70-80% capacity. You will get interrupts.
2. **One clear sprint goal** — If you can't state it in one sentence, the sprint is unfocused.
3. **Identify stretch items** — Know what to cut if things take longer.
4. **Carry over honestly** — If something didn't ship, understand why before re-committing.
