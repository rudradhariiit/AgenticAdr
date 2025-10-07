---
### ADR-012: Resilience Patterns — Timeouts, Retries, Idempotency, Circuit Breakers

**Status:** Inferred
**Context:** Distributed failures are inevitable; we must fail fast and recover gracefully.
**Decision:** Standardize client timeouts, bounded retries with exponential backoff and jitter, idempotency for non-read operations, and circuit breakers/bulkheads for critical dependencies. Define retry budgets and classify errors as retryable vs non-retryable.
**Consequences:** Improved reliability and user experience under failure. Added complexity in policies and tuning; improper retries can amplify incidents.