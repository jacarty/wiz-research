
# Slackbot Prompt: Wiz Use-Case Alignment Generator

Analyze the following Prospect Intelligence Report and identify all Wiz use-cases that align to the prospect's business strategy, priorities, technology environment, and security gaps.

## INSTRUCTIONS

Use Wizdoc's, roadmap tracker, gdrive, slack, product knowledge and use-case library:

1. **Identify ALL Wiz use-cases** that align to:
   - Business priorities (cloud cost management, merger integration, developer velocity, scalability)
   - Technology environment (cloud providers, tech stack, IaC tools, CI/CD)
   - Security posture gaps (CSPM, CWPP, CNAPP, SIEM, secrets management, IaC scanning)
   - Compliance requirements (GDPR, SOC2, ISO27001, FCA, PCI-DSS, etc.)
   - Buying signals (audits, incidents, expansion, technical debt)

2. **Highlight the TOP 5 use-cases** that are:
   - Most directly aligned to stated priorities and pain points
   - Address the most critical security gaps identified
   - Map to urgency indicators or strategic initiatives
   - Provide measurable business value (cost savings, risk reduction, compliance, velocity)

3. **For each use-case include:**
   - Use-case name
   - Brief description of what Wiz capability solves
   - Specific alignment to prospect's environment/priorities/gaps (reference report facts)
   - Expected business outcome

## OUTPUT FORMAT

Return in markdown:

```markdown
# Wiz Use-Case Alignment: [Company Name]

## TOP 5 PRIORITY USE-CASES

### 1. [Use-Case Name]
**Wiz Capability:** [Description]  
**Alignment:** [Specific reference to report - tech, gap, or priority]  
**Business Outcome:** [Expected value]

[Repeat for top 5]

---

## ADDITIONAL ALIGNED USE-CASES

### [Use-Case Name]
**Alignment:** [Brief alignment description]

[List remaining use-cases]
```

Generate the use-case alignment now.

## PROSPECT INTELLIGENCE REPORT
