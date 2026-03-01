# Synthesize Research Workflow

Synthesize user research from multiple sources into structured insights and recommendations.

## When to Use
When the user has research data (interviews, surveys, usability tests, analytics, support tickets, sales call notes) and wants to extract themes, findings, and actionable recommendations.

## Workflow

### 1. Gather Research Inputs

Accept from any combination of:
- Pasted text (interview notes, transcripts, survey responses, feedback)
- Uploaded files (research documents, spreadsheets, recording summaries)
- Knowledge base (if connected): search for research documents, interview notes, survey results
- User feedback tool (if connected): pull support tickets, feature requests, bug reports
- Product analytics (if connected): pull usage data, funnel metrics, behavioral data
- Meeting transcription (if connected): pull interview recordings, meeting summaries

Ask the user:
- What type of research? (interviews, surveys, usability tests, analytics, support tickets, sales call notes)
- How many sources / participants?
- Specific question or hypothesis being investigated?
- What decisions will this inform?

### 2. Process the Research

For each source, extract:
- **Key observations**: What did users say, do, or experience?
- **Quotes**: Verbatim quotes illustrating important points
- **Behaviors**: What users actually did (vs what they said)
- **Pain points**: Frustrations, workarounds, unmet needs
- **Positive signals**: What works well, moments of delight
- **Context**: User segment, use case, experience level

### 3. Identify Themes and Patterns

Apply thematic analysis from the **user-research-synthesis** steering: affinity mapping, triangulation, theme development.

Group observations into themes, count frequency across participants, assess impact severity. Note contradictions and surprises.

Create a priority matrix:
- **High frequency + High impact**: Top priority
- **Low frequency + High impact**: Important for specific segments
- **High frequency + Low impact**: Quality-of-life improvements
- **Low frequency + Low impact**: Note but deprioritize

### 4. Generate the Synthesis

#### Research Overview
Methodology, research questions, timeframe.

#### Key Findings (5-8)
For each:
- **Finding statement**: One clear sentence
- **Evidence**: Supporting quotes, data points, observations (with source attribution)
- **Frequency**: How many participants/sources support this
- **Impact**: How significantly this affects user experience or business
- **Confidence level**: High (strong evidence), Medium (suggestive), Low (early signal)

Order by priority (frequency × impact).

#### User Segments / Personas
If research reveals distinct segments: name, characteristics, behaviors, unique needs, size estimate.

#### Opportunity Areas
Unmet or underserved needs, where current solutions fall short, new capabilities that would unlock value. Prioritized by potential impact.

#### Recommendations
Specific, actionable: what to build, change, or investigate further. Tied to specific findings. Prioritized by impact and feasibility.

#### Open Questions
Gaps in understanding, areas needing further investigation, suggested follow-up methods.

### 5. Review and Extend

- Ask if findings need more detail or different framing
- Offer to generate: persona documents, opportunity maps, research presentations
- Offer follow-up research plans for open questions
- Offer to draft product implications for the roadmap

## Output Format

Clear headers and structured formatting. Each finding should stand on its own.

## Tips

- Let the data speak. Don't force findings into a predetermined narrative.
- Distinguish what users say from what they do. Behavioral data is stronger.
- Quotes are powerful evidence. Include generously, attributed to participant type (not name).
- Be explicit about confidence levels.
- Contradictions are interesting, not inconvenient — they often reveal segments.
- Recommendations should be specific enough to act on.
- 5-8 strong findings are better than 20 weak ones.
