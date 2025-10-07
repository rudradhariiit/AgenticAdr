---
### ADR-011: Multi-Tenancy and Data Isolation — Shared DB with Tenant Guards

**Status:** Inferred
**Context:** Support multiple tenants while balancing cost, performance, and isolation. Compliance may require logical isolation guarantees.
**Decision:** Use a shared database with tenant_id on all multi-tenant tables. Enforce row-level security (RLS) where available and strict tenancy scoping in all queries. For high-value or regulated tenants, support “premium isolation” via separate schemas or databases.
**Consequences:** Cost-efficient baseline with a path to stronger isolation. Requires rigorous tenancy checks, performance guardrails, and careful cross-tenant data handling.