# Bug Bounty Platform

> Part of the [worlds-biggest-software-project](https://github.com/worlds-biggest-software-project) initiative.
>
> An AI-native, open-source bug bounty platform that filters submission noise, accelerates triage, and brings vulnerability disclosure programmes within reach of smaller organisations.

The Bug Bounty Platform provides researcher onboarding, submission triage, and reward management for organisations running vulnerability disclosure and bug bounty programmes. It is built for AppSec teams, CISOs, and security-conscious engineering organisations who need a credible programme without the per-bounty premiums and lock-in of incumbent SaaS platforms.

---

## Why Bug Bounty Platform?

- Incumbent platforms (HackerOne, Bugcrowd, Synack) charge USD 15,000–50,000 per year in platform fees plus 20–30% of every bounty paid, pricing mid-market organisations out of credible programmes.
- AI-generated low-quality submissions are an acute, industry-wide operational pain in 2026; platforms are still catching up, and there is room for a system designed around AI-quality discrimination from day one.
- No open-source bug bounty platforms of comparable maturity exist — every major incumbent is proprietary SaaS, leaving self-hostable and regulator-friendly deployments unaddressed.
- EU regulatory pressure (Cyber Resilience Act, GDPR) is driving VDP adoption, but most platforms still require manual policy configuration.
- Researcher onboarding and skill development is systematised by only one major platform (YesWeHack's Dojo), leaving a clear gap for integrated learning paths tied to bounty success.

---

## Key Features

### Submission Intake and Triage

- Customisable submission intake form covering title, description, PoC, reproduction steps, and impact
- Submission state machine: new → triage → accepted/rejected → paid
- CVSS severity classification interface with guidance
- Communication and notes system between programme and researcher
- Programme policy and scope definition tools

### AI-Powered Triage

- LLM-based duplicate detection at submission time, going beyond rules-based matching
- Severity estimation and CVSS proposals derived from PoC and impact descriptions
- Report summarisation and structured extraction of vulnerability class, affected component, and impact
- Automated PoC reproducibility testing in a sandboxed clone of the target, producing a pass/fail signal for triagers

### Researcher Management

- Researcher ranking and reputation display
- Reputation scoring driven by historical submission quality, accuracy, and novelty
- Researcher skill tagging and programme-to-researcher matching
- Programme dashboard and researcher dashboard views

### Payments and Workflow

- Payment processing integration (PayPal, bank transfer, crypto)
- JIRA integration for remediation workflow
- Slack/Teams integration for notifications
- Multi-programme duplicate tracking across programmes a researcher participates in

### Compliance and Policy

- VDP policy auto-generation from scope and compliance templates
- Compliance validation against CVD, ISO/IEC 29147, ISO/IEC 30111, GDPR, and the EU Cyber Resilience Act
- Advanced analytics dashboard with benchmarking against peers

---

## AI-Native Advantage

AI is woven through the platform rather than bolted on. An AI triage layer classifies incoming reports, estimates severity, and detects duplicates before human review — research suggests this can cut triage costs by 40–60%. An AI agent attempts to reproduce reported exploits in a sandboxed clone of the target, giving triagers a pass/fail signal. Natural-language to PoC assistance helps less-experienced researchers structure and evidence their reports, raising overall submission quality. A scoping assistant analyses an organisation's asset inventory and past vulnerability history to recommend scope, reward bands, and eligibility criteria.

---

## Tech Stack & Deployment

The platform is designed around open standards: CVSS for severity, ISO/IEC 29147 and ISO/IEC 30111 for vulnerability disclosure and handling, CVD for researcher-vendor coordination, and OWASP Top 10 / API Security Top 10 for scope templates. Sandboxed reproducibility testing runs in isolated containers. Integration is API-first, with connectors for JIRA, Slack, and Teams. Deployment targets include both self-hosted and managed cloud modes, with EU-hosted options for GDPR-bound buyers.

---

## Market Context

The bug bounty platforms market is estimated at USD 2.06 billion in 2026, projected to reach USD 5.7 billion by 2033 at a CAGR of approximately 15.8% (Business Research Insights, 2026). Incumbents charge USD 15,000–50,000 per year in platform fees plus 20–30% of bounty payouts, with managed triage at a premium. Primary buyers are CISOs and AppSec leads at mid-to-large enterprises, financial institutions and fintech, SaaS companies, government agencies mandating VDP policies, and blockchain protocol teams.

---

## Project Status

> This project is in the **research and specification phase**.  
> Contributions, feedback, and domain expertise are welcome.

---

## Contributing

We welcome contributions from developers, domain experts, and potential users.
See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

**Important:** All contributions must be your own original work or clearly attributed
open-source material with a compatible licence. Copyright infringement and licence
violations will not be tolerated and will result in immediate removal of the offending
contribution. If you are unsure whether a piece of code, text, or other material is
safe to contribute, open an issue and ask before submitting.

---

## Licence

Licence to be determined. See [discussion](#) for context.
