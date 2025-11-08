# Merlin GTM Intelligence Brief - Synthesis Prompt

## Purpose

You will receive THREE comprehensive research reports about a prospect company:
1. **Industry Strategy Map** - Industry trends, regulatory landscape, technology adoption
2. **Company Business Intelligence** - Business strategy, priorities, leadership, challenges  
3. **Tech Stack Discovery** - Verified technology infrastructure and tools

Your task is to synthesize these into a **single 10,000 character GTM Intelligence Brief** optimized for an internal Slackbot that helps sales teams align product use-cases to prospect needs.

---

## Slackbot Context

The Slackbot:
- Is built on Gemini with RAG capabilities
- Has access to all internal product documentation, roadmap, and use-case library
- Has access to company GDrive and Slack history
- Will generate custom use-case recommendations by combining prospect context (your output) with product capabilities (its existing knowledge)
- Needs to understand: prospect's business priorities, technology environment, and key stakeholders
- Does NOT need: information gaps, discovery questions, or unknowns

---

## Critical Requirements

### CHARACTER LIMIT
- **MAXIMUM 10,000 characters** (strict limit - 2,000 chars reserved for Slackbot prompt)
- Count characters before submitting
- If over limit, trim in this order:
  1. Reduce regulatory context detail
  2. Condense business priorities descriptions
  3. Reduce stakeholder background details
  4. NEVER reduce: company snapshot, verified tech stack, or use-case opportunities

### CORE PHILOSOPHY
**The brief provides only the "WHAT" - verified facts about the prospect.**

The Slackbot will:
- Understand the "WHY" (context and implications)
- Provide the "HOW" (solutions using product knowledge via RAG)

### VERIFICATION STANDARD
- **Include ONLY verified information with HIGH confidence**
- NO speculation, assumptions, or "likely" statements
- NO mention of information gaps or unknowns
- NO "NOT FOUND" or "NONE" entries
- If information doesn't meet HIGH confidence threshold, simply omit it entirely
- For tables: only include rows where you have verified technology

### FOCUS AREAS
- ✅ Known facts about their business and technology
- ✅ Verified technical environment (tools, platforms, maturity)
- ✅ Strategic priorities (state the priority, not why it matters)
- ✅ Compliance requirements that directly apply to them
- ✅ Recent events creating urgency for security/cloud purchases
- ❌ Generic industry trends
- ❌ Information gaps or unknowns
- ❌ Interpretations or implications (let Slackbot determine these)
- ❌ Speculative information

---

## Output Structure

Deliver in this exact format:

---

# GTM_BRIEF: [Company Name]

**Last Updated:** [Research Date]  
**Industry:** [Specific vertical]  
**Company Size:** [X] employees | $[Y]M revenue  
**Primary Cloud:** [AWS/Azure/GCP/Multi-cloud]  
**Security Maturity:** [Early/Developing/Mature]

---

## COMPANY_SNAPSHOT

**Business Model:**
[1-2 sentences: How they make money, primary offerings]

**Company Structure:**
- Type: [Public/Private/PE-backed]
- Founded: [Year]
- Headquarters: [City, Country]
- Geographic Reach: [UK only/EU/Global]

**Financial Profile:**
- Annual Revenue: $[X]M ([Fiscal Year])
- Growth Rate: [X]% YoY
- Employee Count: [X] ([Source: LinkedIn/Companies House])
- Funding: [Latest round, amount, date if private | Public: Ticker if applicable]

**Cloud Environment:**
- Primary: [AWS/Azure/GCP] ([Evidence: case study/blog/job postings])
- Multi-cloud: [Yes/No - if yes, list secondary providers]
- Adoption Stage: [Lift-shift/Hybrid/Cloud-native]
- Orchestration: [Kubernetes/ECS/Other/Unknown]

**Security Posture:**
- Maturity Level: [Early/Developing/Mature - based on tools and practices]
- DevSecOps Integration: [Low/Medium/High]
- Tool Consolidation: [Fragmented/Partial/Unified]

---

## STRATEGIC_PRIORITIES

**Top 5 Business Priorities:**

### 1. [Priority Name]
**Description:** [What they're trying to achieve - 2-3 sentences]  
**Evidence:** [Source: earnings call/annual report/CEO statement/job postings]  
**Timeline:** [Timeframe if known: Q2 2025, ongoing, etc.]

### 2. [Priority Name]
**Description:** [What they're trying to achieve]  
**Evidence:** [Source]  
**Timeline:** [If known]

### 3. [Priority Name]
**Description:** [What they're trying to achieve]  
**Evidence:** [Source]  
**Timeline:** [If known]

### 4. [Priority Name]
**Description:** [What they're trying to achieve]  
**Evidence:** [Source]  
**Timeline:** [If known]

### 5. [Priority Name]
**Description:** [What they're trying to achieve]  
**Evidence:** [Source]  
**Timeline:** [If known]

---

## VERIFIED_TECH_STACK

**Note:** Only HIGH confidence verified tools included. If a category has no verified tool, the row is omitted entirely.

### Cloud & Infrastructure
| Category | Technology | Evidence Source |
|----------|-----------|-----------------|
| **Cloud Provider(s)** | [AWS/Azure/GCP] | [Blog post/Case study/Job postings] |
| **Orchestration** | [Kubernetes/ECS/AKS/GKE] | [Engineering blog/Job postings] |
| **IaC** | [Terraform/CloudFormation/Pulumi] | [Job postings/GitHub repos] |
| **CI/CD** | [Jenkins/GitLab CI/GitHub Actions/CircleCI] | [Job postings/Blog] |
| **Version Control** | [GitHub/GitLab] | [Public repos/Job postings] |

### Security Tools (Current Stack)
| Category | Tool | Evidence Source |
|----------|------|-----------------|
| **CSPM** | [Tool name] | [Vendor case study/Job posting] |
| **CWPP** | [Tool name] | [Source] |
| **Container Security** | [Tool name] | [Source] |
| **IaC Scanning** | [Tool name] | [Source] |
| **SAST/DAST** | [Tool name] | [Source] |
| **API Security** | [Tool name] | [Source] |
| **SIEM** | [Tool name] | [Source] |
| **Secrets Management** | [Tool name] | [Source] |

**Important:** Only include table rows where you have HIGH confidence verified tools. If no tool is verified for a category, simply omit that row from the table.

### Development Stack
| Category | Technology | Evidence Source |
|----------|-----------|-----------------|
| **Primary Languages** | [Python, Java, Go, etc.] | [Job postings/GitHub] |
| **Frontend** | [React/Vue/Angular] | [Job postings/Blog] |
| **Mobile** | [Swift/Kotlin/React Native] | [Job postings] |
| **Data/ML** | [Python/R/Scala + frameworks] | [Job postings/Blog] |

### Business Applications
| Category | Application | Evidence Source |
|----------|-------------|-----------------|
| **CRM** | [Salesforce/HubSpot/etc.] | [Case study/Job postings] |
| **Collaboration** | [Slack/Teams/Google Workspace] | [Job postings/Website] |
| **Project Mgmt** | [Jira/Asana/Linear] | [Job postings] |
| **Data Warehouse** | [Snowflake/Databricks/BigQuery] | [Case study/Job postings] |

### Technical Maturity Indicators
- **Cloud-Native Adoption:** [Early: Lift-shift | Mid: Hybrid | Advanced: Cloud-native microservices]
- **Container Adoption:** [None/Docker only/Kubernetes in production]
- **IaC Maturity:** [None/Basic/Advanced with modules & state management]
- **CI/CD Integration:** [Manual/Semi-automated/Fully automated pipelines]
- **Security Shift-Left:** [None/Beginning/Integrated in pipelines]

---

## REGULATORY_CONTEXT

**Applicable Compliance Frameworks (Verified Only):**

### [Framework Name 1: e.g., FCA Operational Resilience]
- **Applicability:** [Why this applies to them specifically]
- **Key Requirements:** [Most relevant security/cloud requirements - 2-3 bullets]
- **Audit Timeline:** [If known - annual, bi-annual]
- **Urgency Drivers:** [Recent enforcement, upcoming deadlines]

### [Framework Name 2: e.g., GDPR]
- **Applicability:** [Why this applies]
- **Key Requirements:** [Security/cloud relevant items]
- **Audit Timeline:** [If known]

### [Framework Name 3: e.g., SOC 2, ISO 27001, PCI-DSS]
- **Applicability:** [Why needed]
- **Current Status:** [Certified/In progress/Required for customer contracts]

**Industry-Specific Security Obligations:**
- [Specific requirement 1 relevant to their vertical]
- [Specific requirement 2]

**Upcoming Regulatory Changes:**
- **[Regulation]:** [Brief description, effective date, impact on security/cloud]

---

## RECENT_URGENCY_CATALYSTS

**Events in Last 12 Months Related to Security/Cloud:**

### [Event Type: M&A / Funding / Leadership Change / Security Incident / Compliance Deadline / Product Launch]
- **Date:** [Month Year]
- **Description:** [What happened - 2-3 sentences]
- **Evidence:** [Press release/News article/Company announcement]

### [Event 2]
- **Date:** [Month Year]
- **Description:** [What happened]
- **Evidence:** [Source]

### [Event 3 if applicable]
- **Date:** [Month Year]
- **Description:** [What happened]
- **Evidence:** [Source]

**Note:** Only include events from last 12 months that relate to security, cloud, compliance, or infrastructure.

---

**CHARACTER COUNT: [X/10,000]** ← MUST BE ≤10,000

---

# END OF OUTPUT

---

## Synthesis Instructions

When creating this brief from the three source reports:

### 1. COMPANY_SNAPSHOT
- Pull company basics from Business Intelligence Report (Section 4.1)
- Pull cloud environment from Tech Stack Discovery (Section 5.1)
- Assess security maturity by looking at verified tools in Tech Stack Discovery (Section 5.4)
- Keep concise - this is quick reference info

### 2. STRATEGIC_PRIORITIES
- Extract from Business Intelligence Report (Sections 2.1, 2.2, 4.3, 4.4)
- State the priority clearly - what they're trying to achieve
- Include evidence source and timeline if known
- Do NOT interpret why it matters or how security relates - just state the priority
- The Slackbot will determine relevance to security/cloud
- Include up to 5 priorities

### 3. VERIFIED_TECH_STACK
- Pull ONLY HIGH confidence items from Tech Stack Discovery (Section 5.1-5.5)
- If confidence is MEDIUM or LOW, do not include
- **CRITICAL:** Only include table rows where you have verified tools
- If no tool is verified for a category (e.g., CSPM), simply omit that entire row from the table
- Do NOT use "NONE" or "Not found" - just leave those rows out
- Include the evidence source for transparency
- Technical maturity comes from patterns across verified tools

### 4. REGULATORY_CONTEXT
- Pull from Industry Strategy Map (Section 4) AND Business Intelligence Report (Section 4)
- Include only regulations that verifiably apply to THIS company
- Focus on security-relevant compliance requirements
- Mention upcoming deadlines or recent enforcement if relevant
- Keep brief - Slackbot doesn't need full regulatory details

### 5. RECENT_URGENCY_CATALYSTS
- Pull from Business Intelligence Report (Section 4.4)
- Include ONLY events from last 12 months
- Filter for events related to security, cloud, compliance, or infrastructure:
  - ✅ M&A (acquisition or being acquired)
  - ✅ New CISO/CTO/security leadership
  - ✅ Funding rounds
  - ✅ Security incidents (if public)
  - ✅ Compliance deadlines or regulatory actions
  - ✅ Major product launches requiring infrastructure
  - ✅ Cloud migrations announced
  - ❌ General business updates without tech/security angle
- State what happened - do NOT interpret implications or urgency
- The Slackbot will determine how these events create opportunities

### 5. CHARACTER MANAGEMENT
**If approaching 10,000 character limit, trim in this priority order:**
1. Reduce detail in REGULATORY_CONTEXT (keep it to 2-3 frameworks max)
2. Condense STRATEGIC_PRIORITIES descriptions (tighten language)
3. Limit RECENT_URGENCY_CATALYSTS to top 2-3 events
4. Reduce Technical Maturity Indicators detail in VERIFIED_TECH_STACK
5. **NEVER trim:** COMPANY_SNAPSHOT core facts, VERIFIED_TECH_STACK tables

### 6. Quality Checks Before Submission

**Verify:**
- [ ] Character count is ≤10,000
- [ ] All tech stack items are HIGH confidence only
- [ ] Tech stack tables only include rows with verified tools (no "NONE" or blank rows)
- [ ] No "gaps" or "unknowns" mentioned anywhere
- [ ] Priorities stated as facts without interpretation of relevance
- [ ] Recent events stated as facts without implication analysis
- [ ] No speculation or "likely" statements
- [ ] Evidence sources noted where helpful but kept minimal
- [ ] Structured exactly as template (AI-parseable format)
- [ ] Brief provides only "WHAT" - no "WHY" or "HOW"

---

## Slackbot Usage Note

The Slackbot will use this brief to:
- Understand the prospect's business context and priorities
- Know their verified technology stack and maturity
- Generate custom use-case recommendations by combining this context with internal product documentation via RAG
- Align product capabilities to their specific needs

The brief provides the "what" and "why" - the Slackbot provides the "how" using product knowledge.

---

## Example Use-Case Generation (for understanding only - NOT in output)

## Example: How Slackbot Uses This Brief

**Scenario:** Sales rep asks "What use-cases should I discuss with this prospect?"

**Slackbot Process:**
1. Reads STRATEGIC_PRIORITIES: "Priority #1: Reduce cloud costs by 15% while scaling to 10M customers"
2. Reads VERIFIED_TECH_STACK: "AWS primary + Azure, Kubernetes on EKS, no CSPM found"
3. Uses RAG to pull relevant product capabilities from internal docs
4. Generates recommendation: "Multi-cloud security posture management use-case aligns to their cost reduction priority. They have multi-cloud without CSPM, creating visibility gaps and potential waste. Our product can provide unified visibility, misconfiguration detection, and cost optimization insights."

The brief gives Slackbot the prospect context. The Slackbot adds the product solution.

---

**Now synthesize the three source reports into this format, staying within 10,000 characters.**