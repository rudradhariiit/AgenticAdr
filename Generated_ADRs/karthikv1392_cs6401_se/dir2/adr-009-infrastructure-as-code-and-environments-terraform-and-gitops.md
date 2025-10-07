---
### ADR-009: Infrastructure as Code and Environments — Terraform and GitOps

**Status:** Inferred
**Context:** Repeatability, auditability, and safe change management across multiple environments are mandatory.
**Decision:** Manage cloud resources with Terraform in a multi-environment structure (dev/stage/prod), with remote state and state locks. Apply GitOps or CI-driven change application, peer reviews, and drift detection. Separate blast radiuses by environment and account.
**Consequences:** Predictable, reviewable infra changes and easier compliance. Requires disciplined workflows, state management, and secret hygiene.