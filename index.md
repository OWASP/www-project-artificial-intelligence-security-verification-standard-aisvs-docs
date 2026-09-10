---

layout: col-sidebar
title: OWASP Artificial Intelligence Security Verification Standard (AISVS)
tags: aisvs, ai-security, llm-security, agentic-ai, mcp-security
level: 2
type: documentation
pitch: An open standard of testable security requirements for designing, building, and verifying AI systems, from training data to autonomous agents and MCP.

---

The OWASP Artificial Intelligence Security Verification Standard (AISVS) is an open, community-driven catalogue of testable security requirements for AI-enabled systems. It gives developers, architects, security engineers, and auditors one shared checklist for designing, building, testing, and verifying AI applications across their whole lifecycle: training data, model development, deployment, agent orchestration, monitoring, and retirement.

AISVS is modeled on the [OWASP Application Security Verification Standard (ASVS)](https://owasp.org/projects/asvs) and follows the same rule: every requirement must be verifiable, testable, and implementable. It is vendor-neutral, free to use, and published under the Creative Commons Attribution-ShareAlike 4.0 license.

## AISVS 1.0 is available now

AISVS 1.0 was released in June 2026 at the OWASP Global AppSec conference in Vienna. It contains 191 requirements across 12 chapters and three appendices, and every requirement carries a verification level of 1, 2, or 3.

* [Download the AISVS 1.0 PDF](https://github.com/OWASP/AISVS/raw/main/1.0/dist/AISVS-1.0.pdf)
* [Read AISVS 1.0 online](https://github.com/OWASP/AISVS/tree/main/1.0/en) in its Markdown source form
* [AISVS Research Wiki](https://github.com/OWASP/AISVS/blob/main/1.01-dev/research/README.md) with the threats mitigated, verification approach, and tooling notes for every requirement
* [Versioning and release policy](https://github.com/OWASP/AISVS/blob/main/RELEASE.md)

## How to use AISVS

* **Design.** Use the requirements as a security checklist when architecting AI systems and agents.
* **Development.** Turn requirements into acceptance criteria, code review checks, and automated tests in CI/CD pipelines.
* **Assessment.** Use AISVS as the verification framework for AI penetration tests, red-team exercises, and audits.
* **Procurement.** Reference specific requirement IDs when evaluating AI vendors, third-party models, and MCP servers.

AISVS is intentionally narrow. It covers only what is specific to AI and ML systems, and it assumes that general application, infrastructure, and supply-chain security are verified in parallel against ASVS and the other standards that own those topics.

## Verification levels

Every requirement is assigned one of three levels. Choose a target level based on the risk profile of the AI system; most production systems should aim for at least Level 2. AISVS levels are aligned with ASVS levels and are designed to be applied together at the matching level.

* **Level 1: Baseline.** Essential controls that every AI system should implement. For all AI applications, including internal tools and low-risk systems. 51 requirements.
* **Level 2: Standard.** Controls for systems that handle sensitive data or make consequential decisions. For production systems, customer-facing AI, and systems that process personal data. 95 requirements.
* **Level 3: Advanced.** Controls for high-assurance environments that face sophisticated attackers. For critical infrastructure, safety-critical AI, and regulated industries. 45 requirements.

## Requirement chapters

1. [C1: Training Data Integrity & Traceability](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C01-Training-Data-Integrity-and-Traceability.md)
2. [C2: Input Validation](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C02-Input-Validation.md)
3. [C3: Model Lifecycle Management & Change Control](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C03-Model-Lifecycle-Management.md)
4. [C4: Infrastructure, Configuration & Deployment Security](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C04-Infrastructure.md)
5. [C5: Access Control & Identity for AI Components & Users](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C05-Access-Control-and-Identity.md)
6. [C6: Supply Chain Security for Models](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C06-Supply-Chain.md)
7. [C7: Model Behavior, Output Control & Safety Assurance](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C07-Model-Behavior.md)
8. [C8: Memory, Embeddings & Vector Database Security](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C08-Memory-Embeddings-and-Vector-Database.md)
9. [C9: Orchestration & Agentic Security](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C09-Orchestration-and-Agentic-Action.md)
10. [C10: Model Context Protocol (MCP) Security](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C10-MCP-Security.md)
11. [C11: Adversarial Robustness](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C11-Adversarial-Robustness.md)
12. [C12: Monitoring, Logging & Anomaly Detection](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C12-Monitoring-and-Logging.md)

Three appendices support the chapters:

* [Appendix A: Glossary](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x90-Appendix-A_Glossary.md)
* [Appendix B: AI Security Controls Inventory](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x91-Appendix-B_AI_Security_Controls_Inventory.md), a cross-reference of every defense technique in AISVS
* [Appendix C: AI-Assisted Secure Coding](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x92-Appendix-C_AI_for_Code_Generation.md), controls for using AI coding tools safely

## Referencing a requirement

Each requirement has an identifier of the form `C<chapter>.<section>.<requirement>`, for example `C9.4.3`. Because identifiers can change between versions, include the version when you cite one: `v1.0-C9.4.3` refers unambiguously to requirement 9.4.3 of AISVS 1.0, "Verify that agent identity credentials rotate on a defined schedule."

## How AISVS relates to other standards

* **OWASP ASVS** covers web application security. AISVS extends the same approach to AI-specific threats and is meant to be applied alongside it.
* **[OWASP Top 10 for LLM Applications](https://genai.owasp.org/llm-top-10/)** and **[OWASP Top 10 for Agentic Applications](https://genai.owasp.org/resource/owasp-top-10-for-agentic-applications-for-2026/)** raise awareness of the most critical risks. AISVS supplies the detailed, testable controls that mitigate them.
* **[NIST AI RMF](https://www.nist.gov/itl/ai-risk-management-framework)** and **[ISO/IEC 42001](https://www.iso.org/standard/42001)** govern AI risk and management systems. AISVS provides the implementation-level security controls those frameworks point to.

AISVS is not a governance framework, not a risk management methodology, and not a list of recommended products.

## Road Map

* Phase 1: Research and category list creation (Done)
* Phase 2: Requirement creation with community, partner, and subject-matter-expert input (Done)
* Phase 3: Beta release and pilot testing on real-world AI applications (Done)
* Phase 4: Final 1.0 release with full documentation (Done, June 2026)
* Phase 5: Continuous improvement (Current phase). Maintain AISVS as an open standard, grow the Research Wiki, and prepare the [next minor release, 1.01](https://github.com/OWASP/AISVS/tree/main/1.01-dev), to address emerging threats, new AI architectures, and regulatory change.

## Get involved

AISVS is built in the open, and every contribution counts, from a typo fix to a new requirement.

* Join the [#project-aisvs channel on OWASP Slack](https://owasp.slack.com/archives/C08NKTCJT5E). New to OWASP Slack? Get an invite at [owasp.org/slack/invite](https://owasp.org/slack/invite).
* [Open an issue](https://github.com/OWASP/AISVS/issues) to report a problem or propose a requirement, then follow the [contributing guide](https://github.com/OWASP/AISVS/blob/main/CONTRIBUTING.md) to submit a pull request.
* Follow [@OWASP_AISVS on X](https://x.com/OWASP_AISVS) for release news.
* Report a vulnerability in the project's own scripts or infrastructure through the [security policy](https://github.com/OWASP/AISVS/blob/main/SECURITY.md). Reporters are credited in the [Hall of Fame](https://github.com/OWASP/AISVS/blob/main/HALL_OF_FAME.md).

Everyone participating in the project agrees to the [OWASP Code of Conduct](https://policy.owasp.org/operational/code-of-conduct).
