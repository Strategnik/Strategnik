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

---

## Ontogent — the context layer for GTM AI

A knowledge-graph intelligence layer that gives an LLM *domain-correct* GTM context. Two pieces are open and inspectable; the moat stays behind the product.

### 🕸️ [graphrag-demo](https://github.com/Strategnik/graphrag-demo) — multi-axis GraphRAG, from scratch
Dependency-free and runnable in one command. Combines **vector similarity + axis filtering + graph traversal**, fuses the signals with **Reciprocal Rank Fusion**, diversifies with **MMR**, and runs **graph-query inference** to derive new edges and flag drift — every result carries provenance (e.g. `graph_traversal:SUPPORTS@depth2`). Clone it and watch a weakly-matched artifact correctly rank #1 because three signals agree.
`TypeScript` · OSS · `bun run demo -- "your question"`

### 🧩 [ontogent-core](https://github.com/Strategnik/ontogent-core) — the open context engine
Domain-agnostic infrastructure (MIT): pack format → loader → validator → constrained-CEL evaluator → **Shield→Rank resolver** → MCP delivery. Zero domain knowledge compiled in — delete the packs and it still runs, it just has nothing to apply. *The plumbing is open; the brain is the content.*
`TypeScript` · OSS · runs out of the box

### 🔒 The product *([ontogent.ai](https://ontogent.ai))*
The hosted layer swaps in a learned embedding model, a cross-encoder reranker, and the **canonical GTM playbooks** — 20+ years of positioning and pipeline judgment encoded as authority-weighted content. That's the moat, and it stays private.

---

📍 California · 🌐 [strategnik.com](https://strategnik.com)
