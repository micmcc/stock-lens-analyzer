# Distribution failing test

## User prompt
Run the distribution lens on this holding.

## Expected behavior

- select DISTRIBUTION
- score in the high urgency range
- state should be `deteriorating` or `failing`
- entry/action language should be `trim review`, `exit review`, or `failed reclaim / reduce`
- identify the active trigger condition
- include a score interpretation consistent with high exit urgency
- name a common distribution pattern
- summary should name the recovery condition that would negate the bearish exit thesis

## What the model should notice

- break of higher-low structure or recent support shelf
- failed reclaim or weak bounce into resistance / EMA
- downside participation through red expansion candles or heavy sell volume
- momentum rolling over with limited recovery
- price trading below acceptance / back under value
- context should note whether the breakdown is first failure or later-stage damage if visible

## Failure modes to avoid

- defaulting to `hold` because one indicator still looks neutral
- treating a failed reclaim as harmless
- skipping the trigger condition and pattern callout
- omitting the condition that would invalidate the bearish exit view
