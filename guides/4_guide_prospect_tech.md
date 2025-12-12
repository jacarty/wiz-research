# Tech Stack Discovery & Verification - User Guide

## What It Does

Identifies and verifies a company's technology stack through systematic research. **Source-backed intelligence only** - no assumptions or guesses.

**Discovers:** Cloud infrastructure, programming languages, security tools, business applications, DevOps tooling, and explicitly documents knowledge gaps.

---

## How to Use

```
Conduct Tech Stack Discovery & Verification for:

Company: [Company Name]
Website: [URL]
[Optional: Industry/Sector, LinkedIn URL]

[Paste full prompt]
```

**Examples:**
- Basic: `Company: Monzo Bank, Website: https://monzo.com`
- With focus: `Company: [Name], Website: [URL], Note: Prioritize security tooling`

---

## What You'll Get

### 1. Executive Summary
Overall confidence level, key findings, primary cloud/languages (if verified), security posture

### 2. Verified Technology Stack (6 Tables)
Each technology entry includes: Evidence | Source URL | Date | Confidence Level

- **Cloud Infrastructure** - Providers, orchestration, CDN
- **Programming Languages** - Backend, frontend, mobile
- **Business Applications** - CRM, ERP, collaboration, analytics
- **Security Tools** - CSPM, SAST, SIEM, secrets management, etc.
- **DevOps & CI/CD** - GitHub/GitLab, Terraform, monitoring, registries
- **Knowledge Gaps** - What wasn't found (saves discovery time)

### 3. Research Methodology
Sources checked, dates, limitations

---

## Key Features

### Verification Standards

**VERIFIED means:**
- Engineering blogs/tech publications
- Multiple job postings (3+)
- Vendor case studies
- Public GitHub/GitLab repos
- Conference talks
- Partnership announcements

**Every finding has:** Technology | Evidence | Source URL | Date | Confidence (High/Medium/Low)

**Never includes:** Assumptions, "likely uses" statements, unsourced claims, guesses

### Knowledge Gaps (Critical)

Instead of speculation, explicitly lists what **wasn't found**:
- "SIEM platform - no evidence found (searched job postings, blog, vendor sites)"
- Helps focus discovery questions
- Avoids asking about already-verified tech

### GitHub + GitLab Coverage

Always checks BOTH platforms (companies often use both):
- Public repositories
- CI/CD pipelines (.github/workflows/, .gitlab-ci.yml)
- Container registries (ghcr.io, registry.gitlab.com)
- Self-hosted instances

---

## Output Example

```
| Technology | Evidence | Source | Date | Confidence |
|------------|----------|---------|------|------------|
| AWS | 12 job postings require AWS + blog post "Our AWS Migration" | [URLs] | Nov 2025 | High |
| Python | 15 job postings require Python | [Careers URL] | Oct-Nov 2025 | High |
| GitLab | Public group (gitlab.com/company) with 23 repos, CI/CD visible | [URL] | Nov 2025 | High |
```

**Knowledge Gap:**
```
#### Security Tools
- SIEM platform - no evidence (searched: jobs, blog, Splunk/Datadog customer pages)
- Secrets management - no public information
```

---

## Use Cases

- **Pre-sales technical research** - Understand landscape before calls
- **Competitive displacement** - Verify current tools for replacement opportunities
- **Solution architecture** - Cloud environment, language support, integration planning
- **Discovery preparation** - Focus questions on gaps, avoid re-confirming verified tech
- **Account strategy** - Identify expansion opportunities, assess maturity

---

## Tips

**Provide:**
- Accurate company name and website
- LinkedIn company page (helpful but not required)
- Research focus if needed ("prioritize security tooling")

**Follow-ups:**
- "Deep dive on security tooling - check more vendor case studies"
- "Update with job postings from past month"
- "Research their monitoring/observability stack"
- "Create discovery questions based on knowledge gaps"

---

## When to Use

**✅ Ideal for:**
- Companies with engineering blogs, active hiring, public repos
- Tech companies with vendor case studies
- Pre-meeting research requiring verified intel

**❌ Less useful for:**
- Stealth companies with minimal public presence
- Small companies with no blog or public repos
- Organizations with private-only repos

**Limitations:** Cannot verify internal tools, pilot projects, or legacy systems not mentioned publicly. Absence of evidence ≠ they don't use it.

---

## Research Sources (10 Primary)

1. Engineering blogs
2. Job postings
3. Vendor case studies
4. GitHub repositories
5. GitLab repositories
6. Conference talks
7. LinkedIn profiles
8. Partnership announcements
9. Tech adoption posts
10. Public APIs

---

## Quality Checklist

- ✅ Every tech has source URL, date, confidence level
- ✅ Both GitHub AND GitLab checked
- ✅ Job patterns (3+ postings, not single mentions)
- ✅ Knowledge gaps explicitly documented
- ✅ No "likely" or "probably" without clear flagging
- ✅ Research methodology complete