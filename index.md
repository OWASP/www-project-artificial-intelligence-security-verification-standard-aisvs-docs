---

layout: col-sidebar
title: OWASP Artificial Intelligence Security Verification Standard AISVS Docs
tags: AI, LLM, Security, AISVS
level: 2
type: documentation
pitch: OWASP AI verification standard for developers and testers

---

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="images/aisvs-logo-dark.png">
    <source media="(prefers-color-scheme: light)" srcset="images/aisvs-logo-light.png">
    <img alt="OWASP AISVS Logo" src="images/aisvs-logo-light.png" width="520">
  </picture>
</p>

The **Artificial Intelligence Security Verification Standard (AISVS)** is an
open catalogue of testable security requirements for AI-enabled systems. It
helps developers, architects, security engineers, and auditors design, build,
test, and verify AI applications throughout their lifecycle, from data
collection and model training to deployment, monitoring, and retirement.

Every requirement is verifiable, testable, and implementable.

This site is the public documentation wrapper for the main
[OWASP/AISVS](https://github.com/OWASP/AISVS) content repository.

### How to use AISVS

* **Design.** Use it as a security checklist when architecting AI systems.
* **Development.** Integrate it into CI/CD pipelines, code reviews, and tests.
* **Assessment.** Apply it as a verification framework for pen testing and audits.
* **Procurement.** Reference specific requirements when evaluating AI vendors and third-party models.

### Verification Levels

Each requirement is assigned a level (1, 2, or 3) indicating depth of assurance.

<table>
  <thead>
    <tr>
      <th style="white-space:nowrap; text-align:center;">Level</th>
      <th>Description</th>
      <th>When to use</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:center;"><strong>1</strong></td>
      <td>Essential baseline controls every AI system should implement.</td>
      <td>All AI applications, including internal tools and low-risk systems.</td>
    </tr>
    <tr>
      <td style="text-align:center;"><strong>2</strong></td>
      <td>Standard controls for systems handling sensitive data or making consequential decisions.</td>
      <td>Production systems, customer-facing AI, systems processing personal data.</td>
    </tr>
    <tr>
      <td style="text-align:center;"><strong>3</strong></td>
      <td>Advanced controls for high-assurance environments facing sophisticated threats.</td>
      <td>Critical infrastructure, safety-critical AI, regulated industries.</td>
    </tr>
  </tbody>
</table>

Most production systems should aim for at least Level 2.

### Requirement Chapters

1. [Training Data Governance & Bias Management](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C01-Training-Data-Integrity-and-Traceability.md)
2. [User Input Validation](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C02-Input-Validation.md)
3. [Model Lifecycle Management & Change Control](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C03-Model-Lifecycle-Management.md)
4. [Infrastructure, Configuration & Deployment Security](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C04-Infrastructure.md)
5. [Access Control & Identity](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C05-Access-Control-and-Identity.md)
6. [Supply Chain Security for Models, Frameworks & Data](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C06-Supply-Chain.md)
7. [Model Behavior, Output Control & Safety Assurance](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C07-Model-Behavior.md)
8. [Memory, Embeddings & Vector Database Security](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C08-Memory-Embeddings-and-Vector-Database.md)
9. [Autonomous Orchestration & Agentic Action Security](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C09-Orchestration-and-Agentic-Action.md)
10. [MCP Security](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C10-MCP-Security.md)
11. [Adversarial Robustness & Attack Resistance](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C11-Adversarial-Robustness.md)
12. [Privacy Protection & Personal Data Management](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C12-Privacy.md)
13. [Monitoring, Logging & Anomaly Detection](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C13-Monitoring-and-Logging.md)
14. [Human Oversight and Trust](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x10-C14-Human-Oversight.md)

### Appendices

* [Appendix A: Glossary](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x90-Appendix-A_Glossary.md)
* [Appendix B: References](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x91-Appendix-B_References.md)
* [Appendix C: AI-Assisted Secure Coding](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x92-Appendix-C_AI_for_Code_Generation.md)
* [Appendix D: AI Security Controls Inventory](https://github.com/OWASP/AISVS/blob/main/1.0/en/0x93-Appendix-D_AI_Security_Controls_Inventory.md)

### Road Map

| Phase | Status | Focus |
| --- | --- | --- |
| Phase 1: Research and Category List Creation | Done | Establish the research base and define the AISVS category structure. |
| Phase 2: Requirement Creation | Current Phase | Create requirements for each category and refine them with community, partner, and subject matter expert input. |
| Phase 3: Beta Release and Pilot Testing | Planned | Release a beta version of AISVS and gather feedback from early adopters using it on real-world AI applications. |
| Phase 4: Final 1.0 Release | Planned | Incorporate pilot feedback and publish Version 1.0 with full documentation and a lightweight checklist. |
| Phase 5: Continuous Improvement | Ongoing | Maintain AISVS as an open source project and update it to address emerging threats, new AI approaches, and regulatory change. |
