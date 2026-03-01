# Create an Asset

Generate custom sales assets tailored to your prospect, audience, and goals. Supports interactive landing pages, presentation decks, executive one-pagers, and workflow/architecture demos.

## Triggers

"create an asset", "build a demo", "make a landing page", "mock up a workflow"

## Overview

Gathers context about (a) the prospect, (b) the audience, (c) the purpose, (d) the format — then researches, structures, and builds a polished, branded asset as a self-contained HTML file.

## Input Collection

### Seller Context (detected or asked once, persisted)
Company, product, value props, differentiators, pricing model.

### Prospect Context
- Company (required)
- Key contacts, deal stage, pain points, past materials (optional)

### Audience Context
- Audience type (required): Executive, Technical, Operations, Mixed
- Primary concern (required): ROI, Technical depth, Strategic alignment, Risk mitigation, Implementation
- Specific roles, objections (optional)

### Purpose Context
- Goal (required): Intro, Discovery follow-up, Technical deep-dive, Exec alignment, POC proposal, Deal close
- Desired action (required)

### Format Selection
| Format | Best For |
|--------|----------|
| Interactive landing page | Exec alignment, intros, value prop |
| Deck-style | Formal meetings, large audiences |
| One-pager | Leave-behinds, quick summaries |
| Workflow / Architecture demo | Technical deep-dives, POC demos, integrations |

## Research Phase

Assess context richness (Rich/Moderate/Sparse) and adjust research depth.

Always research: prospect basics (revenue, strategy), leadership, brand colors.
If moderate/sparse: also industry context, technology landscape, competitive context.
If transcripts uploaded: extract pain points, decision criteria, objections, key quotes.

## Structure by Format

### Interactive Landing Page
Sections vary by purpose: Strategic Fit → Solution → Use Cases → Why Us → Next Steps (intro), Their Priorities → How We Help → Examples → ROI → Next Steps (discovery follow-up), etc.

### Deck-Style
Title → Agenda → Content slides → Summary → Next Steps → Appendix. One key message per slide.

### One-Pager
Hero → 3 Key Points → Proof Point → CTA. Single-scroll format.

### Workflow Demo
Component nodes, flow arrows (animated), step panel, controls (Play/Pause/Step/Reset), annotations, data preview. Complexity determines layout (simple/medium/complex).

## Visual Design

Dark theme with prospect brand colors as accent. Cards with rounded corners, subtle borders, hover states. Self-contained HTML — all CSS/JS inline, no external dependencies.

## Clarifying Questions (Required Before Building)

1. Summarize understanding (format, audience, goal, key themes)
2. Standard questions: "Does this match?", "ONE thing this must nail?", tone preference, scope preference
3. Format-specific questions
4. Max 2 rounds of questions. If ambiguous, make reasonable choice and note it.

## Delivery

Self-contained HTML file named `[ProspectName]-[format]-[date].html`.

Deployment options: static hosting (Netlify, Vercel, GitHub Pages), password protection, direct share, embed via iframe.

## Quality Checklist

- Content: Names correct, pain points accurate, no placeholders, proof points sourced
- Visual: Brand colors applied, text readable, animations smooth, responsive
- Functional: All tabs/sections work, interactive elements functional, navigation intuitive
- Professional: Tone matches audience, appropriate detail level, no typos, feels tailored
