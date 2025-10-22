# Customer-Specific Strategy with Wiz Alignment Map Generator

## How to Use
This prompt generates a strategic alignment document that maps a **specific customer's** business objectives, initiatives, and organizational priorities to Wiz.io's cloud security platform capabilities. It prioritizes understanding the customer's actual business strategies, then demonstrates how and where Wiz products provide targeted value.

Use this for customer discovery, opportunity analysis, sales strategy development, solution architecture planning, and executive business case development.

---

## Prompt Template

```
Create a comprehensive Customer-Specific Strategy with Wiz Alignment Map for [CUSTOMER NAME].

Customer Context:
- Company: [Company name and brief description]
- Industry/Vertical: [Industry vertical and relevant sub-sector]
- Company Size: [Employee count, revenue, growth stage]
- Cloud Maturity: [Cloud adoption level - cloud-native, hybrid, migrating, multi-cloud]
- Primary Cloud Providers: [AWS, Azure, GCP, and/or other platforms]
- Current Security Tools: [Known existing security tools and vendors]
- Key Business Drivers: [Primary business initiatives and goals]
- Known Challenges: [Any disclosed security or operational challenges]
- Customer Type: [Prospect, active opportunity, customer, expansion opportunity, at-risk renewal]

This document should be structured to prioritize THIS SPECIFIC CUSTOMER'S strategic objectives and business context first, then demonstrate how Wiz.io's Cloud Security Platform (Wiz Code, Wiz Cloud, and Wiz Defend) aligns with and enables those objectives.

---

## PART 1: CUSTOMER PROFILE & BUSINESS CONTEXT

### Company Overview
Provide a detailed understanding of this specific customer:
- **Company Background**: Founded, headquarters, key business lines
- **Market Position**: Market share, competitive positioning, key competitors
- **Financial Profile**: Revenue, growth rate, profitability, funding status
- **Organizational Structure**: Relevant departments, team sizes, reporting lines
- **Recent Company News**: Notable announcements, M&A, product launches, leadership changes
- **Strategic Initiatives**: Announced business priorities, transformation programs, growth plans

### Current Technology & Cloud Environment
- **Cloud Strategy**: Current multi-cloud approach, primary and secondary providers
- **Application Architecture**: Microservices, monolithic, serverless, containerized patterns
- **Infrastructure Patterns**: Data center presence, hybrid cloud deployment, edge computing
- **Development Velocity**: Release cadence, team structure, DevOps maturity
- **CI/CD Maturity**: Pipeline sophistication, automation level, integration practices
- **Existing Security Stack**: Current tools, vendors, and technology investment

### Organizational Security Context
- **Security Team Structure**: CISO reporting line, SOC size and maturity, engineering security team
- **Security Maturity Model**: Current CMMC/maturity assessment, audit readiness
- **Regulatory Environment**: Applicable regulations, compliance frameworks, audit cycles
- **Recent Security Events**: Known incidents, breach history, security-driven changes
- **Security Culture**: Organizational attitude toward security, developer security involvement
- **Security Budget & Planning**: Known budget constraints or planned investments

### Known Buyer Personas & Decision-Makers
For each key stakeholder (target 3-5):
- **Role/Title**: [Specific person if known, or role type]
- **Department**: Security, Engineering, DevOps, Compliance, etc.
- **Key Priorities**: What matters most to this person
- **Pain Points**: Specific challenges they face
- **Success Criteria**: How they measure success
- **Influence Level**: Decision authority, veto power, champion potential

---

## PART 2: CUSTOMER'S STATED BUSINESS GOALS & STRATEGIC PRIORITIES

For each major business goal stated or implied for this customer (target 4-6 goals), structure as follows:

### Goal [X]: [Customer's Specific Business Objective]
*The actual business outcome this customer is trying to achieve, in their own terms*

#### Business Context & Customer Motivation (Target: 100-150 words)
- Why this goal matters specifically to THIS customer
- Business drivers and strategic importance to their organization
- Known pain points or blockers they've mentioned or that are evident
- Their success criteria and definition of "good" for this goal
- Urgency level and timing factors
- Where this fits in their broader strategic roadmap

#### Customer's Current Approach & Initiatives
- 3-4 bullet points on what this customer is currently doing or planning to achieve this goal
- Existing tools or processes they're using
- Known gaps or limitations in their current approach
- Any stated challenges or frustrations with their current solution

#### Wiz Alignment Assessment - Customer-Specific

**How Wiz Enables This Goal**
- **Relevant Wiz Product(s)**: Which Wiz product(s) directly address this customer's goal
- **Specific Customer Scenario**: How this customer would actually use Wiz
- **Competitive Advantage**: Why Wiz is better positioned than their current approach
- **Key Differentiators**: Wiz capabilities that specifically matter to this customer's context

**Realistic Outcomes & Business Impact for This Customer**
- Specific, quantified improvements possible based on their environment
- Operational efficiencies they could gain
- Cost reductions or revenue enablement achievable
- Timeline for realizing these benefits

**Customer-Specific Success Metrics & KPIs**
List 5-8 measurable indicators tailored to THIS CUSTOMER with realistic target values. Use format: **Metric Name**: Current State → Target (timeframe):
- Deployment metrics specific to their environment (e.g., **Time to Full Cloud Visibility**: 4 weeks → <24 hours)
- Operational metrics matching their current maturity (e.g., **MTTR**: 72 hours → 8 hours [90% reduction])
- Coverage metrics based on their infrastructure (e.g., **Multi-cloud Asset Coverage**: 45% → 100%)
- Business metrics aligned to their stated priorities (e.g., **Security Issues in Production**: 25/month → <3/month)
- Efficiency metrics reflecting their team constraints (e.g., **Security Issues Reviewed by Developers**: 20% → 95%)

---

## PART 3: CUSTOMER'S ORGANIZATIONAL FUNCTION ALIGNMENT

Focus on the three core business functions most relevant to THIS CUSTOMER'S operations and pain points. For each function, describe what's happening specifically at this customer:

### Security Operations (SecOps) - THIS CUSTOMER'S CONTEXT
**Primary Wiz Product**: Wiz Defend

**Customer's Current State & Initiatives**:
- Describe the customer's current SOC setup, team size, and maturity level
- List 5-7 actual initiatives or challenges this customer faces
- Specific pain points they've mentioned or that align with industry norms for their size
- Current tools they use and any known limitations
- Compliance and incident response requirements relevant to them

**Why Wiz Matters for This Customer**:
- How Wiz directly addresses their specific SecOps challenges
- Key capabilities that solve their stated (or implied) pain points
- Integration with their existing tools and processes
- Impact on their specific team structure and workflow

**Expected Outcomes for This Customer**:
- Specific metrics they would care about (detection speed, MTTR, alert noise, team efficiency)
- Realistic improvements based on their current maturity level
- Cost or headcount implications
- Compliance or audit benefits
- Timeline for implementation and value realization

---

### Cloud Security / Infrastructure Security - THIS CUSTOMER'S CONTEXT
**Primary Wiz Product**: Wiz Cloud

**Customer's Current State & Initiatives**:
- Describe their multi-cloud environment (AWS, Azure, GCP proportions)
- Current cloud security practices and tool usage
- Known misconfigurations or security debt they've mentioned
- Compliance requirements specific to their industry and customer base
- Their cloud migration trajectory and infrastructure growth patterns

**Why Wiz Matters for This Customer**:
- How Wiz's agentless visibility applies to their specific cloud architecture
- Security Graph capabilities relevant to their attack surface
- Compliance automation benefits for their specific regulatory requirements
- Integration with their development and ops workflows

**Expected Outcomes for This Customer**:
- Specific metrics aligned to their infrastructure (e.g., cloud coverage %, critical risks, MTTR to remediation)
- Compliance benefits (audit readiness, policy automation, compliance reporting)
- Developer velocity impact (shifting left, reducing cloud-related security delays)
- Cost implications (cloud spend optimization, reduced incident costs)

---

### Application Development / DevSecOps - THIS CUSTOMER'S CONTEXT
**Primary Wiz Product**: Wiz Code

**Customer's Current State & Initiatives**:
- Development team size, engineering organization structure
- Current development practices (release cadence, sprint length, CI/CD maturity)
- Development security capabilities and tools (SAST, SCA, secrets management)
- Known challenges in shifting security left or developer security adoption
- IaC usage and infrastructure-as-code security maturity

**Why Wiz Matters for This Customer**:
- How Wiz Code reduces friction in their development workflow
- Code-to-cloud visibility benefits specific to their architecture
- Developer experience improvements for their team structure
- Pre-production risk detection aligned to their development velocity
- Supply chain security considerations for their specific dependencies and vendors

**Expected Outcomes for This Customer**:
- Developer remediation speed and quality improvements
- Pre-production vs. production security issue distribution shift
- Reduced security-related deployment delays
- Developer productivity and satisfaction improvements
- Supply chain risk visibility and management

---

### Cross-Functional: Risk & Compliance - THIS CUSTOMER'S CONTEXT
**Wiz Products**: All three products (Code, Cloud, Defend)

**Customer's Compliance & Audit Environment**:
- Applicable regulations (HIPAA, PCI-DSS, SOC 2, ISO 27001, etc.)
- Audit frequency and auditor requirements
- Known compliance gaps or recent audit findings
- Customer expectations and contract requirements
- Internal audit or governance cadence

**Common Initiatives in This Customer's Context**:
- List 5-7 actual risk and compliance initiatives this customer is prioritizing
- Known audit findings or compliance gaps they're addressing
- Continuous compliance challenges specific to their industry/size
- Reporting and governance requirements

**How Wiz Enables This Customer's Compliance Goals**:
- Automated compliance evidence collection for their specific frameworks
- Reporting capabilities aligned to their audit needs
- Continuous compliance monitoring vs. point-in-time audits
- Risk quantification and prioritization for their stakeholders

**Typical Outcomes for This Customer**:
- Reduced audit preparation time and cost
- Faster compliance evidence generation
- Reduced audit findings and remediation cycles
- Improved risk visibility to board/executive stakeholders
- Continuous compliance monitoring efficiency

---

## PART 4: CUSTOMER OPPORTUNITY ANALYSIS

### Competitive & Tool Landscape Assessment
- **Current Security Tools**: Known vendors and tools the customer uses
- **Gaps in Current Approach**: Limitations or pain points with existing tools
- **Competitive Threats**: Who Wiz competes with in their environment
- **Switching Costs**: Factors making change difficult (vendor lock-in, integration, training)
- **Win/Loss Patterns**: What matters most in selection decisions for this customer type

### Deal Dynamics & Sales Context
- **Opportunity Stage**: Early awareness, active evaluation, negotiation, etc.
- **Budget Status**: Known budget available, timing, budget cycle
- **Buying Process**: Known approval authorities, evaluation criteria, timeline
- **Strategic Initiatives**: How Wiz aligns with their strategic imperatives
- **Internal Champions**: Likely champions, skeptics, and influencers
- **Competitive Positioning**: Differentiated reasons to choose Wiz vs. alternatives

### Customer ROI & Business Case
*Tailored to THIS customer's specific situation*

**Investment Required**:
- Implementation effort and timeline
- Training and enablement needs
- Tool consolidation or replacement costs
- Any required organizational changes

**Benefits Achievable**:
- Quantified time savings (SOC efficiency, developer time, analyst time)
- Cost avoidance (incident prevention, reduced audit costs, tool consolidation)
- Revenue enablement (faster product releases, new market access, customer satisfaction)
- Risk reduction (compliance, breach prevention, audit readiness)

**Business Case Metrics**:
- **ROI Timeline**: When will the customer break even?
- **Year 1 Impact**: Quantified value in first 12 months
- **3-Year Value**: Projected cumulative benefit
- **Payback Period**: Months to positive ROI
- **Key Assumptions**: What needs to be true for this ROI to be realized

### Implementation Roadmap
**Phased Approach**:
- **Phase 1 [Weeks X-Y]**: Initial deployment and visibility
- **Phase 2 [Weeks X-Y]**: Integration with their tools and workflows
- **Phase 3 [Weeks X-Y]**: Full enablement and optimization

**Success Criteria for This Customer**:
- Specific milestones aligned to their priorities
- Expected outcomes at each phase
- Customer team involvement and responsibilities

---

## PART 5: CUSTOMER-SPECIFIC USE CASES & SCENARIOS

### Use Case 1: [Customer-Specific Scenario]
*A realistic scenario based on this customer's environment and challenges*

**Business Context**: Why this matters to THIS customer specifically
**Technical Scenario**: How the situation manifests in their environment
**Solution with Wiz**: Step-by-step how Wiz enables the outcome
**Customer Impact**: Specific benefits for this customer

### Use Case 2: [Another Customer-Specific Scenario]
*Additional scenario highlighting different Wiz capabilities or teams*

---

## PART 6: RISK & CONCERNS ASSESSMENT

### Potential Customer Objections & Concerns
- **Technical Concerns**: Known technical objections or integration questions
- **Organizational Concerns**: Change management, team capability, internal resistance
- **Commercial Concerns**: Price sensitivity, budget constraints, ROI concerns
- **Competitive Concerns**: Preference for current vendor, switching costs
- **Capability Concerns**: Does Wiz address ALL their needs, or are there gaps?

### Wiz Limitations for This Customer
Honestly assess what Wiz does NOT address:
- Specific capabilities this customer might need that Wiz doesn't provide
- Complementary tools they might still need
- Scenarios where alternatives might be better positioned
- Known gaps in Wiz's capabilities relevant to their environment

### Mitigation & Positioning Strategy
- How to address each concern authentically
- Where to reinforce Wiz's strengths vs. this customer's priorities
- How to handle competitive positioning
- Reference customers or case studies most relevant to THIS customer

---

## PART 7: DISCOVERY & ENGAGEMENT STRATEGY

### Key Discovery Questions
*Targeted questions to validate assumptions and uncover real pain points*

For the CISO/Security Leader:
- [3-4 specific discovery questions]

For the VP/Head of Engineering:
- [3-4 specific discovery questions]

For the DevSecOps/Platform Engineering Lead:
- [3-4 specific discovery questions]

For the Compliance/Risk Officer:
- [3-4 specific discovery questions]

### Recommended Engagement Approach
- **Initial Conversation**: Focus areas, tone, references
- **Technical Deep Dive**: What to demo, who should attend
- **Business Conversation**: ROI, business impact, executive alignment
- **References**: Which Wiz customer stories are most relevant to THIS customer

### Win Strategy
- **Value Drivers**: What matters most to decision-makers
- **Competitive Positioning**: How to position vs. known alternatives
- **Timeline**: Realistic sales cycle for this customer type
- **Stakeholder Alignment**: How to ensure all decision-makers see value
- **Risk Mitigation**: How to move past concerns and build consensus

---

## PART 8: REFERENCES & EVIDENCE

### Relevant Wiz Case Studies
List Wiz customer case studies or testimonials most relevant to THIS customer:
- **Case Study Name**: [Link to case study]
  - Similar company size, industry, or use case
  - Specific outcomes they achieved (with numbers)
  - Why this reference is relevant to THIS customer
- **Customer Testimonial**: [Link or source]
  - Quote or summary from similar customer
  - Context and relevance

### Analyst & Industry Research
For each source, include title, author/organization, publication date, and full link:
- **[Report Title]**: [Full URL]
  - Author/Organization, Publication Date
  - Relevance: Why this report matters for THIS customer's situation
  - Key Finding: Most relevant insight from the report
  
- **[Benchmark Study]**: [Full URL]
  - Source, Publication Date
  - Data relevant to their company size/industry
  - How it supports the proposed ROI or outcomes

### Compliance & Regulatory Resources
For each framework or regulation relevant to THIS customer:
- **[Regulation/Framework Name]**: [Full URL to official source]
  - Governing Body/Organization
  - Applicability to THIS customer
  - Key requirements impacting their security strategy
  - Link to official documentation

Example format:
- **HIPAA Security Rule**: https://www.hhs.gov/hipaa/for-professionals/security/
  - U.S. Department of Health & Human Services
  - Applicable if customer operates in healthcare or handles PHI
  - Requires continuous monitoring and incident response capabilities
  - Full compliance framework documentation

### Wiz Resources & Documentation
With direct links and context:
- **[Resource Title]**: [Full URL]
  - Wiz product/blog/whitepaper
  - Why this resource addresses THIS customer's needs
  - Specific sections or features most relevant
  
- **Product Documentation**: [Link to docs.wiz.io or relevant page]
  - Specific capability or integration documentation
  - Relevance to THIS customer's tech stack

Example:
- **Wiz Code Documentation - IaC Security**: https://docs.wiz.io/[path]
  - Covers infrastructure-as-code scanning and secrets detection
  - Relevant for THIS customer's Terraform and CloudFormation usage
  - Shows integration with their CI/CD pipeline tools

### Company-Specific Research
Research specific to THIS customer's company:
- **[Company Name] News**: [Link to announcement/news article]
  - Publication/Source, Date
  - Relevance to security or cloud strategy initiatives
  - Connection to Wiz alignment

- **[Company Name] Financial Data**: [Link to source - SEC filing, earnings call, etc.]
  - Source and Date
  - Growth trajectory and cloud investment implications
  - Relevant to ROI timeline and budget availability

- **[Company Name] Tech Stack Research**: [Link to sources - LinkedIn, Crunchbase, StackShare, etc.]
  - Current known tools and infrastructure
  - Links to documentation for better understanding of their environment
  - Competitive tools they may be evaluating

### Industry-Specific Resources
- **[Industry Association] Reports**: [Full URL]
  - Organization and publication date
  - Key trends or benchmarks relevant to THIS customer
  - Security challenges specific to their industry

- **[Regulatory Body] Guidance**: [Full URL]
  - Guidance document or resource
  - How it relates to THIS customer's compliance requirements
  - Link to full guidance documentation

---

## PART 9: RESEARCH METHODOLOGY & SOURCE ATTRIBUTION

### How This Analysis Was Conducted
Describe the sources and methods used to create THIS analysis:
- Public company research conducted on: [websites, news sources, LinkedIn, etc.]
- Industry research from: [analyst firms, association reports, publications]
- Regulatory research from: [official government/regulatory sources]
- Competitor research from: [vendor websites, customer reviews, G2, etc.]
- Wiz resource compilation from: [Wiz documentation, case studies, blogs]

### Source Quality & Verification
- All Wiz case studies and testimonials: [Link to Wiz customer success page]
- All regulatory compliance information: [Link to official sources - HHS, SEC, etc.]
- All analyst data: [Source of analyst reports - Gartner, Forrester, etc.]
- All product information: [Links to official product documentation]

### Key Assumptions & Limitations
- **Assumption 1**: [What we assumed about the customer or their situation]
  - Source or basis for assumption
  - How this affects the analysis
  - How to validate this assumption with the customer

- **Assumption 2**: [Another key assumption]
  - How it impacts recommendations
  - Validation method

### Recommended Additional Research
If you want to deepen this analysis, consider researching:
- [Specific aspect of customer environment]
- [Competitor capability or positioning]
- [Industry trend or benchmark]
- [Regulatory change or compliance requirement]
- [Customer's specific technology or vendor]

With suggested sources or search terms for each

---

## FORMATTING REQUIREMENTS

- Use clear headers and subheaders with proper hierarchy
- Lead with THIS CUSTOMER'S actual business priorities before Wiz capabilities
- Be specific and quantitative with metrics (avoid generic statements)
- Use customer-specific language and context throughout
- Provide concrete examples based on THIS CUSTOMER'S environment
- Clearly acknowledge Wiz limitations for this customer's situation
- Include realistic, achievable outcomes based on this customer's maturity level
- Make it actionable for sales, solutions, and customer success teams
- **Include specific, named references and sources where available**
- **Tie everything back to THIS CUSTOMER'S stated or evident priorities**

---

## DOCUMENT TONE & PERSPECTIVE

This document should be written from a **customer-specific sales and solution strategy perspective** that:
- Demonstrates deep understanding of THIS CUSTOMER'S business priorities
- Shows how Wiz enables THIS CUSTOMER'S specific strategic objectives
- Acknowledges what Wiz can't do for THIS CUSTOMER
- Uses THIS CUSTOMER'S specific context and language
- Balances technical capabilities with business value relevant to THIS CUSTOMER
- Positions Wiz as the right fit (or highlights where it might not be) for THIS CUSTOMER
- Provides a roadmap for sales and solutions teams to engage effectively
- Helps identify the best starting point and engagement strategy
- Serves as a reference for internal alignment and opportunity planning

---

Please create a detailed, professional document that would be valuable for:
- Sales opportunity planning and deal strategy
- Solution architecture and customer-specific implementation planning
- Executive conversations with C-suite prospects
- Technical discovery and requirements alignment
- Business case development and ROI modeling for THIS CUSTOMER
- Understanding THIS CUSTOMER'S buying process and decision criteria
- Risk assessment and competitive positioning
- Customer success planning and post-sale engagement strategy
```

---

## Example Usage

**Input:**
```
Create a comprehensive Customer-Specific Strategy with Wiz Alignment Map for Acme Corporation.

Customer Context:
- Company: Acme Corporation (E-commerce, Series C SaaS backend platform)
- Industry: E-commerce Technology
- Company Size: 350 employees, $45M ARR, founded 2019
- Cloud Maturity: Multi-cloud - 60% AWS, 35% Azure, 5% GCP
- Primary Cloud Providers: AWS (RDS, EC2, Lambda), Azure (Kubernetes, VMs)
- Current Security Tools: Qualys, Jira for vulnerability tracking, manual IAM reviews
- Key Business Drivers: IPO readiness, rapid product scaling, international expansion into regulated markets
- Known Challenges: CISO mentioned compliance audit findings, legacy code quality issues, wanted to shift security left
- Customer Type: Active opportunity - late-stage evaluation against Prisma Cloud and other vendors

[Insert full prompt from above]
```

**Input:**
```
Create a comprehensive Customer-Specific Strategy with Wiz Alignment Map for Global Bank PLC.

Customer Context:
- Company: Global Bank PLC (Financial Services, regional bank)
- Industry: Banking & Financial Services
- Company Size: 2,500 employees, $750M in managed assets
- Cloud Maturity: Hybrid cloud - 40% AWS, 35% Azure, 25% on-premise
- Primary Cloud Providers: AWS (core systems), Azure (compliance workloads), On-prem (legacy)
- Current Security Tools: ServiceNow, RSA Archer, multiple SIEM tools, fragmented approach
- Key Business Drivers: Digital transformation, open banking initiative, cloud migration by 2027
- Known Challenges: Legacy compliance, multiple auditors (Fed, OCC, third-party), SOC overwhelmed with alerts
- Customer Type: Early-stage prospect from analyst call

[Insert full prompt from above]
```

---

## Key Differences from Vertical/Segment Template

### Original Template (Vertical/Segment)
- Focused on typical patterns across an entire industry vertical
- Market-level analysis and competitive landscape
- Generic buyer personas
- Average metrics and "typical" outcomes
- Go-to-market strategy for a category

### Customer-Specific Template (This Version)
- Focused on THIS specific customer's unique situation
- Customer's actual business context and environment
- Named decision-makers and their specific priorities
- Customer-tailored metrics and realistic outcomes for THEM
- Sales and deal strategy for a specific opportunity

---

## Tips for Best Results

1. **Gather Customer Intelligence First**:
   - Review company website, recent news, SEC filings
   - LinkedIn research on key stakeholders and org structure
   - Research their current tech stack and security tools
   - Look for any public statements about security or compliance priorities

2. **Be Specific About Customer Context**:
   - Include actual company name and relevant context
   - Document what you know about their environment
   - Reference specific conversations or known pain points
   - Include growth stage and financial context

3. **Tailor to Decision-Makers**:
   - Identify actual stakeholders if possible
   - Document their specific priorities and concerns
   - Frame Wiz value in terms that matter to THEM
   - Include realistic concerns they might have

4. **Use Real Customer Data**:
   - Reference their cloud environment (known provider mix)
   - Include their regulatory requirements
   - Document their current tool stack
   - Acknowledge their specific challenges

5. **Build Realistic Business Cases**:
   - Base ROI on their actual team size and maturity
   - Include implementation timeline realistic for them
   - Account for their budget constraints and cycles
   - Factor in their organizational change management needs

6. **Iterate with Sales & Solutions Teams**:
   - Review with account executive for accuracy
   - Get solutions architect input on technical fit
   - Incorporate any recent customer conversations
   - Update as you learn more about the customer

---

## Sample Follow-Up Requests

After generating the customer-specific alignment map, you can ask:

- "Generate discovery call questions for the CISO at [Customer]"
- "Create a technical demo scenario highlighting how Wiz solves [their specific problem]"
- "Develop a competitive battlecard positioning Wiz vs. [competitor] for this customer"
- "Create an ROI calculator for [Customer] based on their specific team size and environment"
- "Generate objection handling scripts for [specific concern raised]"
- "Create a customer success plan for post-sale implementation at [Customer]"
- "Identify potential internal champions and skeptics at [Customer]"
- "Develop a multi-threaded engagement strategy across [Customer]'s stakeholders"
- "Create a reference customer conversation guide for similar companies"
- "Generate a win/loss analysis for why [Customer] chose us (or competitor)"
- "Create a business case presentation deck for [Customer] leadership"
- "Develop a risk mitigation strategy for [specific implementation concern]"

---

## Version History
- v1.0 (October 2025): Customer-specific focus for targeted sales and solution strategy