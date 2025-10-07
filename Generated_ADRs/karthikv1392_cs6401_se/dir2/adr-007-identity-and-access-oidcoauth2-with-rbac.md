---
### ADR-007: Identity and Access — OIDC/OAuth2 with RBAC

**Status:** Inferred
**Context:** Secure authentication and authorization across web and API clients with potential for third-party integration.
**Decision:** Use an OpenID Connect provider for authentication and OAuth2 for delegated access. Use JWT access tokens with short lifetimes and refresh tokens where needed. Implement application-level RBAC and, where applicable, ABAC for fine-grained rules. Store secrets in a managed secrets vault.
**Consequences:** Standards-based integration and interoperability. Requires careful token lifecycle management, key rotation, and least-privilege policy hygiene.