# ProjectFong AI Governance Framework — Security and Isolation Notes  
Author: projectfong  
Copyright (c) 2025 Fong  
All Rights Reserved  
License: ProjectFong Non-Commercial Research License (PNCRL-1.0)

---

## Summary
Describes the conceptual security posture for the AI Governance Framework public research release.  
Focuses on isolation, least privilege, audit logging, and evidence assurance.

---

## Design Principles
* **Secure-by-default:** minimal privilege, no network trust assumptions.  
* **Auditability:** every governance action logged with timestamp.  
* **Transparency:** no hidden logic or unlogged execution paths.  
* **Reproducibility:** configuration and evidence hashes verifiable.

---

## Isolation Overview
| Layer | Purpose | Trust Boundary |
|-------|----------|----------------|
| Frontend/UI | User interaction | External zone |
| API Gateway (Go) | RBAC + mTLS | Ingress zone |
| Orchestrator (Python) | Logic execution | Internal zone |
| Database (SQL) | Evidence storage | Data zone |
| Filesystem | Immutable logs | Audit zone |

---

## Logging Policy
* JSON-formatted events: `timestamp, component, user, action, status, sha256_event_id`.  
* Retention: 180 days minimum.  
* Secrets, PII, and LLM prompts not stored in clear text.

---

## Vulnerability and Configuration
* Dependency verification (`go mod verify`, `pip check`).  
* `.env` files never committed; access read-only at runtime.  
* Linux containers non-root UID > 1000; read-only filesystem except `/evidence/`.

---

## Compliance Mapping (Informational)
| Control Family | Objective | Implementation Summary |
|----------------|-----------|-------------------------|
| AC | Restrict access by role | JWT + mTLS |
| AU | Audit events | JSON logs with hash integrity |
| CM | Baseline control | Git tracking + .env validation |
| IA | AuthN/AuthZ | Token claims + cert trust |
| IR | Incident response | Evidence log review |

---

## Revision Control
| Version | Date | Summary | Author |
|---------|------|----------|--------|
| 1.0.0 | 2025-10-29 | Initial publication for PNCRL research security notes | projectfong |
