---
name: stock-lens-analyzer
description: analyze live atlas tradingview stock charts using named technical analysis lenses for entry and exit decisions. use when the user is on a tradingview chart in atlas and asks for technical analysis, setup scoring, entry or exit planning, support and resistance, or to apply a breakout or distribution lens. infer the lens when possible, but also support explicit requests such as apply the breakout lens or run the distribution lens. return a structured scorecard, action zone, invalidation, targets, notes, and a short summary.
---

# Overview

Use this skill when the user is on a live TradingView chart in Atlas and wants a chart read for entry or exit decisions.

This skill currently supports two active lenses:

- BREAKOUT
- DISTRIBUTION

The skill should infer the lens when the request is clear:
- requests about entries, breakout quality, reclaim levels, or watchlist ranking usually map to BREAKOUT
- requests about deterioration, trim/exit review, failed structure, or holding management usually map to DISTRIBUTION

If intent is ambiguous, ask the user which lens to apply.

## Workflow

1. Confirm the chart context is a live Atlas TradingView page.
2. Identify the correct lens.
3. Read price structure, momentum, participation, trend alignment, and nearby supply/demand.
4. Score the chart using the selected lens rubric.
5. Return the exact output structure in `templates/output-template.md`.
6. If the chart is unclear, say what is missing and lower confidence.

## Scoring references

Read these files before answering:
- `references/tradingview-assumptions.md`
- `references/output-contract.md`
- `references/action-tiers.md`

Then load the active lens spec:
- BREAKOUT → `specs/breakout.md`
- DISTRIBUTION → `specs/distribution.md`

Do not load future lens specs unless asked to extend the skill.

## Output rules

- Always name the lens used.
- Always include a one-row score table for single-chart analysis.
- Always include setup state, entry/action zone, invalidation, targets, and a one-line note.
- End with a short summary that states whether the chart is actionable, watchlist-only, or avoid/review.
- Avoid overclaiming precision from a chart image.
- Distinguish clearly between early, triggered, extended, and failing setups.

## Future extension points

Scaffolding exists for:
- ACCUMULATION
- TRAILING_STOP
- DEEP_VALUE

Do not apply these until their specs are implemented and the user requests them.
