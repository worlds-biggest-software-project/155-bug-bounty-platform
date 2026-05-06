# Bug Bounty Platform — Feature & Functionality Survey

> Candidate #155 · Researched: 2026-05-03

## Solutions Analysed

| Tool | Type | Licence / Model | URL |
|------|------|-----------------|-----|
| HackerOne | Commercial SaaS | Proprietary; enterprise licensing | https://www.hackerone.com |
| Bugcrowd | Commercial SaaS | Proprietary; enterprise licensing | https://www.bugcrowd.com |
| Intigriti | Commercial SaaS | Proprietary; pay-for-impact model | https://www.intigriti.com |
| Synack | Commercial SaaS | Proprietary; flat-fee model | https://www.synack.com |
| Immunefi | Commercial SaaS | Proprietary; percentage-based for Web3 | https://immunefi.com |
| YesWeHack | Commercial SaaS | Proprietary; enterprise licensing | https://www.yeswehack.com |

## Feature Analysis by Solution

### HackerOne

**Core features**
- Vulnerability report submission and tracking with embedded forms
- Automated workflow management prioritized by CVSS severity
- Dashboard and analytics for tracking vulnerability trends
- AI-powered triage assistance (Hai copilot) for report summarization and recommendations
- Integration with developer tools (JIRA, Slack, etc.)
- Managed vulnerability disclosure program (VDP) offering with free Essential tier entry point
- Programme management and researcher communication tools
- Remediation assistance and vulnerability scanning templates

**Differentiating features**
- GenAI copilot (Hai) built into platform for summarization, remediation advice, and scanner template generation
- Record-breaking researcher pool (~38% market share); largest programme count
- h1 Validation product specifically designed to filter AI-generated low-quality submissions
- Extensive integration ecosystem

**UX patterns**
- Tiered onboarding: free Essential VDP tier for organizations starting disclosure programmes
- Dashboard-first design emphasizing trend analysis and report prioritization
- In-platform AI assistant reducing manual writing and triage workload

**Integration points**
- Embedded submission forms for external reporters
- API integrations with JIRA, Slack, and other development tools
- Vulnerability scanner template export for regression testing

**Known gaps**
- Managing surge in AI-generated noise from commodity tools
- Handling record submission volumes (76% YoY growth in 2026)

**Licence / IP notes**
- Proprietary SaaS model; no open-source components identified

---

### Bugcrowd

**Core features**
- Vulnerability report submission with embedded submission forms
- Submission state tracking (New, Processing, Accepted, Rejected)
- VRT (Vulnerability Rating Taxonomy) severity classification (1-5 scale)
- Priority-based routing (P1-P5)
- Triage and validation workflow with communication logs
- Crowdcontrol dashboard for submission management
- Engineered triage process
- Integration with JIRA, Slack, and other tools
- Analytics and reporting for clients and researchers

**Differentiating features**
- Specialized machine learning for high-confidence duplicate detection
- Critical-issue escalation automation
- Flexible programme customization across diverse industries
- Strong integration depth with development toolchains

**UX patterns**
- Submission-centric dashboard showing state, priority, and history
- Progressive disclosure of validation checks and triage details
- Streamlined workflow optimized for rapid validation of critical issues

**Integration points**
- Embedded submission form integration for streamlined intake
- JIRA, Slack, and development tool connectors
- API access for custom integrations

**Known gaps**
- Smaller researcher pool compared to HackerOne
- Limited mention of AI-powered features versus competitors

**Licence / IP notes**
- Proprietary SaaS model; no open-source components identified

---

### Intigriti

**Core features**
- Managed vulnerability triage with expert review team
- VDP programme management with templates and automated workflows
- Submission capture and organization
- Vulnerability analytics for security posture improvement
- Bug Bounty, Managed VDP, Penetration Testing as a Service (PTaaS), Focused Sprints, and Live Hacking Events
- Flexible programme offerings tailored to client needs
- Triage standards and quality metrics

**Differentiating features**
- Expert triage team validates every submission before client sees it, eliminating false positives
- Pay-for-impact pricing model (only pay for valid vulnerabilities)
- Managed triage saved customers over 20,000 hours in 2025 by filtering invalid reports
- European headquarters with strong GDPR and compliance posture
- Comprehensive managed service approach beyond platform alone

**UX patterns**
- Quality-gate approach: triage team pre-filters for clients
- Metrics-driven: triage standards published and measurable
- Service-bundled offering allowing flexible engagement models

**Integration points**
- Workflow management with templates
- VDP policy generation and management
- Analytics export and reporting

**Known gaps**
- Less brand recognition outside Europe
- Smaller global researcher base compared to HackerOne/Bugcrowd

**Licence / IP notes**
- Proprietary SaaS model with managed service layer; no open-source components identified

---

### Synack

**Core features**
- Invite-only vetted researcher network (Red Team model)
- Multi-step researcher vetting (background check, skills assessment)
- Hybrid testing model combining human + AI-powered scanning
- On-demand penetration testing with flexible engagements
- Continuous security testing capabilities
- LaunchPoint VPN infrastructure for secure testing access
- Visibility and oversight of all researcher activities
- Flat-fee pricing model to customers; researchers paid per-finding

**Differentiating features**
- Highest researcher vetting bar (acceptance rate well below 10%)
- 1,500+ carefully vetted Red Team members
- Hybrid human-AI testing approach
- Continuous testing model designed for ongoing vulnerability discovery
- Predictable cost structure (flat-fee to clients)

**UX patterns**
- Gated access model: only pre-vetted researchers participate
- Secure communication infrastructure (LaunchPoint VPN)
- Activity visibility dashboard for transparency
- Continuous engagement model

**Integration points**
- LaunchPoint VPN for secure testing connections
- Communication and verification tools for recreating findings

**Known gaps**
- High premium pricing limits accessibility for smaller organizations
- Smaller programme count than HackerOne/Bugcrowd
- Limited public information on specific platform features

**Licence / IP notes**
- Proprietary SaaS model with patented testing infrastructure; no open-source components identified

---

### Immunefi

**Core features**
- Smart contract and Web3-focused bug bounty programmes
- Vaults system for on-chain proof-of-assets and on-chain payouts
- Safe Harbor legal framework for whitehat rescue funds during attacks
- PR Reviews, Audits, Audit Competitions
- Invite-Only programmes
- Managed Triage services
- IMU governance token (launched January 2026) for staking and voting on platform upgrades
- Critical bug reward structure (10% of funds affected, up to $50,000 maximum)

**Differentiating features**
- Decentralized Vaults system allowing on-chain payments and asset demonstration
- Safe Harbor legal framework unique to Web3/DeFi space
- Massive bounty pools ($100M+ paid out, protecting $180B in assets across 650+ protocols)
- Blockchain-native reward structures
- Native governance token enabling decentralized governance

**UX patterns**
- On-chain integration: vaults and payments via smart contracts
- Legal framework (Safe Harbor) reducing friction for whitehat activities
- Decentralized governance through IMU staking

**Integration points**
- Smart contract-based vault system
- On-chain payment infrastructure
- Web3 wallet integration for researcher payments
- Protocol asset management tools

**Known gaps**
- Limited applicability outside blockchain/Web3 space
- Smaller applicability to traditional software security
- High complexity for non-Web3 organizations

**Licence / IP notes**
- Proprietary SaaS with blockchain infrastructure; no open-source components identified

---

### YesWeHack

**Core features**
- Bug Bounty crowdsourcing with 135,000+ global ethical hackers
- Vulnerability Disclosure Policy (VDP) programme creation and management
- Pentest Management aggregating reports from all sources
- Attack Surface Management (ASM) with continuous exposure mapping
- Dojo ethical hacking training platform with lab-style learning
- Autonomous and continuous pentesting
- Unified vulnerability management workflows
- Cost-efficient platform-driven model

**Differentiating features**
- Integrated exposure management and attack surface discovery
- Dojo training module enabling researchers to practice on real-world scenarios
- Comprehensive security posture platform (not just bug bounty)
- EU-hosted infrastructure with strong compliance (ISO 27001, ISO 27017, GDPR, SOC 2 Type II)
- CREST accreditation
- Financial traceability and audit trails

**UX patterns**
- Integrated platform approach: bug bounty + VDP + ASM + training
- Lab-style hands-on learning (Dojo)
- Compliance-first design with audit and traceability built-in

**Integration points**
- API-based integration for unified workflows
- Pentest report aggregation from external sources
- Attack surface mapping and exposure detection

**Known gaps**
- Smaller researcher base compared to HackerOne/Bugcrowd
- Less market presence in non-European regions

**Licence / IP notes**
- Proprietary SaaS model; no open-source components identified. ISO certifications: ISO 27001, ISO 27017, ISO 27018, ISO 27701; SOC 2 Type II compliance

---

## Cross-Cutting Feature Themes

### Table-Stakes Features

- Vulnerability report submission form and intake mechanism
- Submission state tracking (new, in-progress, accepted, rejected, paid)
- Severity classification (CVSS or equivalent)
- Communication and collaboration tools between programme and researchers
- Triage workflow with review and approval stages
- Payment processing and payout management
- Dashboard and analytics for programmes and researchers
- Researcher reputation/ranking system visible to programmes
- Integration with common development tools (JIRA, Slack)
- Programme scope and policy definition tools
- Mobile-responsive design
- API for external integrations

### Differentiating Features

- AI-powered triage assistance (summarization, duplicate detection, severity estimation)
- Managed triage services (human-expert review of all submissions before programme sees)
- Researcher vetting and invite-only models for quality control
- On-chain payment infrastructure and decentralized governance (Web3)
- Comprehensive exposure management and attack surface integration
- Continuous testing and ongoing vulnerability discovery (vs. event-based)
- Training and certification platforms for researcher skill development
- Integrated pentest management and report aggregation
- Advanced analytics and benchmarking against industry peers
- Hybrid human-AI testing approaches

### Underserved Areas / Opportunities

- **AI submission quality filtering**: While HackerOne and Bugcrowd have started addressing AI-generated noise, this remains an acute pain point across all platforms as of 2026. A platform excelling at AI-quality discrimination could capture significant market value
- **Researcher onboarding and skill development**: Beyond Dojo (YesWeHack), limited platforms systematize researcher training; opportunity for integrated learning paths tied to bounty success
- **Regulatory compliance automation**: EU regulatory pressure (Cyber Resilience Act, GDPR) is driving VDP adoption, but most platforms require manual policy configuration; automated policy generation and compliance checking is emerging
- **Reproducibility verification**: Most triage is manual; automated PoC reproducibility testing in sandboxed environments could accelerate triage and reduce false submissions
- **Real-time duplicate detection at submission time**: Most platforms detect duplicates post-submission; catching them during intake could reduce noise further
- **Cross-programme vulnerability tracking**: No unified view of duplicate/related findings across multiple programmes a researcher or organization participates in
- **Natural-language PoC translation**: Lower-experienced researchers struggle to structure reports; AI-assisted PoC writing and evidence gathering could raise overall quality

### AI-Augmentation Candidates

- **Duplicate detection**: Currently manual or rules-based; LLM-powered semantic duplicate detection could exceed deterministic approaches
- **Severity estimation and CVSS assignment**: LLMs could infer severity from PoC and impact description, propose CVSS scores for human review
- **Report summarization and structured extraction**: Extract key details (vulnerability class, affected component, impact) into machine-readable format
- **Automated PoC reproducibility testing**: AI agents could attempt to reproduce reported exploits in sandboxed clones, providing pass/fail before human triage
- **Researcher reputation scoring**: Analyse historical submission data (acceptance rates, average severity, false-positive ratio) to weight researcher credibility
- **Policy and scope recommendations**: Analyse organization's asset inventory and past vulnerability history to suggest appropriate scope, reward bands, and OWASP coverage
- **Compliance checking**: Validate VDP policies against CVD standards, ISO 29147/30111, and evolving regulation (Cyber Resilience Act)
- **Researcher skill matching**: Match researcher specializations (Web3, API security, infrastructure) to programme scope for targeted outreach

---

## Legal & IP Summary

All six major platforms operate as proprietary SaaS offerings. No open-source bug bounty platforms of comparable maturity were identified during research. HackerOne and Bugcrowd reference standard security frameworks (CVSS, CVD, OWASP Top 10, ISO 29147/30111) which are publicly available and license-compatible. Immunefi's Vaults system and Safe Harbor legal framework are proprietary innovations specific to blockchain; no patent encumbrances were identified. YesWeHack operates under strict EU compliance (GDPR, ISO certifications) and is CREST-accredited; UK/EU data handling and legal review may be required if operating in those jurisdictions. No copyright, licensing, or patent conflicts identified for features discussed in research.

---

## Recommended Feature Scope

Based on the above, here is a prioritised feature scope for a new bug bounty platform project:

**Must-have (MVP)**
- Submission intake form with customizable fields (title, description, PoC, steps to reproduce, impact)
- Submission state machine (new → triage → accepted/rejected → paid)
- CVSS severity classification interface with guidance
- Programme policy and scope definition tools
- Researcher ranking and reputation display
- Payment processing integration (PayPal, bank transfer, crypto)
- Dashboard for both programme and researcher views
- Communication and notes system between programme and researcher
- JIRA integration for remediation workflow

**Should-have (v1.1)**
- AI-powered triage assistant (duplicate detection, severity proposal, summary generation)
- Automated PoC reproducibility testing in sandboxed container
- Researcher reputation scoring (submission quality analysis, false-positive detection)
- VDP policy auto-generation from scope and compliance templates
- Compliance validation against CVD, ISO 29147, and regional requirements (GDPR, Cyber Resilience Act)
- Advanced analytics dashboard with benchmarking against peers
- Slack/Teams integration for notifications
- Researcher skill tagging and programme-to-researcher matching
- Multi-programme duplicate tracking

**Nice-to-have (backlog)**
- Continuous testing engagement model (vs. event-based)
- Researcher training platform (Dojo-style labs)
- Attack surface management integration
- Decentralized governance token (for premium tier)
- On-chain payment infrastructure (Web3 expansion)
- Invite-only vetted researcher tier
- Managed triage service (human expert review layer)
- Advanced hybrid human-AI testing orchestration
- Real-time PoC translation and structured evidence extraction
