# Wiz Research Prompt Templates

A collection of AI prompt templates for generating strategic sales and marketing research materials for Wiz.io's cloud security platform.

## Overview

This repository contains specialized prompts designed to create strategic alignment documents that map business objectives to Wiz's cloud security capabilities across three main product lines:

- **Wiz Cloud**: Cloud security posture management (CSPM), cloud infrastructure entitlement management (CIEM), vulnerability management
- **Wiz Code**: Code security, supply chain risk, Infrastructure as Code (IaC) scanning, CI/CD integration
- **Wiz Defend**: Cloud detection and response (CDR), runtime protection, threat detection and incident response

## Repository Contents

### Customer Intelligence Prompts

**[customer-general.md](customer-general.md)**
- Conducts comprehensive research on UK-headquartered businesses using publicly available information
- Generates detailed customer intelligence reports with sourced findings
- Minimum 25-30 data points with full source URLs and dates
- Ideal for pre-sales research and discovery

**[customer-wiz-aligned.md](customer-wiz-aligned.md)**
- Maps specific customer business objectives to Wiz product capabilities
- Creates tailored strategic alignment documents for individual prospects/customers
- Includes opportunity analysis, implementation roadmap, and ROI analysis
- Requires specific customer context (company size, cloud maturity, existing tools)

### Vertical/Segment Strategy Prompts

**[vertical-general.md](vertical-general.md)**
- Creates industry-wide strategy maps showing typical business objectives
- Generates market analysis and strategic planning documents for entire verticals
- Default output: PowerPoint presentation (10-15 pages for Executive Summary, 30-50 pages for Full Detailed Version)

**[vertical-wiz-aligned.md](vertical-wiz-aligned.md)**
- Maps industry-specific objectives to Wiz capabilities
- Provides go-to-market planning and sales enablement materials
- Includes compliance requirements, typical challenges, and implementation patterns by vertical

## Document Structure

All strategy maps follow a consistent hierarchical framework:

```
Business Goal ’ Strategies ’ Business Functions ’ Initiatives ’ Metrics/KPIs
```

### Typical Components:
- **Business Goals**: 4-6 high-level objectives
- **Strategies**: 3-4 approaches per goal
- **Business Functions**: Technology, Operations, Marketing, HR, Finance, Legal, Risk & Compliance
- **Initiatives**: 5-8 specific tactical actions per function
- **Metrics & KPIs**: 5-8 quantifiable indicators with target values
- **Sources & References**: 8-12 sources (Executive), 15-20 sources (Full Detailed)

## Usage

### Basic Usage

1. Choose the appropriate prompt template based on your needs
2. Copy the prompt content
3. Provide required context (customer name, vertical, company details, etc.)
4. Submit to your AI assistant (Claude Code recommended)

### Customization Options

**Detail Levels:**
- Executive Summary (default): Concise, scannable, 10-15 pages
- Full Detailed Version: Comprehensive, 30-50 pages (specify when prompting)

**Output Formats:**
- PowerPoint (default)
- Markdown
- Excel workbook
- Word document
- Visual diagrams

**Geographic/Segment Targeting:**
- Be specific: "UK Fintech, Series B-C companies"
- Include context: "B2B SaaS companies"
- Specify stage: "Early-stage startups vs. established players"

### Example Workflows

**Customer Research Workflow:**
```
1. Use customer-general.md to conduct initial research
2. Use customer-wiz-aligned.md to create strategic alignment document
3. Customize output format as needed (PowerPoint, Word, etc.)
```

**Vertical Strategy Workflow:**
```
1. Use vertical-general.md to understand market landscape
2. Use vertical-wiz-aligned.md to create Wiz-specific go-to-market materials
3. Request full detailed version for comprehensive analysis
```

## Research Quality Standards

### UK-Specific Sources

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

## Common Follow-Up Requests

After generating initial documents:

- Expand specific sections
- Add detail to metrics and KPIs
- Create visual artifacts (diagrams, charts)
- Convert between formats
- Add implementation guidance
- Include relevant case studies

## Requirements

- AI assistant with web search capabilities (for customer research prompts)
- Access to Claude Code or similar AI coding assistant recommended
- Internet access for research-based prompts

## Contributing

This repository is currently in active development. All prompt files are untracked and uncommitted in the current Git status.

## Documentation

See [CLAUDE.md](CLAUDE.md) for detailed guidance on:
- Prompt template structure and patterns
- Wiz product alignment framework
- Research methodologies
- Quality standards
- Customization patterns

## License

[Add license information]

## Contact

[Add contact information]
