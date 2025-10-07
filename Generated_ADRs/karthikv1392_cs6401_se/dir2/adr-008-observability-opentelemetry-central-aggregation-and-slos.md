---
### ADR-008: Observability — OpenTelemetry, Central Aggregation, and SLOs

**Status:** Inferred
**Context:** Troubleshooting distributed systems and ensuring reliability require end-to-end visibility.
**Decision:** Instrument services with OpenTelemetry for traces, metrics, and logs. Export to centralized backends (managed or OSS stack). Define service-level indicators (SLIs) and SLOs; build alerting on SLO error budgets and high-signal metrics.
**Consequences:** Faster diagnosis and measurable reliability. Added instrumentation work and costs for storage/retention; consistent correlation IDs become mandatory.