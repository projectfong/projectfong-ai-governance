# ProjectFong AI Governance Framework (Public Research Release)

Author: projectfong  
Copyright (c) 2025 Fong  
License: ProjectFong Non-Commercial Research License (PNCRL-1.0)

---

## Summary

The **ProjectFong AI Governance Framework** defines a structured, evidence-driven approach to managing risk, audit, and accountability in artificial intelligence projects.
This public research release provides a **policy reference**, not production code.
It demonstrates how to implement transparent AI lifecycle governance aligned with **established cybersecurity frameworks and best practices (e.g., NIST SP 800-171 concepts)**.

---

## Purpose

* Establish a reference model for AI project governance and documentation.
* Demonstrate secure-by-default design principles and reproducible audit trails.
* Provide public insight into responsible AI management without exposing internal logic or data.
* Support educational and research exploration of trustworthy AI operations.

**License:** PNCRL-1.0 (research and educational use only).
**Commercial or derivative redistribution is prohibited without written authorization.**

---

## Repository Structure

| Path                                | Description                                                                    |
| ----------------------------------- | ------------------------------------------------------------------------------ |
| `AI_GOVERNANCE_FRAMEWORK_PUBLIC.md` | Primary policy framework document.                                             |
| `LICENSE-PNCRL-1.0.md`              | Research license and permitted-use terms.                                      |
| `DISCLAIMER-PNCRL-1.0.md`           | Warranty, limitation, and liability statement.                                 |
| `SECURITY-PNCRL-1.0.md`             | Conceptual security posture and isolation notes.                               |
| `NOTICE.md`                         | Attribution and ownership notice.                                              |
| `/evidence/` *(optional)*           | Internal-only directory for research logs and evidence retention per PNCRL §6. |

---

## Quick Start

### 1. View the Framework

Open [`AI_GOVERNANCE_FRAMEWORK_PUBLIC.md`](./docs/AI_GOVERNANCE_FRAMEWORK_PUBLIC.md) to review the governance lifecycle, roles, and evidence structure.

### 2. Review Legal Documents

* [LICENSE-PNCRL-1.0.md](./docs/LICENSE-PNCRL-1.0.md) — Research license terms
* [DISCLAIMER-PNCRL-1.0.md](./docs/DISCLAIMER-PNCRL-1.0.md) — Warranty and usage limits
* [SECURITY-PNCRL-1.0.md](./docs/SECURITY-PNCRL-1.0.md) — Isolation and audit guidance
* [NOTICE.md](./docs/NOTICE.md) — Ownership and attribution

### 3. Framework Alignment (Informational)

The Framework aligns with the following concept families derived from **NIST SP 800-171**:

* **Access Control (AC)** — role-based restrictions
* **Audit and Accountability (AU)** — event logging and verification
* **Configuration Management (CM)** — controlled documentation and change tracking
* **Identification and Authentication (IA)** — reviewer and role-based verification
* **Incident Response (IR)** — traceable review and mitigation actions

> **Note:** Alignment is for educational illustration only and does not constitute certification or compliance claim.

---

## Evidence Retention (Research Context)

Under PNCRL-1.0 §6, entities using this framework for study must:

* Maintain installation, access, and configuration logs.
* Store evidence under `/evidence/logs_YYYY-MM-DD`.
* Retain for at least **180 days** for internal review.

No production-level or personal data should be stored in this repository.

---

## Security and Isolation Highlights

* Least-privilege design and role-based separation.
* Audit logging for every governance decision.
* No secrets, credentials, or prompt logic exposed.
* Framework content is static and reproducible.

Detailed conceptual model: [`SECURITY-PNCRL-1.0.md`](./docs/SECURITY-PNCRL-1.0.md)

---

## Research Use Notice

This repository and its documentation are provided under PNCRL-1.0 for **non-commercial research and educational use**.
You may reference or adapt its structure for internal study, but redistribution or resale is prohibited.
Derived works must include the attribution:

> “Derived from Project Fong Research Work © 2025 Fong — used under PNCRL-1.0 for non-commercial research purposes.”

---

## Contact

For licensing or authorization inquiries:
**[fong.jobs@protonmail.com](mailto:fong.jobs@protonmail.com)**

---

## Revision Control

| Version | Date       | Summary                                       | Author      |
| ------- | ---------- | --------------------------------------------- | ----------- |
| 1.0.0   | 2025-10-29 | Initial publication of public research README | projectfong |

---
