**COMPANY MISSION**
- JustPark is a leading, PE-backed technology marketplace focused on unifying the B2C parking experience with B2B management software to provide seamless, smart, and scalable mobility solutions across the UK and North America.

**SUPPORTING STRATEGY**
- Achieve post-merger unification by securely integrating two distinct B2C and B2B platforms via scalable, API-driven architecture.
- Ensure platform resilience and maintain contractual obligations of **>99.9% uptime** to manage peak demand periods for their real-time marketplace.
- Shift the core value proposition to B2B data monetization using **AI-driven projections** for revenue and occupancy, requiring robust data integrity and processing.

**KEY INITIATIVES**
- Complete the technical transformation from a legacy PHP application to a modern, scalable **Go and Python microservices architecture**.
- Scale the "JustPark Insights" platform to leverage AI for commercial value, predicting occupancy and revenue for over 500 B2B customers.
- Operationalize **Platform Engineering** using Terraform and GitLab CI/CD to accelerate developer velocity and enforce consistent security standards.
- Achieve G-Cloud readiness and potential external security certifications (e.g., ISO 27001) to unlock new B2G and enterprise revenue streams.

**RISKS & CHALLENGES**
- **Unidentified cloud attack paths** due to critical coverage gaps in cloud security posture management (CSPM/CNAPP), risking platform resilience and breach of B2B contracts.
- Erosion of customer trust and severe ICO fines due to failure to meet non-negotiable **GDPR requirements** for 14M+ drivers and sensitive B2G data.
- Inconsistent security standards across the legacy PHP monolith and new Go/Python microservices, potentially exposing **secrets or configuration flaws** during the critical migration period.
- High cloud operational costs (**FinOps**) are a top challenge, limiting investment capital if resources in EKS/Fargate environments are over-provisioned or misconfigured.

**TECHNICAL CONTEXT** (brief)
- Primary cloud platforms in use: **Amazon Web Services (AWS)**, leveraging EKS (Kubernetes), Fargate, and Lambda for cloud-native operations.
- Current security tools/vendors: Application security (Snyk, SonarQube), Identity (Okta), and network protection (Cloudflare).
- Notable tech stack elements relevant to cloud security: Core infrastructure managed via **Terraform (IaC)** and deployed through **GitLab CI/CD**; backend relies on Go and Python microservices.

***

*Analogy for Executive Context:* JustPark is building a global, real-time transportation hub where security and reliability are paramount. If their current technical foundation is like a large, successful UK train station built on legacy track (PHP monolith), the merger and AI strategy require them to simultaneously integrate a modern, high-speed rail network (ParkHub B2B, Go/Python microservices) while keeping the old lines running. **A unified cloud security posture is the signal system needed to prevent catastrophic collisions between the old and new systems, ensuring every train (transaction) arrives on time and safely, thereby protecting their reputation and expansion efforts.**.