---
### ADR-013: Security Baseline — Encryption, Least Privilege, and Compliance Readiness

**Status:** Inferred
**Context:** Protecting data in transit and at rest, minimizing blast radius, and meeting regulatory expectations are foundational.
**Decision:** Enforce TLS 1.2+ everywhere, encrypt data at rest with managed keys, rotate secrets/keys regularly, and apply least-privilege IAM. Implement dependency and container scanning, SBOMs, and image signing. Maintain backups, tested restores, and defined RTO/RPO.
**Consequences:** Strong baseline and auditability. Operational overhead for key/secret rotation, scanning, and periodic recovery drills.