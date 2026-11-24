# The Standing Schedule

Four recurring runs that turn the team into a weekly rhythm. You set them up in the desktop app, the same way you set up the Monday brief in Session 09: **Routines**, then **New routine**, then **Local**.

Set up the first one, test it, and live with it for two weeks before adding the next. Four routines you ignore are worse than one you read.

All times are IST. Point every routine at your `d2cinsider-ai-bootcamp` folder.

## 1. Monday 09:00, the weekly brief

You already have this one from Session 09.

```
Run the growth-analyst skill for this brand. Regenerate the brief, the numbers file and the dashboard for the last 7 days.

Then reply with three things only: the headline sentence, the one alarm in a single line, and the path to the dashboard. Nothing else.
```

## 2. Monday 09:30, the competitor check

```
Run the market-analyst skill in Default scope on the competitors in CLAUDE.md. Compare with the most recent report in my-work/market-analyst/.

Reply with only what changed since last time: prices, offers, new products, new claims. If nothing changed, say "No change" and stop.
```

## 3. Wednesday 10:00, the customer check

Weekly is enough for most brands. Make it daily only if you get more than twenty new messages a day.

```
Run the voice-of-customer skill on anything new in brand-brain/reviews.md since the last report in my-work/voice-of-customer/.

Reply with any new theme, and any existing theme whose count has doubled. If neither, say "Nothing new" and stop.
```

This one only works if new reviews reach `brand-brain/reviews.md`. Paste them in on Tuesday, or connect your store, see [`after-the-bootcamp/connectors.md`](../../after-the-bootcamp/connectors.md).

## 4. First Monday of the month, 10:00, the Chief of Staff

```
Spawn the captain subagent. Read every teammate's latest index. Tell me the one cross-cutting recommendation for this month, flag any teammate whose latest output is more than 30 days old, and refresh my-work/command-center.md.
```

## Test before you trust

After creating a routine, open it and click **Run now**. Check three things:

1. It ran against your brand, not an example.
2. The reply is short.
3. The file it mentions exists.

## Things to know

- **A local routine runs only while the app is open and the laptop is awake.** If the laptop is shut on Monday at 09:00, nothing happens and nothing tells you.
- **Pausing.** Going on holiday: open the routine and turn it off. Turn it back on when you return.
- **Delivery to email** needs Gmail connected. Until then, the reply waits for you in the app.
- Review the list once a month. Delete any routine whose replies you have stopped reading.
