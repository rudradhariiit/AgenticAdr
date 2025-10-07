---
### ADR-005: Asynchronous Communication — Events with Outbox Pattern

**Status:** Inferred
**Context:** Some workflows require decoupling, reliability, and eventual consistency across boundaries.
**Decision:** Use an event streaming platform (e.g., Kafka or managed equivalent) for domain and integration events. Employ the transactional outbox pattern to ensure atomic publication with state changes. Define stable event schemas and versioning.
**Consequences:** Improved decoupling and scalability for background processing. Increases complexity in topology, schema governance, and failure handling. Consumers must be idempotent.