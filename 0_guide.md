# Sales Research & Enablement Workflow
## Complete Guide: 13-Step Process

---

## Overview

This workflow transforms prospect research into actionable sales materials using a combination of AI tools:
- **Manual Input** → **Gemini** (Research & Synthesis) → **Merlin** (Wiz Alignment) → **NotebookLM** (Sales Outputs)

Each step builds on previous work to create comprehensive, personalized sales enablement materials.

---

## Step 1: Base Data

### What It Does
Establishes the foundation by collecting all available prospect information into NotebookLM.

### What to Upload
- **Documents:** Meeting notes, emails, call recordings, CRM exports, account plans
- **URLs:** Company website, LinkedIn (company + key executives), news articles, tech blog, GitHub/GitLab
- **Key Data Points:** Industry, location, employee count, cloud platforms, security tools, compliance requirements, known incidents, meeting participants

### Pro Tips
- Use native formats (PDF, DOCX) when possible
- Descriptive filenames help with citations
- Update progressively as you learn more
- Skip unverified rumors and outdated data (3+ years old)

### Example
```
Upload to NotebookLM:
- Prospect website: https://company.com
- LinkedIn: https://linkedin.com/company/prospect-name
- Recent funding announcement article
- Their Q3 earnings report PDF
- Notes from last meeting with CTO
- Companies House filing
```

---

## Step 2: Industry Intelligence Report

### What It Does
Generates comprehensive industry intelligence reports with market dynamics, technology trends, and regulatory context.

### Key Outputs
- Industry overview and growth projections
- Revenue drivers and strategic opportunities
- Challenges, risks, competitive landscape
- Regulatory requirements
- Deep-dive on technology innovation (cloud, SaaS, AI)
- Curated, verified sources

### Prompt Example
```
Create an executive-level Industry Strategy Map for UK Financial Services - Focus on wealth management and digital banking transformation.

[Include full prompt from your library]
```

### Follow-Up Requests
- "Add more case studies to the technology section"
- "Create a one-page executive summary"
- "Generate discovery questions based on the challenges"

---

## Step 3: Prospect Business Report

### What It Does
Conducts comprehensive business intelligence research on UK-headquartered companies with **verification-first methodology** - only includes sourced information.

### Key Outputs
- Company foundation and financial profile
- Business strategy and current priorities
- Market position and competitive landscape
- Regulatory and compliance context
- Leadership team and organizational structure
- Business challenges and pain points
- Partnership ecosystem
- **Explicit information gaps** (what to ask in discovery)

### Prompt Example
```
Conduct UK Customer Business Intelligence Research on:

Company: [Company Name]
Industry/Sector: [If known, otherwise will be identified]
Website: [Company website URL]
LinkedIn: [LinkedIn Company Page URL if known]
Companies House Number: [Registration number if known]

[Include full prompt from your library]
```

### Verification Standards
Every finding requires: **Evidence + Source URL + Date + Why It Matters**

Acceptable evidence:
- Official company sources
- Public records (Companies House, ICO, FCA)
- Credible news with attribution
- Job posting patterns (3+ postings)

### Follow-Up Requests
- "Expand the CISO profile with more background detail"
- "Research their customer segments in detail"
- "Update with developments from the past 3 months"

---

## Step 4: Prospect Technology Report

### What It Does
Identifies and verifies technology stack through systematic research. **Source-backed intelligence only** - explicitly documents gaps.

### Key Outputs
- Cloud infrastructure (providers, orchestration, CDN)
- Programming languages (backend, frontend, mobile)
- Business applications (CRM, ERP, collaboration, analytics)
- Security tools (CSPM, SAST, SIEM, secrets management)
- DevOps & CI/CD (GitHub/GitLab, Terraform, monitoring)
- **Knowledge gaps** (what wasn't found)

### Prompt Example
```
Conduct Tech Stack Discovery & Verification for:

Company: [Company Name]
Industry/Sector: [If known, otherwise will be identified]
Website: [Company website URL]
LinkedIn: [LinkedIn Company Page URL if known]

[Include full prompt from your library]
```

### Output Format
Each technology entry includes:

| Technology | Evidence | Source | Date | Confidence |
|------------|----------|---------|------|------------|
| AWS | 12 job postings + blog post | [URLs] | Nov 2025 | High |

### Follow-Up Requests
- "Deep dive on security tooling - check vendor case studies"
- "Research their monitoring/observability stack"
- "Create discovery questions based on knowledge gaps"

---

## Step 5: GTM Intelligence Brief Synthesis

### What It Does
Synthesizes all three research reports (Industry, Business, Technology) into a single brief for Merlin input (under 10,000 characters).

### How to Use
**Paste into Gemini in this order:**
1. Synthesis prompt
2. Industry Strategy Map Report
3. Company Business Intelligence Report
4. Tech Stack Discovery Report

### Prompt Example
```
[Paste synthesis prompt from library]

Link files from GDrive

--- INDUSTRY STRATEGY MAP ---
[Full industry report]

--- COMPANY BUSINESS INTELLIGENCE ---
[Full business report]

--- TECH STACK DISCOVERY ---
[Full tech report]
```

### Output
A formatted GTM Intelligence Brief ready for Step 6 (Merlin).

---

## Step 6: Wiz Alignment (Merlin Slackbot)

### What It Does
Analyzes prospect intelligence and generates ranked Wiz use-case recommendations aligned to business priorities.

### How to Use in Slack
1. Open Merlin in Slack
2. Paste the GTM Intelligence Brief from Step 5
3. Add the Merlin prompt
4. Send message

### Prompt Example
```
# Wiz GTM Use-Case Alignment

[Full Merlin prompt from library]

---

## PROSPECT INTELLIGENCE REPORT

[Paste the synthesized GTM Intelligence Brief from Step 5]
```

### Key Outputs
- Top 5 priority use-cases ranked by strategic fit
- Additional aligned use-cases
- Technology-specific recommendations
- Competitive displacement analysis
- **This output goes into NotebookLM for Steps 7-13**

---

## Step 7: Strategic Value Pyramid

### What It Does
Creates an executive-ready strategic summary connecting company mission to technical initiatives.

### How to Use
1. Ensure all research documents are uploaded to NotebookLM (including Merlin output)
2. Paste the Value Pyramid prompt
3. Run

### Prompt Example
```
Generate a Strategic Value Pyramid for this prospect.

[Include full prompt from your library]
```

### Key Outputs
- Company Mission (one sentence)
- Supporting Strategy (2-3 points on tech/digital transformation)
- Key Initiatives (3-4 current projects)
- Risks & Challenges (3-4 critical obstacles framed as business impacts)
- Technical Context (cloud platforms, security tools)

### Use For
- C-level meeting prep
- Team briefings
- Executive presentation decks
- Positioning solutions to business objectives

---

## Step 8: 3Y Challenge Framework

### What It Does
Generates a 3-column challenge framework for "Securing Prospect's Growth" slides.

### How to Use
1. Upload prospect research to NotebookLM (discovery notes, tech stack, MEDDPICC data)
2. Paste the 3Y prompt
3. Run

### Prompt Example
```
Create a 3Y Challenge Framework showing how this prospect's growth is being challenged across 3 strategic themes.

[Include full prompt from your library]
```

### Key Outputs
3 columns, each containing:
- **Business Theme/Goal** (e.g., "Democratizing Security")
- **3 Challenge Boxes** (header + 2-3 bullet points on business implications)

Challenges grounded in:
- Actual tech stack (AWS/Azure/GCP, current tools)
- MEDDPICC pain points with quantifiable impact
- Prospect's own language from discovery

### Use For
- Building executive presentation slides
- Connecting technical gaps to business outcomes
- Structuring discovery findings visually
- Aligning Wiz solutions to strategic goals

---

## Step 9: Champion Development Plan

### What It Does
Generates a champion-building strategy for each key persona at the prospect.

### How to Use
1. Upload prospect research to NotebookLM (contacts, discovery notes, org chart)
2. Paste the Champion Plan prompt
3. Run

### Prompt Example
```
Create a Champion Development Plan for the key stakeholders at this prospect.

[Include full prompt from your library]
```

### Key Outputs
A prioritized table with one row per contact/persona:
- **WHO & ROLE** - Title, influence level, decision authority
- **WHAT THEY CARE ABOUT** - Responsibilities, metrics, challenges
- **TYPICAL KPIs** - How Wiz impacts their performance scorecard
- **CHAMPION BUILDING IDEAS** - Value hooks, quick wins, enablement tactics

Personas ranked by influence and engagement readiness.

### Use For
- Tailoring messaging to each stakeholder
- Identifying quick wins to build credibility
- Equipping champions with internal advocacy tools
- Mapping multi-threaded engagement strategy

---

## Step 10: MEDDPICC Gap Analysis

### What It Does
Generates MEDDPICC gap analysis and role-tailored discovery questions for upcoming meetings.

### How to Use
1. Upload research to NotebookLM
2. **Optional:** Specify who you're meeting with
3. Paste the prompt
4. Run

### Prompt Example
```
Generate Discovery Call Prep with MEDDPICC Gap Analysis.

Meeting with: CISO and Cloud Security Manager

[Include full prompt from your library]
```

### Key Outputs
- **MEDDPICC Gap Analysis** - What we know vs. what's missing across all 8 elements
- **3 Question Funnels** - Tailored to attendees (open → probing → confirming)
- **Red Flags** - Deal risks and unvalidated assumptions

Questions customized to prospect's industry, tech stack, and attendee seniority/function.

### Use For
- Identifying critical unknowns before calls
- Preparing targeted discovery questions
- Avoiding deal-blocking surprises
- Running more strategic conversations

---

## Step 11: Outbound Outreach Generator

### What It Does
Generates personalized emails, LinkedIn messages, or call scripts using your research.

### How to Use
1. Ensure research documents are in NotebookLM (Industry, Business, Technology reports)
2. Paste the Outbound prompt
3. Fill in the inputs
4. Generate

### Prompt Example
```
Generate outbound outreach:

Contact: Sarah Chen, CISO, Revolut
Stage: Cold
Type: Email
Trigger: Recent FCA cloud security guidance
Pain Point: Multi-cloud compliance (AWS + GCP)
CTA: 30-min discovery call

[Include full prompt from your library]
```

### Input Variables
**Required:**
- Contact (Name, Role, Company)
- Stage (Cold / Warm / Re-engagement / Champion)
- Type (Email / LinkedIn / Call)
- CTA (Discovery call / Executive briefing / Technical deep-dive / Coffee / Event)

**Optional (better results):**
- Trigger (Recent news, funding, breach, regulation change)
- Pain Point (Something specific from research)

### Key Outputs
- Subject line (or opening hook)
- Core message (~80 words)
- Alternative version
- Talk track (if call selected)

### Quality Checklist
- [ ] Mentions something specific about their company/industry
- [ ] Focuses on business value (not Wiz features)
- [ ] Appropriate tone for relationship stage
- [ ] Clear, easy call-to-action
- [ ] Sounds human (not robotic)

---

## Step 12: Call Sheet / Meeting Prep

### What It Does
Generates comprehensive meeting preparation documents with attendee analysis, question funnels, and demo scenarios.

### How to Use
1. Upload research to NotebookLM (Industry, Business, Technology reports + Merlin output + MEDDPICC gaps)
2. Paste the Call Sheet prompt
3. Fill in attendees and purpose
4. Generate and copy to Google Docs
5. Share with SE for alignment

### Prompt Example
```
Generate Call Sheet:

Attendees: Sarah Chen (CISO), Mike Johnson (Cloud Architect), James Park (AppSec Director)
Meeting purpose: Second meeting - technical deep-dive on AWS multi-account setup, Splunk integration. Build James as champion.

[Include full prompt from your library]
```

### Key Outputs
- Attendee analysis with decision influence
- 2-3 question funnels (5 questions each) mapped to MEDDPICC gaps
- 2-3 demo scenarios connected to researched pain points
- Clear AE/SE prep split
- Meeting success criteria

### Use For
- AE/SE alignment before meetings
- Ensuring focused, strategic conversations
- Avoiding generic feature dumps
- Building champions through targeted engagement

---

## Step 13: Executive Research & Prep

### What It Does
Creates detailed executive briefings optimized for NotebookLM's audio podcast feature - perfect for pre-meeting listening.

### How to Use
1. Upload prospect research to NotebookLM
2. Paste the Executive Prep prompt with specific executive details
3. Generate
4. Use NotebookLM's audio feature to listen as podcast

### Prompt Example
```
I'm meeting with Jane Smith, CISO at Marks & Spencer (UK retail).

Create an executive briefing document covering:
- Executive background and career trajectory
- Recent company news and strategic initiatives
- Industry trends affecting retail in the UK
- Typical CISO concerns in retail
- Conversation starters and topics to avoid

[Include full prompt from your library]
```

### Tips for Best Results
- Be specific with executive names and titles
- Specify the industry/vertical for targeted insights
- Emphasize recent news (last 3-6 months)
- Request UK-specific regulatory and market context
- Always ask for source links

### Use For
- Pre-meeting briefings (listen to audio version during commute)
- Understanding executive priorities and background
- Identifying conversation hooks
- Avoiding missteps with sensitive topics

---

## Workflow Integration Map

```
1. Base Data (Manual) → NotebookLM
                ↓
2. Industry Report (Gemini) ────┐
3. Business Report (Gemini) ────┼──→ 5. Synthesis (Gemini)
4. Tech Report (Gemini) ────────┘           ↓
                                    6. Merlin (Slackbot)
                                            ↓
                                    NotebookLM Processing
                                            ↓
                    ┌───────────────────────┴───────────────────────┐
                    ↓                       ↓                       ↓
        7. Value Pyramid          9. Champion Plan        11. Outbound
        8. 3Y Framework          10. MEDDPICC Gaps        12. Call Sheet
                                                          13. Exec Prep
```

---

## Success Metrics

Track these to measure workflow effectiveness:
- **Time saved** on research and prep (target: 50% reduction)
- **Meeting quality** and engagement (subjective assessment)
- **Deal velocity** improvements (days to close)
- **Win rate** changes (before/after adoption)
- **Team adoption** and consistency (% of team using workflow)

---

## Next Steps: Roadmap

### Tier 1: Critical Path (Build Next)
- Discovery Question Generator
- Competitive Intelligence Brief
- Meeting Summary → Action Items

### Tier 2: Deal Acceleration
- Business Case Builder
- Follow-Up Email Generator
- Stakeholder Map Generator

### Tier 3: Competitive Advantage
- Security Posture Assessment Summary
- Custom Demo Script
- Regulatory & Compliance Context

### Tier 4: Scale & Efficiency
- Tech Stack Enrichment
- Customer News Alerts
- RFP Response Assistant
- Objection Response Library
- Win/Loss Analysis Template

---

## Quick Reference: When to Use What

| Scenario | Use These Steps |
|----------|-----------------|
| **First time researching prospect** | 1 → 2 → 3 → 4 → 5 → 6 → 7 |
| **Preparing for discovery call** | 10 (MEDDPICC Gaps) → 12 (Call Sheet) |
| **Meeting with C-suite executive** | 7 (Value Pyramid) → 13 (Exec Prep) |
| **Building champion relationships** | 9 (Champion Plan) |
| **Creating outreach** | 11 (Outbound Generator) |
| **Building exec presentation** | 7 (Value Pyramid) → 8 (3Y Framework) |
| **Updating account team** | 5 (Synthesis) → share brief |

---

## Tool Requirements

- **Gemini** - For Steps 2, 3, 4, 5 (research and synthesis)
- **Slack (Merlin)** - For Step 6 (Wiz alignment)
- **NotebookLM** - For Steps 7-13 (sales outputs)
- **Google Docs** - For sharing outputs with team

---

## Character Limits to Remember

- **NotebookLM prompts:** 1,900 characters max
- **Merlin (Slackbot):** 2,000 characters max
- **Synthesis output:** Under 10,000 characters (for Merlin input)

---

*Last Updated: November 2025*
*For prompt library and detailed templates, see individual prompt files*