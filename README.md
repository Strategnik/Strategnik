# Strategnik

**Nick Talbert** — B2B go-to-market strategist who builds the infrastructure, not just the strategy deck.

20+ years in positioning, pipeline mechanics, and GTM systems. The repos here are the working end of that — small, sharp tools — plus the multi-axis GraphRAG engine behind [Ontogent](https://ontogent.ai).

---

### 🧮 [funnel-calculator](https://github.com/Strategnik/funnel-calculator)
A B2B funnel **velocity** calculator. Most funnel math is static — this models how accounts actually *flow* through stages over time using a constraint solver, so you get true CPL, time-to-revenue, and total investment instead of a snapshot ratio.
`TypeScript`

### ⚙️ [overkill](https://github.com/Strategnik/overkill)
A model router for Claude Code. Runs a cheap model by default and **escalates to Opus only when the task earns it** — stop paying top-tier rates for trivial work. Deliberate version pinning, event-driven upgrade ritual.
`Shell` · OSS

### 🕸️ Ontogent — multi-axis GraphRAG infrastructure *(product → [ontogent.ai](https://ontogent.ai))*
Two layers. The bottom one — the engineering — is the part I'm pointing at here.

**Infrastructure layer.** A real multi-axis GraphRAG engine, not vector-search-over-chunks with a graph diagram bolted on:
- **Artifact-first ingestion.** Every source becomes a typed artifact with embeddings and multiple retrieval axes. If multi-axis retrieval can't surface it, it isn't in the graph.
- **Multi-axis retrieval.** Vector similarity *and* graph traversal — entities, relationships, inferred edges — combine to assemble context by relevance *and* connection, not nearest-neighbor text alone.
- **Self-enriching graph.** Inference rules run as graph queries to derive new edges, detect contradiction/tension, and flag orphaned nodes as drift signals.

**Knowledge layer.** 20+ years of GTM judgment — positioning, ICP, pipeline mechanics — encoded as canonical playbooks the engine applies. That's the moat, and it stays behind [ontogent.ai](https://ontogent.ai).

The hard infrastructure is built and real. The soft layer on top is where the value compounds.

---

📍 California · 🌐 [strategnik.com](https://strategnik.com)
