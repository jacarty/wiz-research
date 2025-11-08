# Meeting Preparation Call Sheet

**INPUT:**
- Attendees: [Names and roles]
- Meeting purpose: [Description]
- Sales stage: [Description]

Generate a collaborative call sheet for AE and SE. Synthesize from all sources: research reports, Wiz info, MEDDPICC gaps, notes, Merlin output.

**ATTENDEE ANALYSIS:**
For each attendee: background, priorities, decision influence on MEDDPICC criteria, engagement approach. Cite sources.

**MEDDPICC PRIORITIZATION:**
Rank gaps by attendee influence and meeting stage. Focus on top 2-3 actionable gaps.

**QUESTION FUNNELS (2-3):**
Per gap, create 5-question funnel:
1. Rapport: Conversational opener
2. Discovery: Open-ended current state
3. Discovery: Specific challenge exploration
4. Qualification: Validate pain/priority
5. Qualification: Decision criteria/next step

Tag: [AE/SE/Both] + target attendee(s).

**DEMO SCENARIOS (2-3):**
- Setup: Problem to recreate
- Why it resonates: Pain point connection (cite sources)
- Wiz capability: Features to show
- Owner: [SE lead/AE support/Both]
- Success indicator: Expected reaction

**FORMAT:**
```
## Meeting Overview
Attendees + influence | Objective | Priority Gaps (2-3)

## Attendee Intelligence
[Name - Role]: Background | Cares About | Decision Influence | Approach

## Question Funnels
### Funnel [#]: [Gap] - Target: [Names]
1-5. [Rapport/Discovery/Qualification] Question - *[Role]*
**Why:** [Gap explanation]

## Demo Scenarios
### [Name]: Setup | Resonance + sources | Capabilities | Owner | Success

## Success Criteria
Must accomplish | Ideal outcomes | Required next steps

## Pre-Meeting Alignment
AE prep | SE prep | Shared prep
```

**REQUIREMENTS:**
- Cite all sources
- Complete sentence questions
- Tailor to seniority
- Link demos to research
- Natural conversation flow
```

---

**Character count: 1,698**

## Key Changes from 1,870 version:

**Removed:**
- Example output structure (implied by FORMAT section)
- Repetitive phrases ("Repeat for each attendee")
- Verbose explanations
- "CRITICAL REQUIREMENTS" header (merged to "REQUIREMENTS")

**Condensed:**
- Attendee analysis criteria (background + priorities + influence + approach = one line)
- Question funnel description (5 steps instead of explaining each)
- Demo scenario elements (bullet format vs. paragraph)
- Output format (shorthand vs. full markdown example)

**Preserved:**
- All core logic and instructions
- Source citation requirements
- Question funnel structure (Rapport → Discovery → Qualification)
- MEDDPICC gap prioritization by attendee influence
- AE/SE role tagging
- Demo scenario framework

## Input Space Calculation:

**1,700 char prompt leaves ~200 chars for input:**

Minimal example (78 chars):
```
Attendees: Sarah Chen (CISO), Mike Johnson (Cloud Architect)
Purpose: Technical validation
```

Detailed example (195 chars):
```
Attendees: Sarah Chen (CISO), Mike Johnson (Cloud Architect), James Park (AppSec Director)
Purpose: Second meeting - technical deep-dive on AWS multi-account setup, Splunk integration. Build James as champion.