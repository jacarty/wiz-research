# Merlin GTM Intelligence Brief - Synthesis Prompt 

## Purpose

You will receive THREE comprehensive research reports about a prospect company:
1. **Industry Strategy Map** - Industry trends, regulatory landscape, technology adoption
2. **Company Business Intelligence** - Business strategy, priorities, leadership, challenges  
3. **Tech Stack Discovery** - Verified technology infrastructure and tools

Your task is to synthesize these into a **single 8,000 character GTM Intelligence Brief** optimized for an internal Slackbot that helps sales teams align product use-cases to prospect needs.

---

## Critical Requirements

### CHARACTER TARGET
- **TARGET: 7,500-8,000 characters INCLUDING SPACES**
- **MINIMUM: 7,000 characters INCLUDING SPACES**
- Count ALL characters including spaces before submitting
- Prioritize depth in critical sections over breadth
- If under 7,000 characters, expand key sections (priorities, tech stack, urgency catalysts)

### CORE PHILOSOPHY
**The brief provides detailed "WHAT" - verified facts with context about the prospect.**

### VERIFICATION STANDARD
- **Include information with HIGH or MEDIUM confidence**
- HIGH confidence: Multiple verified sources or authoritative single source
- MEDIUM confidence: Single credible source or strong inference from public data
- Clearly mark MEDIUM confidence items with [MEDIUM] tag
- NO speculation or "likely" statements without evidence
- NO mention of information gaps or unknowns
- NO "NOT FOUND" or "NONE" entries
- If information doesn't meet MEDIUM confidence threshold, omit it entirely
- For tables: include rows where you have HIGH or MEDIUM confidence technology

### FOCUS AREAS
- ✅ Known facts about their business and technology
- ✅ Verified technical environment (tools, platforms, maturity) - include MEDIUM confidence
- ✅ Strategic priorities with context (3 sentences per priority)
- ✅ Compliance requirements that directly apply to them
- ✅ Recent events creating urgency for security/cloud purchases
- ✅ Leadership context for key decision-makers
- ❌ Generic industry trends not specific to this company
- ❌ Information gaps or unknowns
- ❌ Interpretations or implications (let Slackbot determine these)

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
[2-3 sentences: How they make money, primary offerings, target customers]

**Company Structure:**
- Type: [Public/Private/PE-backed]
- Founded: [Year]
- Headquarters: [City, Country]
- Geographic Reach: [UK only/EU/Global with key markets]

**Financial Profile:**
- Annual Revenue: $[X]M ([Fiscal Year])
- Growth Rate: [X]% YoY [if known]
- Employee Count: [X]
- Funding: [Latest round, amount, date if private | Public: Ticker if applicable]

**Cloud Environment:**
- Primary: [AWS/Azure/GCP] with [key services/patterns]
- Multi-cloud: [Yes/No - if yes, list providers]
- Adoption Stage: [Lift-shift/Hybrid/Cloud-native with brief justification]
- Orchestration: [Kubernetes/ECS/AKS/GKE with scale details if known]
- Container Strategy: [Docker/K8s adoption level and maturity]

**Security Posture:**
- Maturity Level: [Early/Developing/Mature - assessment based on tools and practices]
- DevSecOps Integration: [Low/Medium/High with integration points]
- Tool Consolidation: [Fragmented/Partial/Unified]
- Team Size: [If known from LinkedIn/job postings]

---

## STRATEGIC_PRIORITIES

**Top 5-6 Business Priorities:**

### 1. [Priority Name]
[What they're trying to achieve - 3 sentences covering scope, approach, and current status]  
**Timeline:** [If known]  
**Scale:** [Budget/team size if available]

### 2. [Priority Name]
[3 sentences]  
**Timeline:** [If known]  
**Scale:** [If available]

### 3. [Priority Name]
[3 sentences]  
**Timeline:** [If known]  
**Scale:** [If available]

### 4. [Priority Name]
[3 sentences]  
**Timeline:** [If known]

### 5. [Priority Name]
[3 sentences]  
**Timeline:** [If known]

[Include 6th priority if strong evidence exists]

---

## VERIFIED_TECH_STACK

**Note:** HIGH and MEDIUM confidence items only. MEDIUM items marked with [MEDIUM].

### Cloud & Infrastructure
| Category | Technology | Confidence |
|----------|-----------|------------|
| **Cloud Provider(s)** | [AWS/Azure/GCP with key services] | [HIGH/MEDIUM] |
| **Orchestration** | [Kubernetes/ECS/AKS/GKE] | [HIGH/MEDIUM] |
| **IaC** | [Terraform/CloudFormation/Pulumi] | [HIGH/MEDIUM] |
| **CI/CD** | [Jenkins/GitLab CI/GitHub Actions] | [HIGH/MEDIUM] |
| **Version Control** | [GitHub/GitLab/Bitbucket] | [HIGH/MEDIUM] |
| **Container Registry** | [ECR/ACR/GCR] | [HIGH/MEDIUM] |
| **Serverless** | [Lambda/Functions] | [HIGH/MEDIUM] |

### Security Tools (Current Stack)
| Category | Tool | Confidence |
|----------|------|------------|
| **CSPM** | [Tool name] | [HIGH/MEDIUM] |
| **CWPP** | [Tool name] | [HIGH/MEDIUM] |
| **Container Security** | [Tool name] | [HIGH/MEDIUM] |
| **IaC Scanning** | [Tool name] | [HIGH/MEDIUM] |
| **SAST/DAST** | [Tool name] | [HIGH/MEDIUM] |
| **Dependency Scanning** | [Tool name] | [HIGH/MEDIUM] |
| **API Security** | [Tool name] | [HIGH/MEDIUM] |
| **WAF** | [Tool name] | [HIGH/MEDIUM] |
| **SIEM** | [Tool name] | [HIGH/MEDIUM] |
| **EDR/XDR** | [Tool name] | [HIGH/MEDIUM] |
| **Identity/IAM** | [Tool name] | [HIGH/MEDIUM] |
| **Secrets Management** | [Tool name] | [HIGH/MEDIUM] |
| **Vulnerability Management** | [Tool name] | [HIGH/MEDIUM] |

**Only include rows with verified tools. Omit rows if no verified tool.**

### Development Stack
| Category | Technology | Confidence |
|----------|-----------|------------|
| **Primary Languages** | [Python, Java, Go, etc.] | [HIGH/MEDIUM] |
| **Backend Frameworks** | [Django/Spring/Express] | [HIGH/MEDIUM] |
| **Frontend** | [React/Vue/Angular] | [HIGH/MEDIUM] |
| **Mobile** | [Swift/Kotlin/React Native] | [HIGH/MEDIUM] |
| **API** | [REST/GraphQL/gRPC] | [HIGH/MEDIUM] |
| **Testing** | [Jest/Pytest/Selenium] | [HIGH/MEDIUM] |

### Data & Analytics
| Category | Technology | Confidence |
|----------|-----------|------------|
| **Data Warehouse** | [Snowflake/Databricks/BigQuery] | [HIGH/MEDIUM] |
| **ETL/ELT** | [Airflow/dbt/Fivetran] | [HIGH/MEDIUM] |
| **Streaming** | [Kafka/Kinesis/Pub/Sub] | [HIGH/MEDIUM] |
| **Databases** | [PostgreSQL/MySQL/MongoDB] | [HIGH/MEDIUM] |

### Technical Maturity Indicators
- **Cloud-Native:** [Early: Lift-shift | Mid: Hybrid | Advanced: Cloud-native microservices with architectural details]
- **Containers:** [None/Docker only/K8s in prod with scale/patterns]
- **IaC Maturity:** [None/Basic/Advanced with modules & state management]
- **CI/CD:** [Manual/Semi-automated/Fully automated with testing/gates]
- **Security Shift-Left:** [None/Beginning/Integrated with specific tools and automation]
- **Microservices:** [Monolith/Early/Mature with service count or patterns]
- **Observability:** [Tools and maturity level for monitoring/logging/tracing]
- **GitOps:** [None/Exploring/Implemented with tools]

---

## LEADERSHIP_CONTEXT

### [Title - e.g., CISO / CTO / VP Engineering]
**Name:** [Full Name]  
**Tenure:** [Started Month Year]  
**Background:** [2 sentences: Previous companies, relevant experience, achievements]  
**Known Priorities:** [2-3 focus areas from LinkedIn/interviews/job postings]

### [Title 2]
**Name:** [Full Name]  
**Tenure:** [Started Month Year]  
**Background:** [2 sentences]  
**Known Priorities:** [2-3 focus areas]

[Include 2-3 key technical/security leaders]

**Org Structure:**
- Security reports to: [CTO/CIO/CEO/CISO]
- Engineering team: [Size if known]
- Security team: [Size if known]
- Recent changes: [CISO/CTO/VP Eng changes in last 12 months]

---

## REGULATORY_CONTEXT

### [Framework 1: e.g., FCA Operational Resilience]
- **Applicability:** [Why this applies to them - 2 sentences]
- **Key Requirements:** [3-4 bullets focused on security/cloud]
- **Timeline:** [Audit frequency/next audit if known]
- **Urgency:** [Recent enforcement/upcoming deadlines]

### [Framework 2: e.g., GDPR]
- **Applicability:** [2 sentences]
- **Key Requirements:** [3-4 bullets]
- **Timeline:** [If known]

### [Framework 3: e.g., SOC 2/ISO 27001]
- **Applicability:** [2 sentences]
- **Key Requirements:** [3-4 bullets]
- **Status:** [Certified/In progress/Required]

[Include 2-4 frameworks if applicable]

**Upcoming Changes:**
- **[Regulation]:** [2-3 sentences: what's changing, effective date, impact, penalties]

---

## RECENT_URGENCY_CATALYSTS

**Events in Last 12 Months:**

### [Event Type: M&A / Funding / Leadership / Incident / Compliance / Launch]
- **Date:** [Month Year]
- **Description:** [3-4 sentences covering context, scale, infrastructure/security implications, and current status]
- **Impact:** [Known impacts on operations, security priorities, or tech investments]
- **Timeline:** [Deadlines or milestones created by this event]

### [Event 2]
- **Date:** [Month Year]
- **Description:** [3-4 sentences]
- **Impact:** [Details]
- **Timeline:** [If applicable]

### [Event 3]
- **Date:** [Month Year]
- **Description:** [3-4 sentences]
- **Impact:** [Details]

[Include 3-4 events - prioritize security/cloud/infrastructure relevance]

---

## MARKET_POSITION

**Competitive Landscape:**
- Competitors: [2-3 direct competitors]
- Position: [Leader/Challenger/Niche]
- Differentiation: [Key differentiators relevant to tech/security]

**Growth Trajectory:**
- Phase: [Startup/Scale-up/Mature/Enterprise]
- Expansion: [Geographic/product plans relevant to infrastructure]
- Customer Base: [Enterprise/Mid-market/SMB - impacts security needs]

---

**CHARACTER COUNT: [X/8,000]** ← TARGET: 7,500-8,000 INCLUDING SPACES (MIN: 7,000)

---

# END OF OUTPUT

---

## Synthesis Instructions

### 1. COMPANY_SNAPSHOT
- Pull from Business Intelligence Report (4.1) and Tech Stack Discovery (5.1)
- Keep concise but informative
- Provide 2-3 sentences for business model
- Expand cloud environment and security posture with specific details

### 2. STRATEGIC_PRIORITIES
- Extract from Business Intelligence Report (2.1, 2.2, 4.3, 4.4)
- **3 sentences per priority** covering scope and approach
- Include 5-6 priorities
- Add timeline and scale if available
- NO citations

### 3. LEADERSHIP_CONTEXT
- Extract from Business Intelligence Report
- Include 2-3 key technical/security leaders
- 2 sentences for background
- 2-3 known priorities per leader
- Keep org structure concise
- NO citations

### 4. VERIFIED_TECH_STACK
- Pull HIGH and MEDIUM confidence from Tech Stack Discovery (5.1-5.5)
- **Mark MEDIUM items with [MEDIUM]**
- Only include rows with verified tools (omit empty rows)
- Expand technical maturity indicators with specific patterns
- NO citations in tables

### 5. REGULATORY_CONTEXT
- Pull from Industry Strategy Map (4) and Business Intelligence (4)
- 2 sentences for applicability
- 3-4 bullets for key requirements
- Include 2-4 frameworks
- Keep upcoming changes to 2-3 sentences
- NO citations

### 6. RECENT_URGENCY_CATALYSTS
- Pull from Business Intelligence Report (4.4)
- **3-4 sentences per event** with context
- Include 3-4 events from last 12 months
- Focus on security/cloud/infrastructure relevance
- NO citations

### 7. MARKET_POSITION
- Keep brief but informative
- Relevant to understanding maturity and needs
- NO citations

### 8. CHARACTER MANAGEMENT
**Target 7,500-8,000 characters INCLUDING SPACES:**
- Prioritize depth in: Priorities, Tech Stack, Urgency Catalysts
- Keep concise: Company Snapshot, Market Position
- Balance detail across all sections
- **If under 7,000, expand:**
  1. Add 6th priority
  2. Add 4th urgency catalyst
  3. Expand technical maturity indicators
  4. Add more detail to leadership backgrounds
- **If over 8,000, trim:**
  1. Remove 6th priority if exists
  2. Reduce regulatory frameworks to 2-3
  3. Reduce urgency catalysts to 3
  4. Tighten language throughout

### 9. Quality Checks

**Verify:**
- [ ] Character count INCLUDING SPACES is 7,000-8,000 (aim for 7,500+)
- [ ] MEDIUM items marked with [MEDIUM]
- [ ] Tech stack tables: Technology and Confidence columns only
- [ ] Only verified tool rows included (no "NONE" rows)
- [ ] No gaps or unknowns mentioned
- [ ] NO citations anywhere
- [ ] 3 sentences per priority
- [ ] 3-4 sentences per urgency catalyst
- [ ] 2-3 key leaders included
- [ ] 2-4 regulatory frameworks
- [ ] Structured exactly as template

**Synthesize the three source reports into this format, targeting 7,500-8,000 characters (including spaces) with NO citations.**
**Markdown format output**