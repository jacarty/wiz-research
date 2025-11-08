# Tech Stack Discovery & Verification

## Input Required
**Company:** [Company Name]  
**Industry/Sector:** [If known, otherwise identify through research]  
**Website:** [Company website URL]
**LinkedIn Company Page:** [LinkedIn URL if known]

## Objective
Conduct thorough research to identify and verify a customer's technology infrastructure, security tools, cloud environment, programming languages, and applications. **Provide ONLY sourced information with citations. Do not make assumptions or inferences.**

## Research Process

### Phase 1: Public Signal Collection
Search for verified technology indicators:
1. **Engineering blogs & tech publications** (highest confidence)
2. **Job postings** (active tech requirements)
3. **Company careers pages** (required skills = current stack)
4. **Conference talks & presentations** (teams discussing their tools)
5. **Case studies from vendors** (confirmed tool usage)
6. **GitHub repositories** (if public engineering presence)
7. **GitLab repositories** (if public engineering presence)
8. **LinkedIn profiles** (engineering team skills/endorsements)
9. **Stack Overflow jobs/tech profiles** (declared technologies)
10. **Tech radar/blog posts** (technology adoption announcements)
11. **Vendor partnership announcements** (confirmed integrations)
12. **Public APIs** (confirmed for Web/Mobile)

### Phase 2: Cloud & Infrastructure
Identify:
- **Cloud provider(s)**: AWS, Azure, GCP, Oracle, Alibaba, multi-cloud
- **Infrastructure approach**: IaaS, PaaS, SaaS, containers, serverless
- **Orchestration**: Kubernetes, ECS, AKS, GKS, etc.
- **CDN/Edge**: Cloudflare, Fastly, Akamai, etc.

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
- **ASM** (Attack Surface Management)
- **Container security**
- **IaC scanning**
- **SIEM/SOAR**
- **Identity/IAM**
- **DLP**
- **Secrets management**
- **API security**

### Phase 6: Development & DevOps
Track:
- **CI/CD platforms**: Jenkins, GitLab CI/CD, GitHub Actions, CircleCI, Azure DevOps
- **Version control**: GitHub, GitLab, Bitbucket
- **IaC tools**: Terraform, CloudFormation, Pulumi, Ansible
- **Container registries**: Docker Hub, ECR, ACR, GCR, GitLab Container Registry, Artifactory
- **Monitoring/observability**: Datadog, New Relic, Splunk, Prometheus, Grafana
- **APM**: Datadog, New Relic, AppDynamics, Dynatrace
- **Log management**: Splunk, ELK Stack, Datadog, CloudWatch

---

## Output Format

### 🎯 Executive Summary
**Overall Stack Confidence: [High/Medium/Low]**
- Key findings (2-3 sentences summarizing what was verified)
- Primary cloud provider(s) - ONLY if verified
- Primary programming languages - ONLY if verified
- Security posture indicator (mature/developing/unknown) - based only on verified tools

### ✅ Verified Technology Stack

#### Cloud Infrastructure
| Technology | Evidence | Source | Date | Confidence |
|------------|----------|---------|------|------------|
| AWS | Job posting requires "5+ years AWS experience" | [Company Careers Page URL] | [Date] | High |
| Kubernetes | Engineering blog post: "Our Migration to Kubernetes" | [Blog URL] | [Date] | High |

#### Programming Languages & Frameworks
| Language/Framework | Evidence | Source | Date | Confidence |
|-------------------|----------|---------|------|------------|
| Python | 15 job postings require Python | [Careers Page URL] | [Date range] | High |
| React | Job posting: "Senior React Developer" + blog post on React migration | [URLs] | [Date] | High |

#### Business Applications
| Category | Application | Evidence | Source | Date | Confidence |
|----------|-------------|----------|---------|------|------------|
| CRM | Salesforce | Salesforce customer case study | [Salesforce.com URL] | [Date] | High |
| Collaboration | Slack | 8 job postings mention "Slack for team communication" | [Careers URL] | [Date] | High |

#### Security Tools
| Category | Tool | Evidence | Source | Date | Confidence |
|----------|------|----------|---------|------|------------|
| CSPM | Prisma Cloud | Palo Alto Networks case study | [URL] | [Date] | High |
| SAST | SonarQube | Job posting: "Experience with SonarQube required" | [URL] | [Date] | Medium |

#### Development & DevOps
| Technology | Evidence | Source | Date | Confidence |
|------------|----------|---------|------|------------|
| GitHub | Public GitHub organization with 47 repositories | [GitHub URL] | [Accessed Date] | High |
| GitLab | Public GitLab group with active repositories + CI/CD pipelines visible | [GitLab URL] | [Accessed Date] | High |
| Terraform | 6 job postings require Terraform experience | [Careers URL] | [Date range] | High |

---

### ❓ Knowledge Gaps
**Categories with NO verified information found:**

#### Cloud & Infrastructure
- Multi-cloud usage (Azure, GCP) - no evidence found
- CDN provider - no public information
- Container registry - not specified in public sources

#### Programming Languages
- Backend languages beyond [verified ones] - no evidence
- Mobile development stack - no job postings or blog posts found
- Database technologies - no specific mentions found

#### Business Applications
- ERP system - no evidence found
- HR/Payroll platform - no public information
- Marketing automation - no mentions in public sources
- Customer support platform - unknown

#### Security Tools
- IaC scanning solution - no public information
- SIEM platform - no evidence found
- Secrets management tool - no mentions
- API security solution - unknown
- DLP tool - no evidence
- SAST/DAST tooling - no public information

#### Development & DevOps
- CI/CD platform - no specific evidence found (check for GitHub Actions, GitLab CI/CD, Jenkins, CircleCI)
- Container orchestration details - not specified
- Monitoring/APM tools - no verified sources

---

### 🔍 Research Methodology
**Sources searched**:
- ✅ Company engineering blog - [X posts reviewed, date range]
- ✅ Job postings - [X postings reviewed, date range]
- ✅ LinkedIn profiles - [X profiles analyzed]
- ✅ Vendor case studies - [Vendors searched: list]
- ✅ GitHub - [Organization found/not found, URL]
- ✅ GitLab - [Organization found/not found, URL]
- ✅ Conference presentations - [X talks found/none found]
- ❌ Stack Overflow company page - [not found]
- ❌ Tech stack databases - [limited/no information]

**Research date**: [Date of research]
**Information currency**: All sources dated [date range]

**Research limitations**:
- Cannot verify internal/proprietary tools
- Cannot confirm tools in pilot/POC phases
- Cannot see legacy systems not mentioned in recent hiring
- Cannot access private GitHub/GitLab repositories
- Absence of public evidence ≠ confirmation they don't use it

---

## Quality Standards

✅ **DO**:
- Cite every claim with source URL and date
- Rate confidence (High/Medium/Low) based on source quality
- Leave sections blank if no verified information exists
- Use exact quotes from sources when relevant
- Note the date sources were accessed
- Clearly separate "verified" from "not found"
- Include null results (e.g., "No evidence found for...")
- Check both GitHub AND GitLab for public repositories
- Note if repositories are public/private or if organization doesn't exist

❌ **DON'T**:
- Make assumptions or inferences without explicit labeling
- List technologies without sources
- Use phrases like "likely uses" or "probably has"
- Present absence of evidence as confirmation they don't use something
- Include outdated information without date context
- Guess based on industry standards
- Fill in gaps with "common" tools
- Assume GitHub if you haven't checked GitLab (or vice versa)

---

## Confidence Levels

**High Confidence**:
- Official case studies from vendors
- Company engineering blog posts explicitly mentioning tech
- Multiple job postings requiring specific technology
- Public GitHub/GitLab repositories showing active use
- Conference presentations by company engineers

**Medium Confidence**:
- Single job posting mentioning technology
- LinkedIn skills/endorsements from multiple employees
- Tech mentioned in passing in blog posts
- Partnership announcements

**Low Confidence**:
- Single LinkedIn profile mention
- Indirect references
- Old information (>1 year)

**DO NOT REPORT anything below Medium confidence unless explicitly flagged as "unverified speculation"**

---

## Special Notes

### GitHub vs GitLab Detection
- **Always check both platforms** - don't assume one based on company type
- **Public vs Private**: Note if org exists but repos are private
- **CI/CD indicators**: 
  - GitHub: Look for `.github/workflows/` in repos
  - GitLab: Look for `.gitlab-ci.yml` in repos, or check GitLab CI/CD interface
- **Container registries**:
  - GitHub: GitHub Container Registry (ghcr.io)
  - GitLab: GitLab Container Registry (registry.gitlab.com)

### Version Control Platform Signals
High confidence signals for GitHub:
- Public github.com/[company] organization
- Job postings: "GitHub experience required"
- Engineering blog: "We use GitHub for..."

High confidence signals for GitLab:
- Public gitlab.com/[company] group
- Job postings: "GitLab experience required"
- Engineering blog: "We migrated to GitLab..."
- Self-hosted GitLab instance (gitlab.[company-domain].com)

**Note**: Companies may use BOTH platforms (e.g., GitHub for open source, GitLab for internal)

**Container Registry Detection:**
- GitHub: Check for ghcr.io references
- GitLab: Check for registry.gitlab.com references
- AWS: Check for ECR
- Azure: Check for ACR
- GCP: Check for GCR
- Self-hosted: Check for harbor, artifactory mentions
