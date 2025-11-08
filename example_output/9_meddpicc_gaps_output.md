This analysis is prepared by the Account Executive and Sales Engineer to ensure a highly targeted discovery call, focusing on JustPark's post-merger integration, platform resilience, and critical cloud security gaps within their AWS/Kubernetes environment.

---

## MEDDPICC Gap Analysis

### Metrics: Business KPIs/quantifiable impact

| What We Know | What's MISSING (Critical Knowledge Gaps) |
| :--- | :--- |
| **Operational Goals:** The company prioritizes "Platform Resilience & Scalability," aiming for **>99.9% uptime** to manage high-demand periods for its real-time marketplace. | **Latest Financials:** The latest accounts (to Dec 31, 2024) are filed, but the **Annual Revenue** figure is not publicly available. |
| **Volume/Reach:** JustPark is trusted by **13 million+ drivers**, and its combined platform powers **$1 billion+ in booking volume** annually. | **Cost of Pain (COP):** The quantifiable business impact of platform downtime, security incidents, or scaling failures. We know failure undermines their core value proposition, but not the financial cost. |
| **B2B Focus:** They are driving adoption of **AI-driven revenue projections** for operators. | **KPI Targets:** Specific revenue or market share targets for the combined UK business post-merger. How is the success of the "unified provider" strategy measured?. |

### Economic Buyer: Budget authority

| What We Know | What's MISSING (Critical Knowledge Gaps) |
| :--- | :--- |
| **Strategic Leadership:** The global entity is led by **CEO Jeff Shanahan** (FinTech/Payments background) and the UK business by **Founder & President Anthony Eskinazi**. | **CFO/Budget Authority:** The Chief Financial Officer is **NOT FOUND**. We do not know the senior finance executive overseeing the UK budget and new technology investments. **This is the single greatest structural roadblock to closing the deal.** |
| **Operational Leader:** **COO Jonathan Hampson** is responsible for scaling operations and efficiency. | **Budget Allocation:** Where the budget for this initiative sits—under Capex (infrastructure), Opex (FinOps/security tools), or a specific integration fund (post-merger). |

### Decision Criteria: Technical/business requirements

| What We Know | What's MISSING (Critical Knowledge Gaps) |
| :--- | :--- |
| **High Priority:** Solutions must provide **superior performance and reliability** due to their history of switching vendors over "deliverability issues". | **Formal Scorecard/Weighting:** We don't know the relative weighting of technical security (e.g., EKS/IaC scanning) versus operational resilience (e.g., uptime) versus compliance (e.g., GDPR audit readiness). |
| **Technical Stack Fit:** Must integrate with or secure **AWS, Amazon EKS, AWS Fargate, GitLab CI/CD, and Terraform**. | **Required Certifications:** We need to confirm if B2B/B2G customers (via G-Cloud) are *now* explicitly requiring **ISO 27001, SOC 2**, or specific security audit criteria. |
| **Strategic Fit:** Solution must support the **AI-driven B2B data focus** and enhance GDPR/UK data protection compliance. | **Specific Security Standards:** Detailed requirements for cloud-native security coverage (e.g., must the tool support **CIEM** or **CWPP** specifically?). |

### Decision Process: Approval steps, timeline

| What We Know | What's MISSING (Critical Knowledge Gaps) |
| :--- | :--- |
| **Key Influencers:** **CTO Todd Marshall** is the ultimate owner of the technical platform and integration strategy. | **Timeline and Urgency:** What is the non-negotiable deadline for completing the ParkHub/JustPark technical integration? Is there a hard deadline tied to the end of a fiscal year or a specific B2B contract launch? |
| **Organizational Input:** Input will come from Development (PHP to Go/Python migration), Operations (resilience/uptime), and Security (data protection). | **Internal Steps:** Is there a mandatory **Proof of Concept (PoC)**, a technical bake-off, or a "pilot first" approach? How long are these phases expected to last? |

### Paper Process: Procurement, legal, security review

| What We Know | What's MISSING (Critical Knowledge Gaps) |
| :--- | :--- |
| **Legal Entity:** The correct legal entity for contracting is **JUSTPARK PARKING LIMITED**. | **Security Review Contact:** There is **no publicly listed CISO or Head of Security**. We need to know who executes the security sign-off and where they sit organizationally (e.g., reporting to CTO or COO). |
| **Regulatory Burden:** High burden due to **GDPR** and status as a data controller for millions of drivers, meaning stringent legal review of data processing agreements. | **Contract Standards:** What are their standard contract terms, and how lengthy is the legal/procurement review process, especially for G-Cloud eligible vendors? |

### Identify Pain: Current challenges/incidents

| What We Know | What's MISSING (Critical Knowledge Gaps) |
| :--- | :--- |
| **Structural Pain (Integration):** Successfully integrating the JustPark B2C platform with ParkHub's B2B software while retaining talent. | **Tactical Pain (Cloud Security):** We have high confidence in their *gaps* (No known CSPM, SIEM, or Secrets Management), but we don't have a specific **recent incident, failure, or close call** that acts as a compelling event. |
| **Operational Pain (Reliability):** Need for "advanced redundancy and failover mechanisms" to handle "peak demand periods". | **Data Quality Pain:** We know AI requires good data governance, but we don't know if their current post-merger data lake (on S3) suffers from quality or integrity issues that hamper their "JustPark Insights" product. |

### Champion: Internal advocate identification

| What We Know | What's MISSING (Critical Knowledge Gaps) |
| :--- | :--- |
| **Potential Technical Champions:** **Todd Marshall (CTO)** or the **Senior Security Engineer** they are hiring (suggests internal focus on solving these issues). | **Confirmed Champion:** We have **no identified internal advocate** who owns this specific initiative, has influence across IT/Ops/Security, and is willing to put their reputation behind our solution. |
| **Potential Operational Champions:** **Jonathan Hampson (COO)**, whose remit covers operations and reliability. | **Political Standing:** We don't know which individual stakeholder (CTO/COO/President) is being most pressured by the board (FTV Capital) to solve the security and scalability problem. |

### Competition: Incumbent tools/vendors

| What We Know | What's MISSING (Critical Knowledge Gaps) |
| :--- | :--- |
| **Existing Security Tools:** **Snyk** (SAST/DAST) and **SonarQube** (SAST) for application security; **Okta** for identity. **Cloudflare** (WAF, CDN) is also used. | **CNAPP/CSPM Competitors:** Are they actively evaluating direct competitors to our solution (e.g., Wiz competitors like Prisma Cloud, Lacework, Orca Security)? This is critical for positioning. |
| **DevOps Tools:** **GitLab CI/CD, GitHub, Terraform, Docker, Datadog**. We must integrate with these systems. | **SIEM/SOAR/Secrets:** We know they have a **gap** in SIEM and Secrets Management, meaning there is a competitive opportunity but we don't know if they have initiated an RFP for these tools yet. |

---

## Role-Tailored Question Funnels

The prospect is a PE-backed, transactional, cloud-native UK platform company undergoing a critical international merger and facing high regulatory pressure (GDPR/G-Cloud). We target the need for unified cloud security and operational resilience.

**Attendees calibration:** Assume the AE will speak primarily to the Business Context and Buying Process, and the SE will speak to the Technical Environment.

### 1. Business Context Funnel (AE Focus: Merger, Growth, Risk)

**Goal:** Understand how security and reliability fit into the post-merger, international growth strategy and how financial success is measured.

| Stage | Question | Tailored Context/Justification |
| :--- | :--- | :--- |
| **Open Question** | "Since the merger with ParkHub and the North American expansion in January, **what is the single biggest operational challenge that threatens your goal of becoming the unified parking provider** for both the UK and US markets?" | *Specific to:* Post-Merger Unification, Geographic Expansion, COO/President strategic pain points. Encourages a 'storytelling' response about friction. |
| **Probing** | "We know your commitment to B2B customers requires **>99.9% uptime** and that you're focusing on **AI-driven insights**. Can you walk us through a recent situation where maintaining that uptime or securing that critical data became a significant drain on either resources or B2B customer trust?" | *Specific to:* Operational Pain, B2B/B2G focus, and platform resilience. Connects security/uptime directly to revenue/trust. |
| **Confirming** | "It sounds like securing the combined entity's data—especially for GDPR/ICO and your G-Cloud contracts—is now a competitive necessity, not just a compliance checkbox. **Is the ultimate goal to invest in a cloud security solution that acts as a single pane of glass to accelerate audit readiness and reduce the cost of continuous compliance?**" | *Specific to:* G-Cloud, GDPR, and the critical need for compliance mastery as a competitive advantage. |

### 2. Technical Environment Funnel (SE Focus: Cloud-Native Security Gaps)

**Goal:** Deeply explore the security challenges created by the technical stack (EKS, Terraform, Go/Python migration) and confirm the massive public knowledge gaps (CSPM, SIEM, Secrets).

| Stage | Question | Tailored Context/Justification |
| :--- | :--- | :--- |
| **Open Question** | "Your team is doing complex work migrating from a **PHP monolith to Go/Python microservices** using **EKS and Fargate**. What are the greatest security risks you've encountered in managing the posture and compliance across this hybrid environment, especially for the shared data lake on S3?" | *Specific to:* JustPark's unique tech stack and transition. Focuses on *their* specific engineering challenges. |
| **Probing** | "We see you use **Terraform** and hire for **Snyk/SonarQube**, which are great application tools. Given the size of your AWS footprint, **how are you currently scanning your Terraform files for security misconfigurations *before* they deploy, and what solution are you using for Cloud Security Posture Management (CSPM) to monitor EKS runtime compliance?"** | *Specific to:* Addressing the verifiable IaC scanning and CSPM/CNAPP gaps. This is a "gotcha" question designed to force disclosure of the current tooling gap. |
| **Confirming** | "If we could provide a single platform that consolidates vulnerability management across your Go/Python code, Kubernetes clusters, and AWS accounts, while also **securely managing the secrets** needed by your **GitLab CI/CD**—**would that accelerate your integration project timeline by at least 25%?**" | *Specific to:* Confirming the value proposition of holistic CNAPP/Secrets Management relative to their critical integration timeline. |

### 3. Buying Process Funnel (AE Focus: Decision Makers, Budget, Timeline)

**Goal:** Identify the unknown CFO/Economic Buyer, CISO/Paper Process contact, and establish a firm timeline.

| Stage | Question | Tailored Context/Justification |
| :--- | :--- | :--- |
| **Open Question** | "For a strategic investment like this—which touches operational resilience, engineering productivity, and GDPR compliance—**who are the three key stakeholders (roles, not names) who need to champion this project for it to get budget approval and move to implementation?**" | *Specific to:* Complex decision-making common in PE-backed, high-compliance environments. Circumvents the missing CFO/CISO. |
| **Probing** | "We saw the UK C-suite recently changed, and you’re focused on streamlining operations. **Who is the senior finance executive overseeing the UK budget for technology investments**, and does this project need to be approved before the end of the calendar year?" | *Specific to:* Directly addressing the missing CFO and establishing urgency/timeline (M-P-E alignment). |
| **Confirming** | "Assuming we move forward with a technical PoC based on your EKS environment, **who specifically owns the final security sign-off, and what level of certification (ISO 27001/SOC 2) is required on our side to clear their compliance review?**" | *Specific to:* Addressing the missing CISO/Head of Security and confirming the **Paper Process** requirements, particularly around B2B/B2G standards. |

---

## Red Flags & Risks

### Missing information that could derail the deal

1.  **Missing Economic Buyer (CFO):** The inability to identify the senior finance executive in the UK **who holds the budget sign-off authority** is a major blocker. We risk selling to an influencer (CTO) who cannot release funds.
2.  **Missing Security Approver (CISO):** The person responsible for the critical **security review and sign-off** (the final Paper Process step) is unknown. This function is paramount given JustPark's GDPR obligations and B2G engagement.
3.  **No Confirmed Champion:** We lack a confirmed internal advocate who is actively running an evaluation and has a vested political interest in our success. We must confirm the identity of the Champion in the discovery call.
4.  **No Quantified Pain:** We know they need **>99.9% uptime**, but we lack the exact financial cost of an incident (revenue lost, penalty fees, engineering hours spent) which is essential for calculating ROI (Metrics) for the PE investors.

### Assumptions we're making without validation

1.  **Assumption of Security Immaturity:** We are assuming that because there are no *publicly listed* CSPM, SIEM, or Secrets Management solutions, they must be using rudimentary or homegrown tools. They might, however, be using private, non-publicly disclosed enterprise solutions.
2.  **Assumption of Single Evaluation:** We are assuming JustPark is currently only evaluating one or two solution types (e.g., CNAPP). They might be running simultaneous, parallel evaluations for SIEM, secrets management, and CSPM separately, which would require us to consolidate our message against a much wider field of specialized competitors.
3.  **Assumption of UK Focus:** While Anthony Eskinazi leads the UK business, the **CEO Jeff Shanahan is based in the US**. We are assuming the budget and decision process is centered in the UK organization, but the new global structure post-merger might necessitate sign-off from the US HQ.
4.  **Assumption of Technology-Driven Pain:** We are assuming the primary blocker to B2B growth is *technical reliability* and *security*. It may actually be the **challenge of finding clear AI use cases** or **talent retention**, which would require us to pivot the ROI conversation towards developer velocity and FinOps.