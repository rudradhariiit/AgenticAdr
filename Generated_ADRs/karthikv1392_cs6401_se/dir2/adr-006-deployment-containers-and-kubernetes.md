---
### ADR-006: Deployment — Containers and Kubernetes

**Status:** Inferred
**Context:** Need for consistent packaging, portability, auto-scaling, and operational standardization across environments.
**Decision:** Package applications as OCI images and deploy to Kubernetes (managed where possible). Use Helm or equivalent for release manifests, and standardize health probes, resource requests/limits, and autoscaling policies.
**Consequences:** Strong ecosystem and operational consistency. Steeper learning curve and cluster ops overhead; managed offerings mitigate undifferentiated heavy lifting.