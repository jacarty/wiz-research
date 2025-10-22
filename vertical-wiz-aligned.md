# Vertical & Segment Strategy with Wiz Alignment Map Generator

## How to Use
This prompt generates a strategic alignment document that maps common business objectives for a specific **industry vertical and market segment** to Wiz.io's cloud security platform capabilities. It prioritizes typical strategies within that vertical/segment first, then shows where and how Wiz products provide value.

Use this for market analysis, go-to-market planning, sales enablement, and understanding how Wiz serves different verticals and segments.

---

## Prompt Template

```
Create a comprehensive Vertical & Segment Strategy with Wiz Alignment Map for the [INDUSTRY VERTICAL] industry, focusing on [SEGMENT] companies.

Examples:
- "Healthcare Technology industry, focusing on Series B-D SaaS companies"
- "Financial Services industry, focusing on mid-market banks and credit unions"
- "E-commerce industry, focusing on high-growth retailers ($50M-$500M ARR)"
- "Manufacturing industry, focusing on Fortune 1000 industrial companies"

This document should be structured to prioritize TYPICAL strategic objectives for companies in this vertical/segment first, then demonstrate how Wiz.io's Cloud Security Platform (Wiz Code, Wiz Cloud, and Wiz Defend) aligns with and enables those objectives.

---

## PART 1: VERTICAL & SEGMENT PROFILE

### Market Overview & Landscape

Provide a high-level overview of the vertical to set the scene:
- **Market Size & Growth**: Current market size, growth rate, and projections
- **Key Market Dynamics**: Major forces shaping the industry
- **Competitive Landscape**: Number of players, market concentration, notable leaders
- **Investment & Funding Trends**: VC activity, M&A patterns, valuations
- **Technology Adoption Patterns**: Cloud-first adoption rates, innovation cycles
- **Economic & Geopolitical Factors**: Macro trends affecting the vertical
- **Recent Notable Events**: Security incidents, regulatory changes, market shifts that matter

### Industry Vertical Characteristics
- Primary industry vertical and sub-sectors
- Typical regulatory environment and compliance frameworks
- Industry-specific security challenges and threat landscape
- Market trends and competitive pressures
- Digital transformation drivers

### Market Segment Profile
- Company size range (employees, revenue)
- Growth stage (startup, growth, mature enterprise)
- Typical cloud maturity level (cloud-native, hybrid, migrating)
- Common cloud providers used (AWS, Azure, GCP, multi-cloud patterns)
- Development velocity patterns (release cadence, engineering team size)
- Organizational structure norms (centralized vs. distributed security)

### Common Current State Patterns
- **Cloud Security Posture**: Typical challenges and gaps in this segment
- **Development Practices**: Prevalent CI/CD maturity and DevSecOps adoption levels
- **Security Operations**: Common SOC capabilities and incident response maturity
- **Compliance Requirements**: Standard regulations and certifications required
- **Legacy Security Tools**: Existing tool sets typically in place

---

## PART 2: TYPICAL BUSINESS GOALS & STRATEGIC PRIORITIES

For each major business goal common to this vertical/segment (aim for 4-6 goals), structure as follows:

### Goal [X]: [Common Business Objective for this Vertical/Segment]
*High-level strategic objective that companies in this vertical/segment typically pursue*

#### Business Context (Target: 100-150 words)
- Why this goal matters to companies in this vertical/segment
- Common pain points or blockers faced
- Typical success criteria and what "good" looks like
- Urgency factors and market drivers

#### Strategic Approaches (Target: 3-4 bullet points)
List 3-4 strategic approaches companies in this segment commonly take to achieve this goal

#### Wiz Alignment Assessment

**Directly Aligned Capabilities**
- **Primary Wiz Product(s)**: Which Wiz product(s) directly address this goal
- **Key Features**: Specific Wiz capabilities that enable this objective
- **Value Delivery**: How Wiz accelerates or enables this goal for companies in this segment

**Typical Outcomes Enabled**
- Quantifiable improvements commonly seen (time savings, risk reduction, coverage increase)
- Operational efficiencies typically gained
- Competitive advantages unlocked

**Success Metrics & KPIs**
List 5-8 measurable indicators with realistic target values based on this segment. Use format: **Metric Name**: Baseline → Target (timeframe) when applicable:
- Deployment metrics (e.g., **Time to Full Visibility**: 2-3 weeks → <24 hours)
- Operational metrics (e.g., **MTTR**: 48 hours → 5 hours [70% reduction])
- Coverage metrics (e.g., **Cloud Asset Visibility**: 60% → 100%)
- Efficiency metrics (e.g., **Security Issue Remediation Speed**: 10x faster)
- Business impact metrics (e.g., **Critical Security Incidents**: 5/quarter → <1/quarter)

---

## PART 3: BUSINESS FUNCTION ALIGNMENT

Focus on the three core business functions most relevant to Wiz deployment. For each function, describe **typical patterns** for this vertical/segment:

### Security Operations (SecOps)
**Primary Wiz Product**: Wiz Defend

**Common Initiatives in this Segment**:
- List 5-7 typical SecOps initiatives that companies in this segment prioritize
- Examples: Real-time threat detection, incident response automation, threat hunting
- Consider segment-specific patterns (e.g., 24/7 SOC vs. business hours coverage)

**Key Capabilities Provided**:
- Runtime threat detection with eBPF sensors
- Cloud-native anomaly detection
- Investigation and response automation
- Cross-layer visibility (runtime, identity, data, network)

**Typical Metrics & Outcomes for this Segment**:
- Detection speed improvements commonly achieved
- Alert noise reduction percentages typical for segment
- MTTR reduction benchmarks
- Investigation time savings
- Incident readiness improvements

---

### Cloud Security / Infrastructure Security
**Primary Wiz Product**: Wiz Cloud

**Common Initiatives in this Segment**:
- List 5-7 typical cloud security initiatives that companies in this segment prioritize
- Examples: Cloud security posture management, attack path analysis, compliance automation
- Consider segment-specific cloud adoption patterns

**Key Capabilities Provided**:
- Agentless multi-cloud visibility
- Wiz Security Graph for risk prioritization
- Misconfiguration detection
- Vulnerability management with business context
- Attack path visualization

**Typical Metrics & Outcomes for this Segment**:
- Cloud coverage percentages achievable
- Critical risk reduction rates seen
- Time to identify misconfigurations
- Compliance audit readiness improvements
- False positive reduction typical for segment

---

### Application Development / DevSecOps
**Primary Wiz Product**: Wiz Code

**Common Initiatives in this Segment**:
- List 5-7 typical development security initiatives that companies in this segment prioritize
- Examples: Shift-left security, secure CI/CD pipelines, code-to-cloud traceability
- Consider segment-specific development velocity and maturity patterns

**Key Capabilities Provided**:
- IDE and PR-level security feedback
- IaC scanning and misconfiguration prevention
- Secrets detection and remediation
- Software composition analysis (SCA)
- Supply chain security hardening
- Code-to-cloud mapping and drift detection

**Typical Metrics & Outcomes for this Segment**:
- Developer remediation speed improvements
- Pre-production issue detection rate increases
- Security debt reduction patterns
- Developer productivity impact benchmarks
- Secure deployment velocity improvements

---

### Cross-Functional: Risk & Compliance
**Wiz Products**: All three products (Code, Cloud, Defend)

**Common Initiatives in this Segment**:
- Typical compliance and risk management priorities
- Segment-specific regulatory requirements
- Audit preparation patterns
- Risk quantification approaches

**Key Capabilities Provided**:
- Built-in compliance frameworks relevant to this vertical (CIS, NIST, PCI-DSS, HIPAA, etc.)
- Automated evidence collection
- Executive risk dashboards
- Compliance mapping to security findings

**Typical Metrics & Outcomes for this Segment**:
- Audit preparation time reduction benchmarks
- Compliance score improvement patterns
- Policy violation detection rates
- Risk reporting efficiency gains

---

## PART 4: STRATEGIC AREAS OUTSIDE WIZ SCOPE

### Explicitly Out of Scope
List business functions and strategic areas where Wiz does NOT provide direct value:
- Traditional endpoint security (desktop/laptop protection)
- Email security and phishing prevention
- Network perimeter security (traditional firewalls)
- Physical security and access control
- HR security awareness training programs
- Financial security controls and fraud detection
- Non-cloud infrastructure security (on-premises data centers)
- Application performance monitoring (APM)
- General IT service management (ITSM)

### Adjacent Capabilities (Partial Coverage)
List areas where Wiz provides some value but may require complementary tools:
- SIEM integration (Wiz feeds data but isn't a SIEM replacement)
- Identity and Access Management (Wiz detects issues but doesn't manage identities)
- Data Loss Prevention (Wiz identifies sensitive data exposure but isn't full DLP)
- Container security in non-cloud environments

---

## PART 5: UNIFIED PLATFORM VALUE FOR THIS SEGMENT

### Breaking Down Silos (Common in this Segment)
Explain how Wiz enables collaboration across teams typical in this vertical/segment:
- Security Operations ↔ Cloud Security ↔ Development teams
- Shared context via code-to-cloud traceability
- Single source of truth for security decisions
- How this addresses typical organizational challenges in this segment

### Typical Consolidation Opportunities
List traditional tools commonly used in this segment that Wiz can replace or consolidate:
- First-generation CSPM tools
- Standalone vulnerability scanners
- Separate container security tools
- Disparate SAST/DAST tools for cloud
- Multiple cloud-native security point solutions
- Segment-specific tool sprawl patterns

### Strategic Advantages for this Segment
- Multi-cloud consistency (AWS, Azure, GCP, Kubernetes)
- Agentless architecture benefits relevant to this segment
- Graph-based risk correlation value for typical complexity
- Developer-friendly security aligned with segment velocity
- Scalability patterns matching segment growth trajectories

---

## PART 6: SOURCES & REFERENCES

Organize sources for maximum usefulness. Consider grouping by topic (e.g., "Regulatory Guidance", "Threat Intelligence", "Market Analysis") in addition to or instead of source type.

### Industry & Market Research Sources
List credible sources used to inform the vertical/segment analysis:
- Industry reports (Gartner, Forrester, IDC, etc.)
- Market research and analyst publications
- Industry trade publications and associations
- Relevant statistics and market sizing data
- Include publication dates and URLs where available
- Consider organizing by subtopic (Market Size, Competitive Analysis, Technology Trends, etc.)

### Wiz Product Documentation & Resources
List official Wiz resources referenced:
- Wiz product documentation pages
- Wiz blog posts and case studies
- Wiz customer testimonials (with company names if public)
- Wiz Security Graph and methodology references
- Integration and capability documentation

### Compliance & Regulatory References
List relevant compliance frameworks and regulatory sources:
- Industry-specific regulations (HIPAA, PCI-DSS, SOC 2, etc.)
- Government and regulatory body publications
- Compliance framework documentation
- Security standards and best practices (NIST, CIS, etc.)

### Customer Case Studies & Testimonials
List Wiz customer examples from this vertical/segment (if available):
- Company name, vertical, and segment
- Specific outcomes achieved
- Quotes or testimonials
- Link to case study or review

### Additional Reading & Resources
Suggest further reading for deeper understanding:
- Wiz whitepapers relevant to this vertical
- Industry-specific security best practices
- Cloud security trends and research
- Competitive analysis and market positioning

---

## FORMATTING REQUIREMENTS

- Use clear headers and subheaders with proper hierarchy
- Lead with TYPICAL BUSINESS GOALS for the segment before Wiz capabilities
- Be specific and quantitative with metrics (avoid generic statements)
- Include realistic, measurable KPI targets based on Wiz customer testimonials from similar segments
- Make it actionable for both business and technical stakeholders in this vertical/segment
- Use segment-appropriate language and terminology
- Provide concrete examples specific to the industry vertical
- Clearly distinguish between what Wiz does and doesn't address
- Include industry-specific use cases and scenarios
- **Cite all sources with URLs where possible for verification and further reading**
- **Include publication dates for time-sensitive information**
- **Link to official Wiz documentation and case studies**

---

## DOCUMENT TONE & PERSPECTIVE

This document should be written from a **market analysis and consultative perspective** that:
- Demonstrates understanding of typical business priorities in this vertical/segment
- Shows how Wiz enables common strategic objectives (not just features)
- Acknowledges what Wiz doesn't do (builds credibility)
- Uses vertical-specific examples and use cases
- Balances technical depth with business value
- Positions Wiz as an enabler of typical strategies in this segment
- Provides insights useful for go-to-market planning and sales enablement
- Helps identify ideal customer profiles (ICP) within the segment
- **Maintains research rigor with proper source attribution**
- **Enables readers to verify claims and explore topics further**
- **Builds trust through transparency about information sources**

---

Please create a detailed, professional document that would be valuable for:
- Market analysis and vertical go-to-market planning
- Sales enablement and competitive positioning
- Solution architecture and implementation planning
- Executive presentations to prospects in this segment
- Understanding typical buyer personas and their priorities
- ROI modeling and business case development for this segment
- **Due diligence and fact-checking by internal stakeholders**
- **Further research and deep-dive analysis by readers**
```

---

## Example Usage

**Input:**
```
Create a comprehensive Vertical & Segment Strategy with Wiz Alignment Map for the Healthcare Technology industry, focusing on Series B-D SaaS companies (100-500 employees, $20M-$100M ARR).
[Insert full prompt from above]
```

**Input:**
```
Create a comprehensive Vertical & Segment Strategy with Wiz Alignment Map for the Financial Services industry, focusing on regional banks and credit unions ($500M-$5B in assets).
[Insert full prompt from above]
```

**Input:**
```
Create a comprehensive Vertical & Segment Strategy with Wiz Alignment Map for the E-commerce industry, focusing on high-growth direct-to-consumer retailers with $50M-$500M in annual revenue.
[Insert full prompt from above]
```

**Input:**
```
Create a comprehensive Vertical & Segment Strategy with Wiz Alignment Map for the Manufacturing industry, focusing on Fortune 1000 industrial companies undergoing digital transformation.
[Insert full prompt from above]
```

---

## Tips for Best Results

1. **Be Specific About the Vertical and Segment**:
   - Include both industry vertical AND segment definition
   - Example: "Mid-market fintech companies (Series B-C, 200-800 employees, $30M-$150M ARR)"
   - Include growth stage, size range, and maturity indicators

2. **Specify Segment Characteristics When Known**:
   - Cloud adoption patterns: "typically multi-cloud (AWS primary, Azure secondary)"
   - Regulatory context: "subject to SOC 2, PCI-DSS, and state privacy laws"
   - Development culture: "agile teams with 2-week sprints, 50-100 developers"

3. **Focus on Business Outcomes**:
   - Request emphasis on ROI and business impact typical for the segment
   - Example: "Focus on time-to-market improvements for rapid-growth companies"

4. **Request Specific Sections**:
   - "Emphasize compliance requirements specific to healthcare"
   - "Include detailed threat landscape analysis for this segment"
   - "Focus on multi-cloud strategy patterns common in this vertical"

5. **Request Comprehensive Sources**:
   - "Include analyst reports and industry research sources"
   - "Cite all Wiz case studies and customer testimonials used"
   - "Provide URLs for all compliance frameworks and regulations mentioned"
   - "Link to relevant Wiz documentation and product pages"

6. **Iterate and Refine**:
   - "Expand on typical tool consolidation opportunities for mid-market"
   - "Add more segment-specific metrics for SecOps maturity"
   - "Include buyer persona mapping for this vertical"

---

## Sample Follow-Up Requests

After generating the initial alignment map, you can ask:

- "Create an executive summary for this vertical/segment suitable for leadership review"
- "Extract typical ROI metrics and create a segment-specific business case template"
- "Create a competitive comparison showing Wiz vs. traditional tools common in this vertical"
- "Generate typical buyer personas (CISO, VP Engineering, etc.) for this segment"
- "Add a section on change management patterns common in this vertical"
- "Create a one-page visual showing typical customer goals and Wiz product mapping"
- "Develop a qualification framework for identifying ideal customers in this segment"
- "Add win/loss analysis patterns for this vertical"
- "Include typical objection handling for this segment"
- **"Expand the sources section with more analyst reports and market research"**
- **"Find and cite additional Wiz customer testimonials from this vertical"**
- **"Add links to relevant compliance framework documentation"**
- **"Include industry association resources and reports"**
- **"Create detailed buyer persona profiles (CISO, Head of Engineering, Compliance Manager) with priorities, pain points, and typical objections"**
- **"Generate a discovery call question framework based on the identified pain points"**
- **"Develop a demo scenario script using the attack path example from Part 5"**

---

## Output Format Options

You can request the output in different formats:

- **Markdown document** (default) - for detailed review and analysis
- **Slide deck outline** - structured for sales enablement presentations
- **Executive summary** - 2-page vertical overview for leadership
- **Visual strategy map** - diagram showing segment patterns and Wiz alignment
- **Playbook format** - tactical guide for selling into this segment
- **Competitive battlecard** - positioning against alternatives in this vertical
- **ICP definition** - ideal customer profile characteristics
- **Buyer persona guide** - decision-maker profiles and priorities
- **Research bibliography** - annotated list of sources with summaries
- **Visual strategy diagram** - suggested: (1) Market landscape map showing segment position, (2) Goal-to-Product mapping flowchart, (3) Attack path scenario illustration

---

## Version History
- v1.0 (October 2025): Refocused on vertical/segment analysis rather than individual customer strategy