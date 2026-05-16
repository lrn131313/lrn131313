# Loren Stanoi

[linkedin.com/in/loren-stanoi-575598276](https://www.linkedin.com/in/loren-stanoi-575598276/)

I build production AI-agent systems by directing models and understanding
how they actually behave — where they drift, when they lie about being
done, and what makes a tool usable by an agent instead of just a human.
Eval-first, local-first, shipping over theory.

### What I build

**[lrn-team-platform](https://github.com/lrn131313/lrn-team-platform)** — a
local multi-agent IT team orchestrator. Drives Claude Code, OpenAI Codex
and Perplexity under a LangGraph state machine to build real codebases on
your machine. No central server, no SaaS dependency.

- 521 passing tests, Apache-2.0
- **ClawBench eval methodology** — 4-axis trace scoring
  (Completion / Trajectory / Behavior / Judge), failure-regime
  classification, variance decomposition to separate real capability
  from run-to-run noise
- **Hallucination gate** — agents can never silently report DONE;
  `claim.json` reflection + contract checks return work to the board
- **Skill auto-distillation** — repeated tool-use patterns (≥5 calls)
  are distilled into reusable role skills automatically
- Built-in pre-push secret scanner, OAuth Device Flow, signed updater
- LangGraph + FastAPI control plane + Next.js 16 dashboard + Tauri shell
- Per-role AGENTS.md + 4-level memory bundles + machine-checkable
  OpenAPI/design-spec contract gates — how context and contracts are
  exposed to orchestrated agents so they stay on-rails

### Shipped to production

**[app.primkron.ro](https://app.primkron.ro)** — Primkron CRM, a sales
CRM for auto dealerships. Built on **Supabase** (Auth, Row-Level Security,
Postgres RPC, Management API) with Next.js. Live and in real use.

**[echilibrultau.ro](https://echilibrultau.ro)** — a production web
platform I built and shipped end to end (Next.js + Supabase + Vercel +
Cloudflare). Live.

Source for these is private (production / client code) — happy to walk
through the architecture or open access on request.

### How I work

I don't come from a traditional CS track. I ship by decomposing a
problem precisely enough that an AI system can build it, instrumenting
what it does, and fixing the layer where the assumption broke. The
output is real: tested, shipped, used.
