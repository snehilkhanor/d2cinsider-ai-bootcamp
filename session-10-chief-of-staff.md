# Session 10, Chief of Staff

**Time:** 50 minutes, 5:40 to 6:30, followed by 30 minutes of share-outs
**Pace:** check the chain and run in 15 minutes, summary and the cross-cutting call in 10, roadmap in 10, command center in 10, pick Monday's ship in 5
**Primitive:** the Chief of Staff pattern, one subagent reading across every other teammate
**Teammate hired:** 10, Chief of Staff (the `captain` subagent)
**You walk out with:** a 90 day operating roadmap, a one-page command center, a standing schedule, and one recommendation no single teammate could have made

---

## Before you start

- [ ] Every session from 01 to 09 has produced at least one file in `my-work/`
- [ ] `CLAUDE.md` exists and passed its voice test this morning

If three or more teammates never ran, the Chief of Staff will say so and its synthesis will be thin. That is honest behaviour, not a bug. If you fell behind today, run it anyway now, then re-run it at home once the missing teammates have run.

---

## What this teaches

You have ten teammates and a folder with dozens of files in it. Nobody has read all of it, and nobody could: reading every ad, SOP and page would fill any context before a single conclusion got drawn.

The Chief of Staff solves that with one rule.

**Indexes only, never raw outputs.** Every teammate writes a short index precisely so the Chief of Staff never has to open their work. Ten indexes is a manageable read. Two hundred pieces is not.

That rule is what makes an orchestrator possible at all, and it is why every session today insisted on writing an index you probably skimmed.

---

## Steps

### 1. Check the chain is alive

Before synthesis, take stock:

```
For each folder in my-work/, tell me the most recent file and how many days old it is. Flag anything older than 14 days.
```

A stale chain is the most common reason a Chief of Staff run is worthless, and it is invisible unless you name it. Everything you made today is fresh, so today this check is a formality. It matters the next time you run it.

### 2. Run the Chief of Staff

```
Use the captain agent to produce my 90 day roadmap.
```

It reads `CLAUDE.md`, the two reports, and one index per teammate. Watch the Tasks pane: you should see it opening indexes, not pieces. If it starts reading individual ads, stop it and remind it of the rule.

It produces two files:

- `my-work/captain/<date>-90-day-roadmap.md`, the thing you consult
- `my-work/captain/<date>-summary.md`, the thing you actually read

### 3. Read the summary first

Two lines on the state of the chain, the cross-cutting recommendation, a pointer to the roadmap, and one to three things needing your attention right now, ranked.

### 4. Judge the cross-cutting recommendation

**This is the entire reason the Chief of Staff exists**, so hold it to the standard.

A good one looks like: your customer research shows a theme rising, your competitor work shows nobody serving it, so paid should ship that angle, content should bias toward it, and the product page gets rewritten this week. **Three or more teammates moving together on a signal none of them could see alone.**

**If one teammate could have said it by reading only their own output, it is not a Chief of Staff recommendation.** Push back and ask for one that cites at least three.

### 5. Work the roadmap

Week 1 gets three to five items. Each names the action, which teammate runs it, the measurable outcome, and **what it costs you if it does not happen**. That last column is what makes a roadmap something you act on rather than something you file.

Months 2 and 3 get three priorities each and no more. If your month 2 has nine items, it has none.

### 6. Settle the standing schedule

The roadmap recommends a schedule rather than setting it up. Read it and decide what you actually want. **Decide now, set them up at home.** The only routine you need running tonight is the Monday brief from Session 09.

A realistic starting set for a founder with a day job:

| When | Who | What |
|---|---|---|
| Monday 09:00 | Growth Analyst | The weekly brief, already set up in Session 09 |
| Monday 09:30 | Competitive Analyst | What moved in the category last week |
| Monthly | Content Director | Next 30 day calendar |

**Three is plenty.** Six recurring jobs that all ping you is how people end up muting the whole system.

Set each one up in the **Routines** sidebar the same way you did in Session 09, with the same discipline: short ping, detail in the file, test one before scheduling the rest.

Once you have connected Gmail, see [`after-the-bootcamp/connectors.md`](after-the-bootcamp/connectors.md), the Chief of Staff can wire them for you instead of listing them:

```
Use the captain agent with WIRE_SCHEDULE=yes and DELIVERY=email to set up the recurring runs.
```

It needs both flags. Passing the first without a delivery target gets you a checklist rather than a schedule, deliberately, because a recurring job with nowhere to deliver runs silently for weeks and nobody notices.

### 7. Read what it could not synthesise

The last section of the roadmap names the teammates whose output is stale and the questions it could not answer because the data is not there.

**That list is your next month's homework**, and it is usually more actionable than the roadmap itself.

### 8. Build your command center

One page that you open on Monday morning instead of ten folders.

```
Create my-work/command-center.md. One page. At the top: this week's one alarm from the Growth Analyst, and my Monday ship. Then a table with one row per teammate: what they last produced, the date, and a link to their latest index file. Then my three priorities for this month from the roadmap, and the standing schedule. Use only what is in the index files, do not open raw outputs.
```

Click the file path to open it. Every link in it opens a teammate's latest work. When you re-run a teammate, ask the Chief of Staff to refresh this page.

### 9. Pick Monday's ship

One thing. Name it, name the day, and name what has to be true for it to go out. Type it into the Zoom chat. This is what you say in the share-out at 6:30.

A founder who ships one thing on Monday ships the next twenty. A founder who ships nothing has a folder.

---

## Check it worked

- [ ] `my-work/captain/<date>-90-day-roadmap.md` exists
- [ ] `my-work/captain/<date>-summary.md` exists and you read it first
- [ ] The cross-cutting recommendation cites at least three teammates
- [ ] Week 1 has three to five items, each with an owner and a cost of inaction
- [ ] Your standing schedule is set up, tested, and no more than three jobs
- [ ] You know which data gap to close first

---

## If it breaks

**The recommendation is something one teammate already told me.**
Reject it. "Give me one that requires reading at least three teammates, and name them."

**It says my chain is stale.**
Believe it. Re-run the two or three teammates it named, then run the Chief of Staff again. A roadmap built on month-old inputs reads exactly as confident as a good one, which is what makes it dangerous.

**It ran out of room partway through.**
It read raw outputs instead of indexes. Restart it and say explicitly: "read only the index file from each teammate folder, never the pieces, ads, SOPs or pages."

**It wired nothing after I asked it to.**
`WIRE_SCHEDULE=yes` needs `DELIVERY=` alongside it. Check both were in your message.
- [ ] `my-work/command-center.md` exists and its links open

---

## What good looks like

[`examples/gur-and-ghee/my-work/captain/`](examples/gur-and-ghee/my-work/captain/) and [`examples/little-lab/my-work/captain/`](examples/little-lab/my-work/captain/) each hold a summary and a 90 day roadmap. Gur & Ghee also has a finished [`command-center.md`](examples/gur-and-ghee/my-work/command-center.md).

Read [`references/session-10-chief-of-staff/standing-schedule.md`](references/session-10-chief-of-staff/standing-schedule.md) before you wire anything.

---

## You are done

Ten teammates, all operating on your brand. A weekly brief that arrives without being asked. A 90 day plan with owners.

**What to do in the next seven days:**

1. Do the Week 1 items on the roadmap.
2. Close the one data gap the Chief of Staff named.
3. Read the Monday brief when it lands, and do its one action.

**Then come back.** Re-run any teammate by opening its session file. They compound. Your brand profile gets richer, the Competitive Analyst builds history, the Growth Analyst finally gets trends once it has four weeks of archive.

**In the weeks after:** everything in [`after-the-bootcamp/`](after-the-bootcamp/): write your own skill, connect Shopify, Drive and Gmail, and hire the Influencer Scout.

**When you are ready for more tools:** [`resources.md`](resources.md), and read it before installing anything.
