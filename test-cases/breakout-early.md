# Breakout early test

## User prompt
Apply the breakout lens to this chart.

## Expected behavior

- select BREAKOUT
- score in the middle or lower-middle range
- state should be `early`
- entry language should be `watch / wait` or `no entry`
- identify that trigger conditions are not fully met yet
- include a score interpretation consistent with a developing setup
- name the most likely breakout pattern, even if not confirmed
- summary should explain what confirmation is still missing

## What the model should notice

- improving bounce or reclaim attempt, but no clean break yet
- momentum may be turning, but confirmation is incomplete
- participation is present only partially or not decisively
- price may still be under the EMA or under nearby supply
- breakout thesis is developing, not triggered
- context should note first-attempt versus still-under-supply risk if visible

## Failure modes to avoid

- calling it actionable too early
- overstating volume confirmation
- inventing a trigger that is not actually present
- ignoring that structure is still unresolved
