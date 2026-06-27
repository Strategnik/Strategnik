# Strategnik

**Nick Talbert** — B2B go-to-market strategist who builds the infrastructure, not just the strategy deck.

20+ years in positioning, pipeline mechanics, and GTM systems. The repos here are the working end of that — small, sharp tools and the context infrastructure behind [Ontogent](https://ontogent.ai).

---

### 🧮 [funnel-calculator](https://github.com/Strategnik/funnel-calculator)
A B2B funnel **velocity** calculator. Most funnel math is static — this models how accounts actually *flow* through stages over time using a constraint solver, so you get true CPL, time-to-revenue, and total investment instead of a snapshot ratio.
`TypeScript`

### ⚙️ [overkill](https://github.com/Strategnik/overkill)
A model router for Claude Code. Runs a cheap model by default and **escalates to Opus only when the task earns it** — stop paying top-tier rates for trivial work. Deliberate version pinning, event-driven upgrade ritual.
`Shell` · OSS

### 🧩 [ontogent-core](https://github.com/Strategnik/ontogent-core)
The **open context engine** behind Ontogent (MIT). Domain-agnostic infrastructure: pack format → loader → validator → constrained-CEL condition evaluator → **Shield→Rank resolver** → MCP delivery. Zero domain knowledge compiled in — delete the packs and it still runs, it just has nothing to apply. *The plumbing is open; the brain is the content.*
`TypeScript` · OSS · runs out of the box

### 🕸️ Ontogent — the GraphRAG retrieval layer *(product → [ontogent.ai](https://ontogent.ai))*
On top of the open engine sits the retrieval layer that makes context *correct*, not just present:
- **Artifact-first ingestion.** Every source becomes a typed artifact with embeddings and multiple retrieval axes. If multi-axis retrieval can't surface it, it isn't in the graph.
- **Multi-axis GraphRAG.** Vector similarity *and* graph traversal — entities, relationships, inferred edges — combine to assemble context by relevance *and* connection, not nearest-neighbor text alone.
- **Self-enriching graph.** Inference rules run as graph queries (Cypher over the node graph) to derive new edges, detect contradiction/tension, and flag orphaned nodes as drift signals.

This layer, plus the canonical GTM playbooks — 20+ years of positioning and pipeline judgment — is the moat, and it stays behind [ontogent.ai](https://ontogent.ai).

---

📍 California · 🌐 [strategnik.com](https://strategnik.com)
