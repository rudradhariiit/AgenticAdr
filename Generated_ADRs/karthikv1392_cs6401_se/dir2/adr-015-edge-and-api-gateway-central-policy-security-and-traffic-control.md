---
### ADR-015: Edge and API Gateway — Central Policy, Security, and Traffic Control

**Status:** Inferred
**Context:** Uniform ingress, security controls, and observability at the edge are needed across services.
**Decision:** Deploy an API gateway or ingress controller to terminate TLS, enforce WAF, rate limits, authn/z delegation, request/response normalization, and request size limits. Centralize API analytics at the gateway.
**Consequences:** Consistent edge security and traffic management. Gateway becomes a critical dependency; configuration drift can cause outages without careful change control.