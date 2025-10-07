### ADR-001: Architectural Style — Modular Monolith First, Evolution to Services

**Status:** Inferred
**Context:** The product needs to ship quickly with a small-to-medium team while keeping a path to scale and team autonomy as complexity grows.
**Decision:** Start with a well-structured modular monolith with explicit bounded contexts and internal module boundaries. Establish clear domain seams and anti-corruption layers to enable later extraction to services where justified.
**Consequences:** Faster initial delivery and simpler operations. Requires discipline to enforce boundaries. Later service extraction is straightforward but not free; plan for gradual decomposition.