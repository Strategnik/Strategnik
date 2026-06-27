# Strategnik

**Nick Talbert** — B2B go-to-market strategist who builds the tooling instead of just talking about it.

20+ years in positioning, pipeline mechanics, and GTM systems. The repos here are the working end of that: small, sharp tools that solve a real GTM or build problem, plus the graph layer behind [Ontogent](https://ontogent.ai).

---

### 🧮 [funnel-calculator](https://github.com/Strategnik/funnel-calculator)
A B2B funnel **velocity** calculator. Most funnel math is static — this models how accounts actually *flow* through stages over time using a constraint solver, so you get true CPL, time-to-revenue, and total investment instead of a snapshot ratio.
`TypeScript`

### ⚙️ [overkill](https://github.com/Strategnik/overkill)
A model router for Claude Code. Runs a cheap model by default and **escalates to Opus only when the task earns it** — stop paying top-tier rates for trivial work. Deliberate version pinning, event-driven upgrade ritual.
`Shell` · OSS

### 🕸️ Ontogent — the GraphRAG layer *(product → [ontogent.ai](https://ontogent.ai))*
A GTM intelligence layer built on a **knowledge graph**, not a pile of documents. The graph half — the part worth describing publicly:

- **Artifact-first model.** Every ingested source becomes a typed artifact with embeddings and multiple retrieval axes, not an undifferentiated chunk. If retrieval can't find it, it isn't in the graph.
- **Multi-axis GraphRAG.** Retrieval combines vector similarity with graph traversal (entities, relationships, inferred edges) so context is assembled by *relevance and connection*, not just nearest-neighbor text.
- **Self-enriching graph.** Inference rules run as graph queries to derive new edges, surface tensions, and flag orphaned nodes that signal drift.

The result: an LLM gets the highest-relevance GTM context to reason over — and the graph stays the source of truth, not the prompt.

---

📍 California · 🌐 [strategnik.com](https://strategnik.com)
