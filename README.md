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

**GitNexus** — a code knowledge graph exposed to AI agents over **MCP**
(plus CLI + 7 task-routed skills). Agents read process-grouped execution
flows, symbol blast-radius, and git-diff impact through token-cheap
resources instead of grepping blind. A working answer to "how do you
design docs and tooling so agents use them effectively."

### How I work

I don't come from a traditional CS track. I ship by decomposing a
problem precisely enough that an AI system can build it, instrumenting
what it does, and fixing the layer where the assumption broke. The
output is real: tested, shipped, used.

Built under PRIMKRON SRL (Brașov, Romania).
