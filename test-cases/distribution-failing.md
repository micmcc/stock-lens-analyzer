# Distribution failing test

## User prompt
Run the distribution lens on this holding.

## Expected behavior

- select DISTRIBUTION
- score in the high urgency range
- state should be `deteriorating` or `failing`
- entry/action language should be `trim review`, `exit review`, or `failed reclaim / reduce`
- summary should name the recovery condition that would negate the bearish exit thesis

## What the model should notice

- break of higher-low structure or recent support shelf
- failed reclaim or weak bounce into resistance / EMA
- downside participation through red expansion candles or heavy sell volume
- momentum rolling over or repeatedly failing to recover
- price trading below acceptance / back under value

## Failure modes to avoid

- defaulting to `hold` because one indicator still looks neutral
- treating a failed reclaim as harmless
- omitting the condition that would invalidate the bearish exit view