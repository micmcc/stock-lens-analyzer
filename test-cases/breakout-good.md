# Breakout good test

## User prompt
Apply the breakout lens to this chart.

## Expected behavior

- select BREAKOUT
- score in the upper range
- state should be `triggered` or `extended`, not `early`
- entry language should be `breakout trigger` or `retest entry`
- summary should explain why the move is valid, not just that momentum is improving

## What the model should notice

- clear break of the lower-high sequence or consolidation ceiling
- acceptable hold above the breakout area
- visible participation through candle expansion and/or volume
- momentum confirming rather than merely curling
- price accepted above nearby supply or reclaiming the key EMA

## Failure modes to avoid

- calling a confirmed breakout `early`
- using vague language like `looks decent`
- ignoring overhead supply if it materially limits reward/risk