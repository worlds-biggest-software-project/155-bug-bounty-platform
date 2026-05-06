# Standards & API Reference

> Project: Bug Bounty Platform · Generated: 2026-05-03

## Industry Standards & Specifications

### ISO Standards

- **ISO/IEC 29147:2018 — Vulnerability Disclosure** — The primary international standard for coordinated vulnerability disclosure (CVD); defines the guidelines, methods, and policies vendors should use to receive vulnerability reports and publish remediation information; directly governs how bug bounty programmes handle researcher submissions, triage timelines, and public disclosure. URL: https://www.iso.org/standard/72311.html

- **ISO/IEC 30111:2019 — Vulnerability Handling Processes** — Companion standard to ISO 29147; defines the internal processes for handling received vulnerability reports (assessment, prioritisation, remediation, verification); relevant to the backend workflow of bug bounty programme management. URL: https://www.iso.org/standard/69725.html

- **ISO/IEC 27001:2022** — Information security management systems; Annex A control A.5.8 (Information security in project management) and A.8.8 (Management of technical vulnerabilities) require systematic handling of discovered vulnerabilities including those found through bug bounty programmes. URL: https://www.iso.org/standard/82875.html

### W3C & IETF Standards

- **RFC 9116 — security.txt** — IETF standard (2022) specifying a `/.well-known/security.txt` file format for publishing vulnerability disclosure contact information, encryption keys, policy URLs, and bug bounty programme links; used by all major bug bounty platforms as a discoverable entry point. URL: https://datatracker.ietf.org/doc/html/rfc9116

- **RFC 6749 — OAuth 2.0** — Authorization framework used by bug bounty platform APIs (HackerOne, Bugcrowd) for authenticated programme management, webhook delivery, and integration with security orchestration tools. URL: https://datatracker.ietf.org/doc/html/rfc6749

- **RFC 7519 — JSON Web Token (JWT)** — Used in bug bounty platform API authentication flows and webhook payload signing. URL: https://datatracker.ietf.org/doc/html/rfc7519

- **JSON:API Specification** — HackerOne's REST API is compliant with the JSON:API specification for consistent request/response formatting, relationships, pagination, and filtering of programme, report, and bounty objects. URL: https://jsonapi.org/

### Data Model & API Specifications

- **CVSS 4.0 — Common Vulnerability Scoring System** — FIRST.org standard for rating vulnerability severity; used universally by bug bounty platforms for bounty table definitions (reward tiers keyed to CVSS Base score or severity label); CVSS 4.0 Base + Threat scoring is replacing CVSS 3.1 as the submission standard. URL: https://www.first.org/cvss/

- **OWASP Top 10 (2021)** — De facto standard defining the ten most critical web application security risk categories; used as a reference taxonomy for vulnerability classification in bug bounty programme scope definitions and submission categorisation. URL: https://owasp.org/Top10/

- **OWASP API Security Top 10 (2023)** — Defines the ten most critical API security risks; increasingly used by programmes with API-specific scope to classify and prioritise researcher submissions. URL: https://owasp.org/API-Security/

- **OWASP Vulnerability Disclosure Cheat Sheet** — Practical guidance for implementing coordinated disclosure policies aligned with ISO 29147; widely referenced by bug bounty programme managers for crafting Safe Harbour clauses and responsible disclosure policies. URL: https://cheatsheetseries.owasp.org/cheatsheets/Vulnerability_Disclosure_Cheat_Sheet.html

- **OpenAPI 3.1** — Used by HackerOne and Bugcrowd to describe their customer and hacker REST APIs; enables SDK generation, Postman collection creation, and CI/CD integration for automated vulnerability management workflows. URL: https://spec.openapis.org/oas/latest.html

- **CWE — Common Weakness Enumeration** — MITRE standard for classifying software weaknesses; used in bug bounty report templates for root-cause categorisation alongside CVE identifiers for known vulnerabilities. URL: https://cwe.mitre.org/

### Security & Authentication Standards

- **CISA BOD 20-01 — Developing and Publishing a Vulnerability Disclosure Policy** — US federal directive (2020) requiring all federal civilian agencies to publish a vulnerability disclosure policy (VDP); mandated use of Bugcrowd or HackerOne-hosted VDP programmes across dozens of US agencies; set the global precedent for mandatory CVD programmes. URL: https://cyber.dhs.gov/bod/20-01/

- **EU Cyber Resilience Act (CRA) — Articles 13 & 14** — Requires manufacturers of connected products to have a vulnerability disclosure policy and coordinated vulnerability disclosure process; encourages bug bounty programmes as a CVD mechanism; applicable to products sold in the EU from 2027. URL: https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32024R2847

- **EU NIS2 Directive — Article 12** — Requires coordinated vulnerability disclosure frameworks at national level; member states must designate a CSIRT as coordinator; encourages sector operators to maintain CVD/VDP policies compatible with bug bounty platforms. URL: https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32022L2555

- **UK PSTI Act 2022 — Product Security and Telecommunications Infrastructure Act** — Requires consumer IoT device manufacturers to have a vulnerability disclosure policy; bug bounty platforms (HackerOne, Bugcrowd) offer PSTI-compliant VDP programme templates. URL: https://www.legislation.gov.uk/ukpga/2022/46

- **disclose.io Safe Harbour Framework** — Open-source (CC0) legal framework adopted by 300+ organisations for providing researchers with good-faith legal protection during vulnerability research; the standard Safe Harbour clause template used in bug bounty and VDP policy documents. URL: https://disclose.io/

- **NIST CSF 2.0 — ID.RA (Identify: Risk Assessment)** — Continuous risk identification functions align with bug bounty programmes as a crowd-sourced vulnerability discovery mechanism; GV.RM (Govern: Risk Management) covers the programme management aspect. URL: https://www.nist.gov/cyberframework

- **GDPR Article 32 — Security of Processing** — Bug bounty platforms must handle vulnerability reports (which contain sensitive technical details about client systems) with appropriate confidentiality, integrity, and access controls; platforms must have data processing agreements with programme customers. URL: https://gdpr-info.eu/art-32-gdpr/

### MCP Server Specifications

Bug bounty and vulnerability disclosure is an emerging area for AI-assisted workflows:

- **Emerging AI Triage Integration**: Bug bounty platforms are beginning to integrate AI for automated vulnerability report triage, duplicate detection, and severity pre-scoring; MCP server integration patterns are expected for connecting AI triage agents to vulnerability management and JIRA-style ticketing systems (not yet standardised as of May 2026).

- **bounty-targets-data (Open Source)** — Community-maintained hourly-updated data dumps of bug bounty platform scopes (HackerOne, Bugcrowd, Intigriti, YesWeHack) in JSON format; used by AI-assisted recon tools to enumerate eligible test targets. URL: https://github.com/arkadiyt/bounty-targets-data

---

## Similar Products — Developer Documentation & APIs

### HackerOne

- **Description:** The world's largest bug bounty and vulnerability disclosure platform; over 2 million registered hackers; manages private and public programmes, VDPs, and AI Red Teaming engagements; serves Fortune 500 companies and US federal agencies.
- **API Documentation:** https://api.hackerone.com/
- **Customer API Reference:** https://api.hackerone.com/customer-reference/
- **Hacker API Reference:** https://api.hackerone.com/hacker-reference/
- **SDKs/Libraries:** Ruby gem; Python examples; JSON:API compliant REST; Brinqa connector; April 2026: bounty table REST endpoint; February 2026: automation management REST endpoints added
- **Developer Guide:** https://api.hackerone.com/getting-started/
- **Standards:** REST/JSON (JSON:API compliant), OpenAPI, OAuth 2.0
- **Authentication:** HTTP Basic Auth (API token identifier + value generated from Program Settings)

### Bugcrowd

- **Description:** Leading bug bounty and vulnerability disclosure platform; serves enterprise organisations and US government agencies; hosts VDPs compliant with CISA BOD 20-01, HIPAA, SOX, GLBA (US), PSTI (UK), and DORA/NIS2/CRA (EU).
- **API Documentation:** https://docs.bugcrowd.com/api/
- **Advanced API Docs:** https://docs.bugcrowd.com/changelog/api/advanced-api-documentation/
- **SDKs/Libraries:** REST API (versioned, current version 2024-07-11); webhook support; Brinqa connector
- **Developer Guide:** https://docs.bugcrowd.com/
- **Standards:** REST/JSON, OpenAPI, webhook events
- **Authentication:** API key (Bearer token); webhook HMAC signature verification

### Intigriti

- **Description:** Europe's leading bug bounty platform with 50,000+ ethical hackers; strong in EMEA and APAC markets; offers private and public programmes across financial services, retail, government, and technology sectors.
- **API Documentation:** https://kb.intigriti.com/en/articles/6346027-intigriti-api (requires account)
- **SDKs/Libraries:** REST API; personal access tokens; bbscope community tool integration
- **Developer Guide:** https://kb.intigriti.com/
- **Standards:** REST/JSON, OpenAPI, OAuth 2.0 / personal access tokens
- **Authentication:** Personal Access Token (generated from https://app.intigriti.com/researcher/personal-access-tokens)

### YesWeHack

- **Description:** European bug bounty platform (France-based) with significant presence in EMEA and APAC; strong public sector and government programme portfolio; offers VDP and bug bounty programme management with API access.
- **API Documentation:** https://api.yeswehack.com/ (REST API with OpenAPI spec)
- **SDKs/Libraries:** REST API; webhook integrations; community scope tools (bbscope)
- **Developer Guide:** https://yeswehack.com/developers
- **Standards:** REST/JSON, OpenAPI
- **Authentication:** JWT Bearer token (OAuth 2.0 password grant or API token)

### Immunefi

- **Description:** Leading Web3 and blockchain bug bounty platform; specialises in DeFi protocols, NFT projects, and smart contract security; highest bounty payouts in the industry (up to $10M+ for critical smart contract vulnerabilities).
- **API Documentation:** https://immunefi.com/api/ (public JSON programme listings)
- **SDKs/Libraries:** Public JSON feed of all programmes and bounties; bbscope community integration
- **Developer Guide:** https://immunefi.com/
- **Standards:** REST/JSON; Ethereum/Solidity audit standards; on-chain payment via crypto
- **Authentication:** API key for programme management; public read endpoints unauthenticated

### Synack Red Team Platform

- **Description:** Managed platform combining crowd-sourced security researchers with automated scanning; curated vetted researcher pool (Synack Red Team); strong in enterprise application testing and AI/LLM red teaming; structured programme management with compliance reporting.
- **API Documentation:** https://platform.synack.com/api (requires account)
- **SDKs/Libraries:** REST API; JIRA/ServiceNow integrations; webhook support
- **Developer Guide:** Synack platform portal (account required)
- **Standards:** REST/JSON, OpenAPI, OAuth 2.0
- **Authentication:** OAuth 2.0 (platform SSO); API key for programme integrations

### Open Bug Bounty

- **Description:** Open, non-commercial, and non-profit platform for coordinated vulnerability disclosure; free for researchers and website owners; focuses on XSS and CSRF vulnerabilities across public websites; no bounty payments — recognition-based only.
- **API Documentation:** https://www.openbugbounty.org/api/ (public REST API)
- **SDKs/Libraries:** Public REST API returning JSON/XML; no authentication required for public data
- **Developer Guide:** https://www.openbugbounty.org/api/
- **Standards:** REST/JSON, XML, ISO 29147 aligned
- **Authentication:** None for public endpoints; registration required for submissions

### disclose.io Platform Catalogue

- **Description:** Open-source (CC0) collection of bug bounty and VDP platforms and their policies; maintained by the security community; provides Safe Harbour legal framework templates widely adopted across commercial and open platforms.
- **Platform Catalogue:** https://platforms.disclose.io/
- **Safe Harbour Framework:** https://disclose.io/
- **Standards:** CC0, ISO 29147 aligned, RFC 9116 (security.txt)
- **Authentication:** Not applicable (public resource)

---

## Notes

- **RFC 9116 (security.txt) as infrastructure standard**: RFC 9116 has become the primary mechanism for publishing bug bounty and VDP contact information; all major platforms generate a `security.txt` file as part of programme setup. Adoption has increased significantly since CISA BOD 20-01 mandated it for US federal agencies.

- **EU regulatory push (2025-2027)**: The EU Cyber Resilience Act (effective 2027) will require all connected product manufacturers to maintain CVD policies compatible with bug bounty platforms; NIS2 mandates national CVD frameworks; this is driving significant European bug bounty programme growth.

- **AI-assisted triage (2025-2026)**: Bug bounty platforms are integrating AI for automated duplicate detection, severity pre-scoring (CVSS), and report quality assessment to reduce triage workload; HackerOne's February 2026 automation management API release is a marker of this trend.

- **Web3 specialisation**: Immunefi's dominance in smart contract and DeFi bug bounties represents a distinct sub-category with different technical standards (Solidity audits, on-chain payment) from traditional web application programmes.

- **Open-source landscape**: There is no dominant open-source self-hosted bug bounty platform comparable to HackerOne or Bugcrowd; Bugdisclosure.org and Open Bug Bounty serve open VDP roles; self-hosted options are typically custom-built on issue trackers (GitLab, Jira) with VDP policies.
