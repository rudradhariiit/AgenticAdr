---
### ADR-002: API Style and Versioning — RESTful JSON with OpenAPI

**Status:** Inferred
**Context:** Broad client compatibility, simplicity, and tooling support are priorities. The system exposes public and internal APIs that must evolve without breaking clients.
**Decision:** Use RESTful HTTP APIs with JSON payloads and OpenAPI specs for documentation and codegen. Apply semantic, non-breaking evolution where possible and explicit versioning (URI or header) for breaking changes. Enforce idempotency for unsafe operations via idempotency keys.
**Consequences:** Wide compatibility and mature tooling. Some use cases (e.g., high-chattiness) may later justify GraphQL or gRPC for specific interfaces.