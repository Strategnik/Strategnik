# Strategnik

**Nick Talbert** — B2B go-to-market strategist who builds the infrastructure, not just the strategy deck.

20+ years in positioning, pipeline mechanics, and GTM systems. The public repos here are small, inspectable proof points: runnable context infrastructure, model-routing config, and GTM calculators that expose the system underneath the strategy.

## Start Here

| Repo | Why developers may care | Run first |
| --- | --- | --- |
| [graphrag-demo](https://github.com/Strategnik/graphrag-demo) | Dependency-free multi-axis GraphRAG with vector + axis + graph retrieval, RRF, MMR, inference, and provenance. | `bun run demo -- "how do we shorten enterprise sales cycles?"` |
| [ontogent-core](https://github.com/Strategnik/ontogent-core) | Open context engine: pack format, validator, constrained condition evaluator, Shield -> Rank resolver, CLI, and MCP delivery. | `bun run validate packs/reference` |
| [overkill](https://github.com/Strategnik/overkill) | Claude Code model router using native config and model-pinned subagents instead of a proxy. | `bash -n install.sh` |
| [funnel-calculator](https://github.com/Strategnik/funnel-calculator) | B2B funnel velocity calculator that models account flow over time instead of static conversion ratios. | `npm run build` |

## Current Focus

### [graphrag-demo](https://github.com/Strategnik/graphrag-demo)

[![CI](https://github.com/Strategnik/graphrag-demo/actions/workflows/ci.yml/badge.svg)](https://github.com/Strategnik/graphrag-demo/actions/workflows/ci.yml)

A from-scratch GraphRAG retrieval demo that runs with zero API keys, zero external services, and zero runtime dependencies. The interesting part is not "vector search"; it is the fusion of independent evidence:

- vector similarity for lexical/semantic seed hits
- axis matching for business dimensions
- graph traversal for structurally adjacent context
- Reciprocal Rank Fusion to combine non-comparable signals
- MMR to keep the final context diverse
- provenance on every returned artifact

Read: [architecture](https://github.com/Strategnik/graphrag-demo/blob/main/docs/architecture.md) and [sample trace](https://github.com/Strategnik/graphrag-demo/blob/main/examples/retrieval-trace.txt).

### [ontogent-core](https://github.com/Strategnik/ontogent-core)

[![CI](https://github.com/Strategnik/ontogent-core/actions/workflows/ci.yml/badge.svg)](https://github.com/Strategnik/ontogent-core/actions/workflows/ci.yml)

The open engine behind Ontogent's context layer. It contains the plumbing, not the proprietary domain knowledge: pack loading, validation, constrained condition evaluation, Shield -> Rank resolution, and MCP delivery.

The design line is deliberate: **the plumbing is open; the brain is the content.**

Read: [architecture](https://github.com/Strategnik/ontogent-core/blob/main/docs/architecture.md), [build your first pack](https://github.com/Strategnik/ontogent-core/blob/main/docs/build-your-first-pack.md), and [sample resolver output](https://github.com/Strategnik/ontogent-core/blob/main/examples/resolve-output.txt).

### [overkill](https://github.com/Strategnik/overkill)

[![CI](https://github.com/Strategnik/overkill/actions/workflows/ci.yml/badge.svg)](https://github.com/Strategnik/overkill/actions/workflows/ci.yml)

A model router for Claude Code that stays inside native config. It runs a cheap capable model by default and escalates to Opus only when the task earns it. No proxy, no service, no classifier round trip.

The useful idea is reactive escalation: start in the normal model, then delegate when the work proves hard.

Read: [architecture](https://github.com/Strategnik/overkill/blob/main/docs/architecture.md) and [installer behavior](https://github.com/Strategnik/overkill/blob/main/examples/install-output.txt).

### [funnel-calculator](https://github.com/Strategnik/funnel-calculator)

[![CI](https://github.com/Strategnik/funnel-calculator/actions/workflows/ci.yml/badge.svg)](https://github.com/Strategnik/funnel-calculator/actions/workflows/ci.yml)

A B2B funnel velocity calculator. Most funnel math is static; this models how account cohorts move through stages over quarters so you can see true CPL, time-to-revenue, and investment lag.

Read: [model notes](https://github.com/Strategnik/funnel-calculator/blob/main/docs/model.md) and [example scenario](https://github.com/Strategnik/funnel-calculator/blob/main/examples/funnel-scenario.md).

## Ontogent

[Ontogent](https://ontogent.ai) is a knowledge-graph intelligence layer for giving LLMs domain-correct GTM context. The open repos show the engine and retrieval mechanics. The hosted layer swaps in learned embeddings, a cross-encoder reranker, persistence, auth, and the canonical GTM packs.

📍 California · 🌐 [strategnik.com](https://strategnik.com)
