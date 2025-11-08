# Wiz Research Prompt Templates

A structured 13-step workflow of AI prompt templates for generating strategic sales and marketing research materials for Wiz.io's cloud security platform.

## Overview

This repository contains a research-to-output pipeline that creates strategic intelligence documents mapping prospect business objectives to Wiz's cloud security capabilities across three main product lines:

- **Wiz Cloud**: Cloud security posture management (CSPM), cloud infrastructure entitlement management (CIEM), vulnerability management
- **Wiz Code**: Code security, supply chain risk, Infrastructure as Code (IaC) scanning, CI/CD integration
- **Wiz Defend**: Cloud detection and response (CDR), runtime protection, threat detection and incident response

## Workflow Overview

The repository implements a **13-step research pipeline** that progresses through data gathering → intelligence reports → synthesis → use-case alignment → deliverable generation. See [0_flow.mermaid](0_flow.mermaid) for the visual workflow diagram.

### The 13 Steps

#### Phase 1: Data Gathering (Manual)
1. **Base Data Collection** - Gather prospect URLs and internal data sources

#### Phase 2: Intelligence Reports (Gemini)
2. **Industry Intelligence** - Market dynamics, trends, compliance requirements
3. **Prospect Business Report** - Strategic initiatives, revenue drivers, organizational structure
4. **Prospect Technology Report** - Cloud platforms, security tools, tech stack analysis

#### Phase 3: Synthesis (Gemini)
5. **GTM Intelligence Brief** - Consolidated brief combining industry + business + tech intelligence

#### Phase 4: Use-Case Alignment (Merlin Slackbot)
6. **Merlin Analysis** - Ranked Wiz use-case recommendations aligned to prospect priorities

#### Phase 5: Deliverables (NotebookLM)
7. **Strategic Value Pyramid** - Executive-ready strategic summary
8. **3-Year Vision** - Long-term strategic planning document
9. **Champion Plan** - Internal champion enablement strategy
10. **MEDDPICC Gaps** - Discovery call preparation with gap analysis
11. **Proof of Concept Prep** - POC planning and success criteria
12. **Meeting Preparation** - General meeting prep briefings
13. **Executive Research/Prep** - Executive-specific research and meeting prep

## File Structure

All files follow a consistent naming pattern:

- `[NUMBER]_guide_[NAME].md` - User guide explaining how to use the prompt
- `[NUMBER]_prompt_[NAME].md` - Actual prompt template to copy/paste into AI assistant
- `0_flow.mermaid` - Visual workflow diagram
- `CLAUDE.md` - Comprehensive guidance for AI assistants working in this repository

### Quick Reference

| Step | Guide | Prompt | Tool | Purpose |
|------|-------|--------|------|---------|
| 1 | [1_guide_base_data.md](1_guide_base_data.md) | - | Manual | Gather URLs and internal data |
| 2 | [2_guide_industry.md](2_guide_industry.md) | [2_prompt_industry.md](2_prompt_industry.md) | Gemini | Industry intelligence report |
| 3 | [3_guide_prospect_business.md](3_guide_prospect_business.md) | [3_prompt_prospect_business.md](3_prompt_prospect_business.md) | Gemini | Business intelligence report |
| 4 | [4_guide_prospect_tech.md](4_guide_prospect_tech.md) | [4_prompt_prospect_tech.md](4_prompt_prospect_tech.md) | Gemini | Technology intelligence report |
| 5 | [5a_guide_synthesis.md](5a_guide_synthesis.md) | [5a_prompt_synthesis.md](5a_prompt_synthesis.md) | Gemini | GTM Intelligence Brief synthesis |
| 6 | [6a_guide_merlin.md](6a_guide_merlin.md) | [6a_prompt_merlin.md](6a_prompt_merlin.md) | Merlin | Use-case alignment analysis |
| 7 | [7_guide_vp.md](7_guide_vp.md) | [7_prompt_vp.md](7_prompt_vp.md) | NotebookLM | Strategic Value Pyramid |
| 8 | [8_guide_3y.md](8_guide_3y.md) | [8_prompt_3Y.md](8_prompt_3Y.md) | NotebookLM | 3-Year Vision |
| 9 | [9_guide_champ_plan.md](9_guide_champ_plan.md) | [9_prompt_champ_plan.md](9_prompt_champ_plan.md) | NotebookLM | Champion Plan |
| 10 | [10_guide_meddpicc_gaps.md](10_guide_meddpicc_gaps.md) | [10_prompt_meddpicc_gaps.md](10_prompt_meddpicc_gaps.md) | NotebookLM | MEDDPICC Gaps Analysis |
| 11 | [11_guide_pg.md](11_guide_pg.md) | [11_prompt_pg.md](11_prompt_pg.md) | NotebookLM | POC/PG Prep |
| 12 | [12_guide_meeting_prep.md](12_guide_meeting_prep.md) | [12_prompt_meeting_prep.md](12_prompt_meeting_prep.md) | NotebookLM | Meeting Preparation |
| 13 | [13_guide_exec_prep.md](13_guide_exec_prep.md) | [13_prompt_exec_prep.md](13_prompt_exec_prep.md) | NotebookLM | Executive Research/Prep |

## Common Workflows

### Complete Deal Cycle (All 13 Steps)
```
1. Gather base data manually (Step 1)
2. Run parallel research in Gemini (Steps 2, 3, 4)
3. Synthesize in Gemini (Step 5)
4. Generate use-case alignment in Merlin (Step 6)
5. Upload all outputs to NotebookLM
6. Generate specific deliverables as needed (Steps 7-13)
```

### Quick Discovery Prep
```
1. Ensure Steps 1-6 are completed
2. Upload to NotebookLM
3. Run Step 10 (MEDDPICC Gaps) for targeted discovery questions
```

### Executive Meeting Prep
```
1. Ensure Steps 1-6 are completed
2. Upload to NotebookLM
3. Run Step 7 (Value Pyramid) for strategic context
4. Run Step 13 (Executive Prep) for specific executive research
5. Use NotebookLM's Audio Overview feature for listening before meeting
```

### POC Planning
```
1. Complete Steps 1-6
2. Upload to NotebookLM
3. Run Step 11 (PG Prep) for proof-of-concept planning
```

## AI Tool Requirements

Different steps use different AI platforms:

- **Gemini** (Steps 2-5): Web search capabilities for research and synthesis
- **Merlin Slackbot** (Step 6): Team collaboration and use-case alignment
- **NotebookLM** (Steps 7-13): Multi-document synthesis and audio generation

### Important Constraints
- **Merlin Input Limit**: 10,000 characters (enforced in Step 5 synthesis)
- **NotebookLM**: Works best with focused documents; supports audio overview generation

## How to Use

### Basic Usage

1. **Read the Guide**: Open the `_guide_` file for the step you're working on
2. **Copy the Prompt**: Open the corresponding `_prompt_` file and copy its contents
3. **Replace Placeholders**: Substitute values for:
   - `[COMPANY NAME]` - Prospect company name
   - `[INDUSTRY]` - Industry/vertical
   - `[SEGMENT]` - Market segment or company size
   - `[EXECUTIVE NAME]` - Executive name for persona research
4. **Submit to AI Tool**: Use the correct platform (Gemini/Merlin/NotebookLM)
5. **Iterate**: Refine with follow-up requests as needed

### Example: Running Step 2 (Industry Intelligence)

```
1. Open 2_guide_industry.md to understand the output format
2. Copy the full prompt from 2_prompt_industry.md
3. Replace [INDUSTRY] and [SEGMENT] with your values
4. Paste into Gemini and run
5. Save the output for Step 5 synthesis
```

## Research Quality Standards

### UK-Specific Research Sources

When conducting research on UK companies, prioritize:

1. **Official Sources**: Company websites, annual reports, press releases
2. **Government Records**: Companies House, ICO Register
3. **Financial Data**: Published financial filings, analyst reports
4. **News & Analysis**: ComputerWeekly, The Register UK, BusinessCloud
5. **Cloud Providers**: AWS, Azure, GCP case studies and customer references

### Source Credibility Hierarchy

1. **Highest**: Company official sources
2. **High**: Government records, financial filings
3. **Medium-high**: Major news outlets, analyst reports
4. **Medium**: Trade publications, job postings
5. **Lower**: Social media (use only to corroborate)

## Output Examples

Outputs are stored in the [example_output/](example_output/) directory to demonstrate expected format and quality for each step.

## Documentation

- **[README.md](README.md)** (this file): Quick start guide and workflow overview
- **[CLAUDE.md](CLAUDE.md)**: Comprehensive guidance for AI assistants, including:
  - Detailed workflow architecture
  - AI tool routing logic
  - Wiz product alignment framework
  - Research methodologies
  - Customization patterns
  - Testing guidelines

## Contributing

This repository is in active development. When modifying prompt templates:

1. Maintain the numbered sequence (1-13)
2. Keep `_guide_` and `_prompt_` file pairs synchronized
3. Update [0_flow.mermaid](0_flow.mermaid) if adding/removing steps
4. Test changes with real examples before committing
5. Ensure Step 5 synthesis respects the 10,000 character limit for Merlin

## License

[Add license information]

## Contact

[Add contact information]
