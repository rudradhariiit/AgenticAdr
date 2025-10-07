---
### ADR-014: Configuration and Feature Management — Centralized Config, Feature Flags

**Status:** Inferred
**Context:** Need to change behavior without redeploys and to roll out features safely.
**Decision:** Externalize configuration via environment-agnostic config service or files with strict schema validation. Use a feature flag platform for gradual rollouts, experiments, and kill switches. Maintain flag lifecycle with ownership and sunset dates.
**Consequences:** Faster, safer changes. Requires governance to avoid config/flag sprawl and to manage conditional complexity in code.