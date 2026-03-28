# Breakout good test

## User prompt
Apply the breakout lens to this chart.

## Expected behavior

- select BREAKOUT
- score in the upper range
- state should be `triggered` or `extended`, not `early`
- entry language should be `breakout trigger` or `retest entry`
- identify the active trigger condition
- include a clear score interpretation consistent with an actionable setup
- name a common breakout pattern
- summary should explain why the move is valid, not just that momentum is improving

## What the model should notice

- clear break of the lower-high sequence or consolidation ceiling
- acceptable hold above the breakout area
- visible participation through candle expansion and/or volume
- momentum turning up with room to continue, not just curling
- price accepted above nearby supply or reclaiming the key EMA
- context should note whether the move is triggered versus already extended

## Failure modes to avoid

- calling a confirmed breakout `early`
- using vague language like `looks decent`
- skipping the trigger condition and going straight to a generic bullish summary
- ignoring overhead supply if it materially limits reward/risk
