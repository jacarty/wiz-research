# User Guide: GTM Intelligence Brief Bot

## Quick Start

**Purpose:** This bot analyzes prospect intelligence reports and generates ranked Wiz use-case recommendations aligned to the prospect's business priorities.

---

## How to Use in Slack

### Step 1: Prepare Your Command
```
[paste synthesis prompt above]

[paste your prospect intelligence report]
```

### Step 2: Run in Merlin
1. Open your Slack workspace
2. Find Merlin
3. Paste the full prompt + report
4. Send the message

### Step 3: Get Your Output
The bot will generate a markdown file containing:
- Top 5 priority use-cases ranked by strategic fit
- Additional aligned use-cases
- Technology-specific recommendations
- Competitive displacement analysis
- Output will go into NotebookLM

---

## Example Usage

```
# Wiz GTM Use-Case Alignment

[Full synthesis prompt text here]

---

## PROSPECT INTELLIGENCE REPORT

**Company:** Acme Corp
**Industry:** FinTech
**Priority:** Scale to 10M users while reducing infrastructure costs by 15%
**Tech Stack:** AWS, Kubernetes, Terraform, GitHub Actions
**Compliance:** SOC 2, PCI-DSS

[Rest of report...]
```
