# bakeoff

> Holding repo. Methodology + comparison patterns + capture-stack templates published here AFTER the bake-off completes. Trading code stays private. Only the structure is open.

## What this will be

A 10-harness comparison **bake-off** for autonomous stock trading code. Each harness builds the same shared issue (a fully-autonomous CTRL feature) one-shot, scored against the same production-quality bar.

The 10 harnesses under test:

- SST3-AI-Harness (home-grown, methodology-led — the bar)
- Smolagents (lean floor)
- pydantic-ai (lean type-safe)
- OpenAI Agents SDK (lean handoffs)
- CrewAI (heavy roles)
- LangGraph (heavy graph)
- Google ADK (heavy OTel)
- MAF (Microsoft Agent Framework — replaces AutoGen)
- Agno (late entrant)
- Claude Agent SDK (Anthropic-native reference baseline)

## What gets published here

After the bake-off + the blog series complete, this repo gets the **structure** of the experiment:

- `METHODOLOGY.md` — 11-column rubric, composite formula, Pareto-frontier sanity check, tiebreakers, no-winner disposition
- `PRODUCTION_QUALITY_BAR.md` — 8-section scorecard (code quality / observability / verification / monitor / trading safety / deployability / documentation / anti-fabrication)
- `TEST_ORDER.md` — running order rationale, anchoring-bias mitigation
- `capture-stack-templates/` — mitmproxy + inotifywait scaffolding for measuring agent harnesses
- `comparison-patterns/` — how to score and compare without contaminating the measurement

## What stays private

- The autonomous CTRL feature spec (production trading code)
- Each harness's build output (potential vulnerability surface)
- IBKR / broker integration details
- All cost logs, capture logs, postmortems

## Blog series

Documented at [hoiboy.uk](https://hoiboy.uk). Series goes live as one arc after all 10 runs complete (no per-run instalments).

## ETA

A few weeks. The bake-off itself is the long pole; the structure-extraction is mechanical once it's done.

## License

MIT (this holding repo). Each tool / harness retains its own license.
