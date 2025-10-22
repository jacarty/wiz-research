# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This repository contains prompt templates for generating Wiz.io sales and marketing research materials. The prompts are designed to create strategic alignment documents that map business objectives to Wiz's cloud security platform capabilities (Wiz Code, Wiz Cloud, and Wiz Defend).

## Core Prompt Types

### 1. Customer Intelligence Research (`customer-general.md`)
- **Purpose**: Conducts comprehensive research on UK-headquartered businesses using publicly available information
- **Output**: Detailed customer intelligence report with sourced findings
- **Use Case**: Pre-sales research to populate customer-specific strategy documents
- **Key Sections**: Company profile, strategic initiatives, cloud environment, security posture, stakeholder identification, pain points
- **Research Requirements**: Minimum of 25-30 data points with full source URLs and dates

### 2. Customer-Specific Strategy Map (`customer-wiz-aligned.md`)
- **Purpose**: Maps a specific customer's business objectives to Wiz product capabilities
- **Output**: Tailored strategic alignment document for a single customer
- **Use Case**: Opportunity analysis, sales strategy development, executive business cases
- **Key Sections**: Customer profile, business goals, Wiz alignment assessment, implementation roadmap, ROI analysis
- **Personalization**: Requires specific customer context (company size, cloud maturity, existing tools, known challenges)

### 3. Vertical/Segment Strategy Map (`vertical-general.md`, `vertical-wiz-aligned.md`)
- **Purpose**: Creates industry-wide strategy maps showing typical business objectives
- **Output**: Comprehensive strategic planning document for an entire vertical or market segment
- **Use Case**: Go-to-market planning, market analysis, sales enablement
- **Key Sections**: Market overview, typical business goals, business function alignment, compliance requirements
- **Detail Levels**:
  - Executive Summary (default): 10-15 pages, concise, scannable
  - Full Detailed Version: 30-50 pages, comprehensive
- **Default Format**: PowerPoint presentation (can be customized to Markdown, Excel, Word, etc.)

### 4. Executive Meeting Preparation (`persona-exec-meeting-prep.md`)
- **Purpose**: Creates comprehensive briefing documents for meeting senior executives at UK companies
- **Output**: Markdown briefing document with executive profile, company context, and conversation starters
- **Use Case**: Pre-meeting preparation, stakeholder research, relationship building
- **Key Sections**: Company overview & recent news, executive profile, industry insights, role-specific concerns, KPIs, jargon, conversation starters
- **Integration**: Output designed to be uploaded to NotebookLM for audio briefing generation
- **Personalization**: Requires executive name, title, company name, and industry/vertical

## Document Structure Patterns

All strategy maps follow a consistent hierarchical structure:

```
Business Goal → Strategies → Business Functions → Initiatives → Metrics/KPIs
```

### Typical Components:
- **Business Goals**: 4-6 high-level objectives
- **Strategies**: 3-4 approaches per goal
- **Business Functions**: Technology, Operations, Marketing, HR, Finance, Legal, Risk & Compliance
- **Initiatives**: 5-8 specific tactical actions per function
- **Metrics & KPIs**: 5-8 quantifiable indicators with target values
- **Challenges/Opportunities**: 4-5 items each
- **Compliance Requirements**: Relevant regulations and frameworks
- **Sources & References**: 8-12 sources (Executive), 15-20 sources (Full Detailed)

## Wiz Product Alignment

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

### Source Credibility Hierarchy:
1. **Highest**: Company official sources (website, annual reports, press releases)
2. **High**: Government records (Companies House, ICO), financial filings
3. **Medium-high**: Major news outlets, analyst reports, cloud provider case studies
4. **Medium**: Trade publications, job postings, LinkedIn profiles
5. **Lower**: Glassdoor reviews, social media (use only to corroborate)

### UK-Specific Research Sources:
- **Companies House**: https://www.gov.uk/government/organisations/companies-house (registration, financials, directors)
- **ICO Register**: https://ico.org.uk/ (data protection, breach notifications)
- **UK Tech News**: ComputerWeekly, The Register UK, BusinessCloud, TechCrunch UK
- **UK Cloud Guidance**: NCSC Cloud Security Guidance, UK government cloud strategy

## Common Customization Patterns

### Detail Level Selection:
```
Default (Executive Summary): Concise, scannable, 10-15 pages
Full Detailed Version: Comprehensive, 30-50 pages (specify: "create the full detailed version")
```

### Output Format Options:
```
PowerPoint (default - no need to specify)
Markdown ("Output as Markdown instead of PowerPoint")
Excel ("Create as an Excel workbook")
Word ("Output as a Word document")
Visual diagram ("Create as a visual diagram")
```

### Geographic/Segment Targeting:
```
Be specific: "UK Fintech, Series B-C companies" vs. "Fintech"
Include context: "Focus on B2B SaaS companies"
Specify stage: "Early-stage startups vs. established players"
```

## Common Workflows

### Complete Customer Engagement Workflow:
1. **Pre-Meeting Research**: Use `persona-exec-meeting-prep.md` to research the executive and company
2. **Company Intelligence**: Use `customer-general.md` for detailed organizational research
3. **Strategic Alignment**: Use `customer-wiz-aligned.md` to create tailored value proposition
4. **Presentation Preparation**: Request format conversion (PowerPoint, Word) and visual diagrams

### Vertical Go-to-Market Workflow:
1. **Market Analysis**: Use `vertical-general.md` to understand industry landscape
2. **Wiz Positioning**: Use `vertical-wiz-aligned.md` to create product alignment materials
3. **Sales Enablement**: Request executive summary version for quick reference
4. **Deep Dive**: Request full detailed version for comprehensive analysis

### Quick Executive Briefing Workflow:
1. **Generate Briefing**: Use `persona-exec-meeting-prep.md` with specific executive details
2. **Save Output**: Export as markdown or text file
3. **Upload to NotebookLM**: Add as source along with company reports
4. **Generate Audio**: Use NotebookLM's Audio Overview for listening before meeting

## Common Follow-Up Requests

After generating initial documents:
- Expand specific sections (e.g., "Expand the compliance section for Goal 3")
- Add detail to metrics (e.g., "Add more specific KPI targets for Marketing")
- Create visual artifacts (e.g., "Create a visual diagram showing relationships")
- Convert formats (e.g., "Convert this into a presentation with one goal per slide")
- Add implementation guidance (e.g., "Create an implementation roadmap")
- Include case studies (e.g., "Add case studies for each major initiative")

## Repository Structure

This is a **prompt template repository**, not a traditional code repository. It contains:
- **Prompt Templates** (.md files): Copy-paste templates for AI assistants
- **Documentation**: README.md and this CLAUDE.md file
- **No Build System**: No compilation, testing, or deployment required
- **Usage Pattern**: Copy prompt content → Customize placeholders → Submit to AI assistant

### File Organization:
```
/
├── customer-general.md          # Customer intelligence research prompt
├── customer-wiz-aligned.md      # Customer-specific Wiz alignment prompt
├── vertical-general.md          # Industry/vertical analysis prompt
├── vertical-wiz-aligned.md      # Vertical-specific Wiz alignment prompt
├── persona-exec-meeting-prep.md # Executive meeting preparation prompt
├── README.md                    # Repository documentation
├── CLAUDE.md                    # This file - guidance for Claude Code
├── LICENSE                      # MIT License
└── CODEOWNERS                   # Repository maintainer (@jacarty)
```

### Working with Prompt Templates:
1. Read the relevant .md file to understand its purpose and structure
2. Copy the prompt content (usually marked with "PROMPT TO USE" or similar heading)
3. Replace placeholders (e.g., [COMPANY NAME], [EXECUTIVE NAME]) with actual values
4. Submit to Claude Code or another AI assistant with web search capabilities
5. Iterate with follow-up requests as needed

## Modifying Prompt Templates

When updating prompt templates in this repository:

### Maintain Structure:
- Keep the hierarchical document structure consistent across all strategy maps
- Preserve placeholder format: `[PLACEHOLDER IN BRACKETS]` or `**[BOLD PLACEHOLDER]**`
- Maintain section headers and subsection organization
- Keep source citation requirements explicit

### Test Changes:
1. After modifying a prompt, test it with a real example
2. Verify all placeholders are clearly marked
3. Ensure output quality matches expectations
4. Check that sourcing requirements are maintained

### Documentation:
- Update README.md when adding new prompt types
- Update this CLAUDE.md when changing workflows or usage patterns
- Include usage examples in the prompt template itself
