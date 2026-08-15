# Riley Trottier

**Senior Product Manager @ Workday** — building AI agents for enterprise financial operations.
Victoria, BC · [LinkedIn](https://www.linkedin.com/in/rileytrottier/)

Before Workday I spent the better part of a decade shipping transaction-heavy platforms: transit payments at 10M+ user scale (Umo / Cubic Transportation Systems), a health-tech platform serving 15,000 veterans across Canada (WCG), and SaaS payments products for Canadian merchants (Zomaron → Paystone).

I build the tooling I wish existed for shipping AI features — mostly around the question teams struggle most to answer: **"did this agent get better or worse?"**

---

## What I'm building

### [agent-eval-harness](https://github.com/rileytrottier23/agent-eval-harness)

The unit-tests-and-CI-report layer for AI agents. Runs a defined suite of cases against any agent behind a thin adapter and returns a scorecard: task success rate, cost, latency, and guardrail-violation rate — with per-case drill-down and run-over-run regression detection. Every run is stored immutably, so quality stops being a vibe and becomes a number you can diff.

Targets a local function, the Anthropic API, or a live MCP server. Deterministic and LLM-judge grading. Ships a CI workflow and a Streamlit dashboard.

`Python`

### [product-evaluator](https://github.com/rileytrottier23/product-evaluator)

Turns a PRD into a reviewable suite of structured eval cases. Three stages: extract requirements → review and edit → generate cases and export as YAML or JSON.

`TypeScript`

**These two are one pipeline.** They share an eval-case schema, so a written requirement becomes an executable test becomes a scorecard:

```
PRD  ->  product-evaluator  ->  eval cases  ->  agent-eval-harness  ->  scorecard
```

That loop — spec to test to number — is the thing I think most teams shipping AI features are missing.

### [Riley-Claude-Skills](https://github.com/rileytrottier23/Riley-Claude-Skills)

The Claude skills I actually use day to day for PM work: PRD and spec writing, stakeholder decks, competitive research.

---

## How I think about AI product work

**Quality has to become a number before it can be managed.** Most teams know their agent "feels worse this week." Far fewer can say by how much, on which cases, or since which change. Everything here is aimed at closing that gap.

**Eval design is a product skill, not an engineering one.** Choosing the scenarios, writing the rubric, and setting the ship threshold are product judgment calls that sit squarely with the PM. The pipeline that runs them is a solved problem now.

**Guardrail failures shouldn't be averaged away.** An agent that issues a refund outside policy has failed differently than one that gave a slightly unhelpful answer. Scoring them in the same bucket hides the failure that actually matters.

---

riley.a.trottier@gmail.com

