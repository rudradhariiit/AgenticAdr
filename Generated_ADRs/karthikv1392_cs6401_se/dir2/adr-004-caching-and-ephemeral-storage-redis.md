---
### ADR-004: Caching and Ephemeral Storage — Redis

**Status:** Inferred
**Context:** Reducing latency and database load is needed for hot reads, sessions, and transient coordination.
**Decision:** Introduce Redis for read-through and write-through caches, request-level caching, distributed locks, and ephemeral data (e.g., rate limits). Define cache keys, TTLs, invalidation rules, and cache observability upfront.
**Consequences:** Lower latency and DB offload. Adds operational complexity and coherence considerations; stale data risks must be managed via TTLs and invalidation strategies.