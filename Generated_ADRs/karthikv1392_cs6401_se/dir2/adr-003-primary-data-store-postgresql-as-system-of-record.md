---
### ADR-003: Primary Data Store — PostgreSQL as System of Record

**Status:** Inferred
**Context:** Strong consistency, relational modeling, and transactional integrity are required for core business data.
**Decision:** Use PostgreSQL as the primary relational database. Standardize on UUID primary keys, strict foreign keys, and optimistic locking where appropriate. Manage schema changes via a migration tool and apply zero-downtime migration practices.
**Consequences:** Reliable consistency and rich SQL capabilities. Vertical scaling is simple initially; read replicas and partitioning can extend capacity. Highly write-intensive workloads may later require service-specific datastores.