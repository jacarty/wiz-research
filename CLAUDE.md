# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This repository contains a structured workflow of AI prompt templates for generating Wiz.io sales and marketing research materials. The prompts create strategic intelligence documents that map prospect business objectives to Wiz's cloud security platform capabilities (Wiz Code, Wiz Cloud, and Wiz Defend).

## Workflow Architecture

The repository implements a **13-step research-to-output pipeline** that feeds into NotebookLM for final deliverable generation. The workflow is visualized in [0_flow.mermaid](0_flow.mermaid) and follows this sequence:

### Phase 1: Data Gathering (Manual)
**Step 1: Base Data Collection** ([1_guide_base_data.md](1_guide_base_data.md))
- Gather prospect URLs (website, LinkedIn, X, social media)
- Collect data from Cognism, Marketing systems, and SFDC
- Manual input phase - no prompt execution

### Phase 2: Intelligence Reports (Gemini)
These three reports run in parallel using Gemini with web search:

**Step 2: Industry Intelligence** ([2_guide_industry.md](2_guide_industry.md), [2_prompt_industry.md](2_prompt_industry.md))
- Generates industry overview with market dynamics, trends, compliance requirements
- Deep-dive on cloud/SaaS/AI technology innovation in the vertical
- Output: 8-12 page executive-ready industry strategy map

**Step 3: Prospect Business Report** ([3_guide_prospect_business.md](3_guide_prospect_business.md), [3_prompt_prospect_business.md](3_prompt_prospect_business.md))
- Business intelligence on the specific prospect company
- Strategic initiatives, revenue drivers, organizational structure
- Focus on non-technical business context

**Step 4: Prospect Technology Report** ([4_guide_prospect_tech.md](4_guide_prospect_tech.md), [4_prompt_prospect_tech.md](4_prompt_prospect_tech.md))
- Technical intelligence: cloud platforms, security tools, tech stack
- Infrastructure analysis, development practices, compliance posture
- Technology-specific discovery

### Phase 3: Synthesis (Gemini)
**Step 5: GTM Intelligence Brief** ([5a_guide_synthesis.md](5a_guide_synthesis.md), [5a_prompt_synthesis.md](5a_prompt_synthesis.md))
- Synthesizes Steps 2, 3, and 4 into a consolidated brief
- Output must be under 10,000 characters for Merlin compatibility
- Combines industry + business + tech intelligence

**Step 5b: Merlin Prep (Optional)** ([5b_prompt_nlm_merlin_prep.md](5b_prompt_nlm_merlin_prep.md))
- Alternative synthesis prompt for NotebookLM input preparation

### Phase 4: Use-Case Alignment (Slackbot)
**Step 6: Merlin Analysis** ([6a_guide_merlin.md](6a_guide_merlin.md), [6a_prompt_merlin.md](6a_prompt_merlin.md), [6b_prompt_merlin.md](6b_prompt_merlin.md))
- Run in Slack using Merlin bot
- Analyzes GTM Intelligence Brief and generates ranked Wiz use-case recommendations
- Outputs top 5 priority use-cases aligned to prospect's business priorities
- Includes competitive displacement analysis

### Phase 5: NotebookLM Outputs (Steps 7-13)
Upload Steps 1-6 outputs to NotebookLM, then generate these deliverables:

**Step 7: Strategic Value Pyramid** ([7_guide_vp.md](7_guide_vp.md), [7_prompt_vp.md](7_prompt_vp.md))
- Company mission → Strategy → Initiatives → Risks → Technical context
- Executive-ready strategic summary

**Step 8: 3-Year Vision** ([8_guide_3y.md](8_guide_3y.md), [8_prompt_3Y.md](8_prompt_3Y.md))
- Long-term strategic planning document

**Step 9: Champion Plan** ([9_guide_champ_plan.md](9_guide_champ_plan.md), [9_prompt_champ_plan.md](9_prompt_champ_plan.md))
- Internal champion enablement strategy

**Step 10: MEDDPICC Gaps** ([10_guide_meddpicc_gaps.md](10_guide_meddpicc_gaps.md), [10_prompt_meddpicc_gaps.md](10_prompt_meddpicc_gaps.md))
- Discovery call preparation with gap analysis
- What we know vs. what's missing across all 8 MEDDPICC elements
- Role-tailored question funnels and red flags

**Step 11: Proof of Concept Prep** ([11_guide_pg.md](11_guide_pg.md), [11_prompt_pg.md](11_prompt_pg.md))
- POC planning and success criteria

**Step 12: Meeting Preparation** ([12_guide_meeting_prep.md](12_guide_meeting_prep.md), [12_prompt_meeting_prep.md](12_prompt_meeting_prep.md))
- General meeting prep briefings

**Step 13: Executive Research/Prep** ([13_guide_exec_prep.md](13_guide_exec_prep.md), [13_prompt_exec_prep.md](13_prompt_exec_prep.md))
- Executive-specific research and meeting preparation
- Designed for upload to NotebookLM for audio briefing generation

## File Naming Convention

All files follow a consistent pattern:
- `[NUMBER]_guide_[NAME].md` - User guide explaining how to use the prompt
- `[NUMBER]_prompt_[NAME].md` - Actual prompt template to copy/paste into AI assistant
- Numbers indicate workflow sequence (1-13)
- `0_flow.mermaid` - Visual workflow diagram

## AI Tool Routing

Different steps use different AI platforms:

| Step | Tool | Reason |
|------|------|--------|
| 2-5 | **Gemini** | Web search capabilities for research |
| 6 | **Merlin (Slackbot)** | Team collaboration, character limit optimization |
| 7-13 | **NotebookLM** | Synthesis across multiple documents, audio generation |

## Wiz Product Framework

When mapping to Wiz products, use this framework:

### Wiz Cloud
- Cloud security posture management (CSPM)
- Cloud infrastructure entitlement management (CIEM)
- Vulnerability management
- Agentless scanning and discovery
- Multi-cloud visibility (AWS, Azure, GCP)

### Wiz Code
- Code security and supply chain risk
- Infrastructure as Code (IaC) scanning
- CI/CD pipeline integration
- Developer security workflows
- Shift-left security practices

### Wiz Defend
- Cloud detection and response (CDR)
- Runtime protection
- Threat detection and incident response
- Security operations center (SOC) enablement
- Active threat hunting

## Research Quality Standards

### UK-Specific Research Sources (Primary Focus)
- **Companies House**: https://www.gov.uk/government/organisations/companies-house (registration, financials, directors)
- **ICO Register**: https://ico.org.uk/ (data protection, breach notifications)
- **UK Tech News**: ComputerWeekly, The Register UK, BusinessCloud, TechCrunch UK
- **UK Cloud Guidance**: NCSC Cloud Security Guidance, UK government cloud strategy

### Source Credibility Hierarchy
1. **Highest**: Company official sources (website, annual reports, press releases)
2. **High**: Government records (Companies House, ICO), financial filings
3. **Medium-high**: Major news outlets, analyst reports, cloud provider case studies
4. **Medium**: Trade publications, job postings, LinkedIn profiles
5. **Lower**: Glassdoor reviews, social media (use only to corroborate)

## Common Workflows

### Complete Deal Cycle (All 13 Steps)
1. Gather base data manually (Step 1)
2. Run parallel research in Gemini (Steps 2, 3, 4)
3. Synthesize in Gemini (Step 5)
4. Generate use-case alignment in Merlin (Step 6)
5. Upload all outputs to NotebookLM
6. Generate specific deliverables as needed (Steps 7-13)

### Quick Discovery Prep
1. Ensure Steps 1-6 are completed
2. Upload to NotebookLM
3. Run Step 10 (MEDDPICC Gaps) for meeting preparation

### Executive Meeting Prep
1. Ensure Steps 1-6 are completed
2. Upload to NotebookLM
3. Run Step 7 (Value Pyramid) for strategic context
4. Run Step 13 (Executive Prep) for specific executive research
5. Use NotebookLM's Audio Overview feature for listening before meeting

### POC Planning
1. Complete Steps 1-6
2. Upload to NotebookLM
3. Run Step 11 (PG Prep) for proof-of-concept planning

## Working with Prompt Templates

### Usage Pattern
1. Read the `_guide_` file to understand the prompt's purpose and usage
2. Copy content from the corresponding `_prompt_` file
3. Replace placeholders with actual values:
   - `[COMPANY NAME]` - Prospect company name
   - `[INDUSTRY]` - Industry/vertical
   - `[SEGMENT]` - Market segment or company size
   - `[EXECUTIVE NAME]` - Executive name for persona research
4. Submit to the appropriate AI tool (Gemini/Merlin/NotebookLM)
5. Iterate with follow-up requests as needed

### Character Limits
- **Merlin Input**: Must be under 10,000 characters (enforced in Step 5 synthesis)
- **NotebookLM**: No strict limit, but works best with focused documents

## Modifying Workflow

When updating prompt templates:

### Maintain Workflow Integrity
- Preserve the numbered sequence (1-13)
- Keep `_guide_` and `_prompt_` file pairs synchronized
- Update [0_flow.mermaid](0_flow.mermaid) if adding/removing steps
- Ensure Step 5 synthesis respects 10,000 character limit for Merlin

### Placeholder Format
- Use `[PLACEHOLDER IN BRACKETS]` or `**[BOLD PLACEHOLDER]**`
- Keep placeholders consistent across related prompts
- Document required vs. optional placeholders in guide files

### Test Changes
1. Run the modified prompt with a real example
2. Verify compatibility with downstream steps
3. Check that outputs feed cleanly into NotebookLM
4. Validate character limits for Merlin-bound content

## Repository Type

This is a **prompt template repository**, not a traditional code repository:
- No build system, compilation, or testing framework
- No package managers or dependencies
- Version control is for prompt evolution tracking
- Files are markdown documents, not executable code

## Current Repository State

Based on git status, several older files were deleted and new numbered workflow files (1-13) were added. The repository is in transition from the old naming scheme to the new numbered workflow system.
