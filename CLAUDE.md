# bakeoff (public holding repo) CLAUDE.md

This is the PUBLIC holding repo for the bake-off structure: methodology, comparison patterns, capture-stack templates. Trading code stays in a private companion repo and is never published.

## Project overview

A 10-harness comparison bake-off for autonomous stock trading code. Each harness builds the same shared issue (a fully-autonomous CTRL feature spec) one-shot, scored against the same production-quality bar.

## Future-publication intent

After the bake-off and the blog series complete on hoiboy.uk, the following gets extracted into this repo:

- `METHODOLOGY.md` (11-column rubric, composite weighted formula, Pareto-frontier sanity check, tiebreaker order, no-winner disposition)
- `PRODUCTION_QUALITY_BAR.md` (8-section scorecard with criteria counts)
- `TEST_ORDER.md` (running order rationale, anchoring-bias mitigation)
- `capture-stack-templates/` (mitmproxy + inotifywait scaffolding, sanitised)
- `comparison-patterns/` (how to score and compare without contaminating the measurement)
- One-line summaries of each harness's outcome (no source code, no postmortems)

## What does NOT get published

- Trading code (any direction: buy/sell logic, position sizing, kill-switches with thresholds)
- IBKR / broker integration details (account IDs, connection patterns specific to Hoi's setup)
- Per-harness build outputs (potential vulnerability surface)
- Cost logs, capture logs, postmortems
- Anything that would identify individual harness internals beyond what their public docs already disclose

## Reference to dotfiles patterns

The bake-off uses Hoi's SST3 (Single Source of Truth v3) workflow patterns. See the public mirror at [hoiung/SST3-AI-Harness](https://github.com/hoiung/SST3-AI-Harness) for the harness itself. This repo will publish the comparison patterns separately.

## Privacy preservation

Per Hoi's `feedback_private_business_details.md`: the existence and name of any private companion repo is intentionally not advertised here. Searches for "bakeoff" on hoiung's GitHub profile will find only this public repo.

## Contributing

This repo will not accept contributions until after the bake-off + blog completes (the holding period). Once the structure is published, issues + discussions will be welcomed.

## License

MIT. Each tool / harness referenced retains its own license.
