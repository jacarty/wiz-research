# Tech Stack Discovery & Verification

## Objective
Conduct thorough research to identify and verify a customer's technology infrastructure, security tools, cloud environment, programming languages, and applications. Provide only sourced information and explicitly flag gaps in knowledge.

## Input Required
- **Customer name and domain**
- **Optional context**: Industry, size, region (helps focus research)

## Research Process

### Phase 1: Public Signal Collection
Search for verified technology indicators:
1. **Engineering blogs & tech publications** (highest confidence)
2. **Job postings** (active tech requirements)
3. **Company careers pages** (required skills = current stack)
4. **Conference talks & presentations** (teams discussing their tools)
5. **Case studies from vendors** (confirmed tool usage)
6. **GitHub repositories** (if public engineering presence)
7. **LinkedIn profiles** (engineering team skills/endorsements)
8. **Procurement/vendor databases** (if accessible)
9. **Stack Overflow jobs/tech profiles** (declared technologies)
10. **Tech radar/blog posts** (technology adoption announcements)

### Phase 2: Cloud & Infrastructure
Identify:
- **Cloud provider(s)**: AWS, Azure, GCP, multi-cloud
- **Infrastructure approach**: IaaS, PaaS, containers, serverless
- **Orchestration**: Kubernetes, ECS, etc.
- **CDN/Edge**: Cloudflare, Fastly, etc.

### Phase 3: Programming Languages & Frameworks
Map development languages and frameworks:
- **Backend languages**: Python, Java, Go, Node.js, C#, Ruby, PHP, Rust, etc.
- **Frontend frameworks**: React, Vue, Angular, Next.js, etc.
- **Mobile development**: Swift, Kotlin, React Native, Flutter
- **Data/ML languages**: Python, R, Scala, Julia
- **Infrastructure languages**: Go, Python (for tooling)

### Phase 4: Applications & Business Systems
Track enterprise applications:
- **CRM**: Salesforce, HubSpot, Microsoft Dynamics
- **ERP**: SAP, Oracle, NetSuite, Workday
- **Collaboration**: Slack, Microsoft Teams, Zoom, Google Workspace
- **Project management**: Jira, Asana, Monday.com, Linear
- **HR systems**: Workday, BambooHR, ADP
- **Finance**: NetSuite, QuickBooks, Xero
- **Marketing automation**: Marketo, Eloqua, Pardot
- **Data warehouse**: Snowflake, Databricks, BigQuery, Redshift
- **Analytics**: Tableau, Looker, Power BI, Metabase
- **Customer support**: Zendesk, Intercom, Freshdesk

### Phase 5: Security & Compliance Tools
Map current security tooling by category:
- **CSPM** (Cloud Security Posture Management)
- **CWPP** (Cloud Workload Protection)
- **CNAPP** (Cloud-Native Application Protection)
- **SAST/DAST** (Application security testing)
- **Container security**
- **IaC scanning**
- **SIEM/SOAR**
- **Identity/IAM**
- **DLP**
- **Endpoint protection**
- **Secrets management**
- **API security**

### Phase 6: Development & DevOps
Track:
- **CI/CD platforms**: Jenkins, GitLab, GitHub Actions, CircleCI, Azure DevOps
- **Version control**: GitHub, GitLab, Bitbucket
- **IaC tools**: Terraform, CloudFormation, Pulumi, Ansible
- **Container registries**: Docker Hub, ECR, ACR, GCR, Artifactory
- **Monitoring/observability**: Datadog, New Relic, Splunk, Prometheus, Grafana
- **APM**: Datadog, New Relic, AppDynamics, Dynatrace
- **Log management**: Splunk, ELK Stack, Datadog, CloudWatch

## Output Format

### 🎯 Executive Summary
**Overall Stack Confidence: [High/Medium/Low]**
- Key findings (2-3 sentences)
- Primary cloud provider(s)
- Primary programming languages
- Security posture indicator (mature/developing/unknown)

---

### 📋 Quick Reference - Tech Stack One-Liners
*Copy these summaries directly into Customer Alignment or Meeting Prep prompts*

**Cloud & Infrastructure**: [e.g., "AWS (primary), Kubernetes orchestration, Cloudflare CDN"]

**Programming Languages**: [e.g., "Python (backend), React/TypeScript (frontend), Go (microservices)"]

**Business Applications**: [e.g., "Salesforce (CRM), Snowflake (data warehouse), Slack (collaboration), Looker (analytics)"]

**Security Tools**: [e.g., "Prisma Cloud (CSPM), Aqua Security (containers), SonarQube (SAST)"]

**DevOps & CI/CD**: [e.g., "GitHub (version control + Actions for CI/CD), Terraform (IaC), Datadog (monitoring)"]

**Critical Gaps**: [e.g., "No verified IaC scanning, SIEM unknown, secrets management unclear"]

---

### ✅ Verified Technology Stack

#### Cloud Infrastructure
| Technology | Evidence | Source | Confidence |
|------------|----------|---------|------------|
| AWS | Job posting requires "5+ years AWS experience" | [Company Careers Page, Date] | High |
| Kubernetes | Engineering blog post on K8s migration | [Blog URL, Date] | High |

#### Programming Languages & Frameworks
| Language/Framework | Evidence | Source | Confidence |
|-------------------|----------|---------|------------|
| Python | 15 job postings require Python, GitHub repos show Python | [Careers Page + GitHub] | High |
| React | Frontend engineer job posting + tech blog on React migration | [Blog URL, Date] | High |
| Go | Backend services blog post mentions Go microservices | [Blog URL] | Medium |
| Node.js | LinkedIn profiles show Node.js skills (5+ engineers) | [LinkedIn] | Medium |

#### Business Applications
| Category | Application | Evidence | Source | Confidence |
|----------|-------------|----------|---------|------------|
| CRM | Salesforce | Salesforce case study published | [Salesforce.com] | High |
| Collaboration | Slack | Job postings mention "Slack for communication" | [Careers Page] | High |
| Analytics | Looker | Data analyst job requires Looker experience | [Job Posting URL] | High |
| Data Warehouse | Snowflake | Engineering blog on data platform | [Blog URL] | High |

#### Security Tools
| Category | Tool | Evidence | Source | Confidence |
|----------|------|----------|---------|------------|
| CSPM | Prisma Cloud | Case study on Palo Alto website | [URL] | High |
| Container Security | Aqua Security | LinkedIn profiles show 3 engineers with Aqua skills | [LinkedIn] | Medium |
| SAST | SonarQube | Job posting: "Experience with SonarQube" | [Careers Page] | Medium |

#### Development & DevOps
| Technology | Evidence | Source | Confidence |
|------------|----------|---------|------------|
| GitHub | Public repositories visible | [GitHub URL] | High |
| Terraform | Job posting: "Terraform expertise required" | [Careers Page] | High |
| Jenkins | DevOps engineer job mentions Jenkins pipelines | [Job Posting] | Medium |
| Datadog | Partnership announcement on Datadog blog | [Datadog Blog] | High |

---

### ❓ Knowledge Gaps & Assumptions

#### Critical Unknowns
- **IaC scanning solution**: No public information found on infrastructure-as-code security scanning
- **SIEM platform**: Unknown what they use for log aggregation and security monitoring
- **Multi-cloud presence**: Confirmed AWS, unclear if also using Azure/GCP
- **Mobile development**: No evidence of mobile apps or mobile tech stack
- **Secrets management**: No information on how they handle secrets/credentials
- **ERP system**: Unknown if using enterprise resource planning software

#### Reasonable Assumptions (Flagged as Unverified)
- **Assumption**: Likely using TypeScript with React (based on modern frontend job requirements)
  - **Why reasonable**: Job postings emphasize "modern JavaScript" and type safety
  - **Verification needed**: Confirm in technical discovery

- **Assumption**: Probably using Docker for containerization (based on Kubernetes use)
  - **Why reasonable**: K8s requires container runtime, Docker is standard
  - **Verification needed**: Ask what container tooling they use

- **Assumption**: Likely using GitHub Advanced Security (based on GitHub Enterprise use + engineering blog focus on security)
  - **Why reasonable**: Company size (500+ engineers) and security maturity indicators suggest need for code scanning
  - **Verification needed**: Confirm in discovery conversation

- **Assumption**: Probably have basic cloud-native monitoring (CloudWatch)
  - **Why reasonable**: Standard with AWS, mentioned in passing in blog
  - **Verification needed**: Ask what visibility gaps exist

#### Missing Categories
**Languages**:
- [ ] No evidence of: .NET/C# (unclear if using Microsoft stack)
- [ ] No evidence of: Java (possible gap or not used)
- [ ] Unknown: Database languages (SQL variants, NoSQL)

**Applications**:
- [ ] Unknown: ERP/finance systems
- [ ] Unknown: HR/payroll systems
- [ ] No evidence of: Marketing automation platform
- [ ] Unknown: Customer support ticketing system

**Security**:
- [ ] No evidence of: Secrets management tool (Vault, etc.)
- [ ] No evidence of: API security solution
- [ ] No evidence of: Data loss prevention (DLP) tool
- [ ] Unknown: Incident response platform
- [ ] No evidence of: DAST tooling

---

### 🔍 Research Methodology Notes
**Sources searched**:
- ✅ Company engineering blog (12 posts reviewed)
- ✅ Last 50 job postings (past 6 months)
- ✅ LinkedIn (25+ relevant employee profiles)
- ✅ Vendor case study databases (Salesforce, AWS, Datadog)
- ✅ Conference presentation archives (2 talks found)
- ✅ GitHub (public repositories analyzed)
- ❌ No Stack Overflow company page found
- ❌ No accessible tech stack databases (BuiltWith limited info)

**Research limitations**:
- Information current as of [date]
- Cannot verify internal/proprietary tools or applications
- Some tools may be in pilot/POC phase
- Legacy applications not visible in public hiring/blog posts
- Absence of evidence ≠ evidence of absence

---

### 💡 Discovery Question Priorities
Based on gaps, prioritize asking about:

**Technical Discovery**:
1. **Language standardization**: "What are your primary programming languages for backend and frontend development?"
2. **IaC security**: "How do you currently scan Terraform/CloudFormation for misconfigurations?"
3. **SIEM/logging**: "What's your approach to centralizing cloud security logs?"
4. **Application scanning**: "How do you scan your Python/React applications for vulnerabilities in the CI/CD pipeline?"
5. **Secrets management**: "How do you manage secrets and credentials across your development and cloud environments?"

**Business Context**:
1. **Application landscape**: "What are your mission-critical applications that need security coverage?"
2. **Data systems**: "What data warehouses or analytics platforms are you running in the cloud?"
3. **Coverage gaps**: "What parts of your cloud environment or application stack feel least visible from a security perspective?"

---

### 🎯 Wiz Positioning Opportunities

**Language/Framework Coverage** (verified stack):
- ✅ Python scanning (Wiz Code supports)
- ✅ JavaScript/React scanning (Wiz Code supports)
- ✅ Terraform/IaC scanning (Wiz Code + Cloud)
- ⚠️ Go microservices (confirm scanning needs)

**Potential consolidation plays** (verified competitors):
- Prisma Cloud (CSPM) + Aqua (Container) + SonarQube (SAST) = Wiz Code + Cloud all-in-one
- [List only if you found verified tools]

**Capability gaps** (based on missing categories):
- IaC scanning at scale across Terraform
- Unified scanning for Python + React codebases
- Container registry scanning (if using ECR/private registry)
- Secrets detection in code and IaC
- API security for microservices architecture
- [List only confirmed gaps, not speculation]

**Application security coverage**:
- Cloud-native apps built with Python/React/Go need runtime + code scanning
- Kubernetes workloads need continuous posture management
- Multi-repo GitHub environment needs centralized security visibility

---

## Quality Standards
✅ **DO**:
- Cite every claim with a source URL and date
- Rate confidence level for each finding (High/Medium/Low)
- Explicitly call out assumptions vs. verified facts
- Highlight what you couldn't find
- Note when evidence is circumstantial (e.g., "implies Python usage")
- Include programming language version info if available
- Keep one-liner summaries concise and copy-paste ready

❌ **DON'T**:
- Guess or infer without labeling it as an assumption
- Present absence of evidence as confirmation
- Use outdated information without date stamps
- Include "likely uses X" without explaining reasoning
- Assume a language/app is used just because it's popular
- Conflate frameworks with languages (React ≠ JavaScript)
- Overcomplicate the one-liner summaries with details

---

## Refresh Cadence
- **Before first meeting**: Full research
- **Before technical/demo deep dive**: Update with any new job postings or blog posts, focus on dev stack
- **Before security review**: Verify security tools and scanning coverage
- **Before close**: Final verification of tech stack for scoping/SOW, confirm language support needs

---

## Special Notes

### Programming Language Priority
Focus on:
1. **Production languages** (what they build products with)
2. **Infrastructure languages** (what they manage cloud with)
3. **Data languages** (what they analyze with)

### Application Priority
Focus on:
1. **Cloud-connected SaaS** (security implications)
2. **Data storage systems** (sensitive data concerns)
3. **Developer tools** (integration opportunities)
4. **Business-critical apps** (compliance requirements)

### One-Liner Usage
The Quick Reference section is designed to be:
- **Copy-paste ready** for other research prompts
- **Concise** (one line per category)
- **Accurate** (only verified tech, no assumptions)
- **Contextual** for sales conversations
```

Perfect! Now the output includes a **"Quick Reference - Tech Stack One-Liners"** section right after the Executive Summary that provides:

1. **Easy copy-paste** - Single lines ready to drop into Customer Alignment prompts
2. **Organized by category** - Matches the detailed sections below
3. **Verified only** - Only includes confirmed tech, not assumptions
4. **Includes gaps** - Has a "Critical Gaps" line so you know what's missing

Example output would look like:
```
**Cloud & Infrastructure**: "AWS (primary), Kubernetes orchestration, Cloudflare CDN"
**Programming Languages**: "Python (backend), React/TypeScript (frontend), Go (microservices)"
**Critical Gaps**: "No verified IaC scanning, SIEM unknown, secrets management unclear"