# Session 09, Growth Analyst

**Time:** 50 minutes, 4:50 to 5:40
**Pace:** run the brief and open the dashboard in 15 minutes, the alarm and the estimates in 10, schedule and test the routine in 20, leave 5 spare
**Primitive:** Routines, scheduled runs inside the desktop app
**Teammate hired:** 09, Growth Analyst (`/growth-analyst`)
**You walk out with:** your first weekly brief, a dashboard that opens on a double click, and a routine that produces it again every Monday without you asking

---

## Before you start

- [ ] `brand-brain/unit-economics.md` filled with your real numbers, however rough
- [ ] Your last 30 to 90 days of orders exported from your store as a CSV file and saved in `brand-brain/`. If you do not have it, use the sample file `examples/little-lab/sample-inputs/shopify-orders-28d.csv`
- [ ] Ad spend for the same period, as an export or a screenshot, if you run ads
- [ ] Customer Researcher and competitor reports in `my-work/`

---

## What this teaches

Two things, and the second is the one that changes your week.

**First, one alarm.** The brief surfaces the single number that needs your attention, not fifteen. If everything is flagged, nothing is. That constraint is what makes a weekly brief readable on a Monday morning rather than another dashboard you stop opening.

**Second, Routines.** Up to now, everything ran because you typed something. A routine runs on a schedule. The brief lands whether or not you remember to ask, and the difference between a system you use and one you abandon is almost entirely this.

---

## Steps

### 1. Run the brief

```
/growth-analyst
```

It reads `CLAUDE.md`, your unit economics, and the exports in `brand-brain/`. **Founder-written numbers are the source of truth. Exported data is enrichment on top.** Where the two disagree by more than 20 percent, it surfaces the gap rather than silently picking one, and that disagreement is usually the most interesting thing on the page.

It produces four files:

| File | What it is |
|---|---|
| `<date>-brief.md` | The structured read, and what other teammates cite |
| `<date>-index.md` | A short pointer so other skills can find this week |
| `data/numbers.json` | Machine readable, with a weekly archive copy |
| `dashboard.html` | The visual read |

### 2. Open the dashboard

Click `dashboard.html` in the chat. It opens in the browser pane inside the app.

**It works on a double click from Finder or Explorer too**, with no server and no terminal, because the data is written into the file rather than fetched. That matters: you can send it to a cofounder and it just opens.

### 3. Read the alarm, and only the alarm

The alarm card is the most emphasised block on the page for a reason. It carries the metric, the movement, what is driving it, and one action naming who runs it.

**Everything else on the page is context for that one number.** Read it after.

### 4. Check what it says is estimated

If the brief opens with a banner saying it is running on partly estimated data, read that banner carefully. It names what is missing and how to fix it.

**A confident brief on stale numbers is worse than an honest empty one**, because it reads exactly as convincing. The banner is the skill protecting you from itself.

### 5. Do the action

Every brief ends with exactly one action for the week, and it is written so you could check later whether it worked: "should lift add to cart on the hero product by 5 to 10 percent", not "improve conversion".

Do it now if it takes ten minutes. Put it in your calendar if it does not.

### 6. Schedule it

This is the part that outlasts the day.

In the **Code** tab, find **Routines** in the sidebar. Click **New routine**, then choose **Local**.

Fill in four things:

| Field | What to put |
|---|---|
| **Name** | Monday growth brief |
| **Folder** | Your `d2cinsider-ai-bootcamp` folder |
| **Schedule** | Weekly, Monday, 09:00 |
| **Instructions** | See below |

For the instructions, paste this:

```
Run the growth-analyst skill for this brand. Regenerate the brief, the numbers file and the dashboard for the last 7 days.

Then reply with three things only: the headline sentence, the one alarm in a single line, and the path to the dashboard. Nothing else. The full read lives in the file.
```

**That last paragraph is doing real work.** A recurring job that dumps four pages into your view gets ignored within a month, and then the whole system is invisible to you. Short ping, detail in the file.

### 7. Know the limits of a local routine

Be clear about what you just set up, because the failure mode is silent:

- It runs **on your machine**, which means the **app has to be open and the computer awake** at the scheduled time.
- If your machine sleeps through Monday 09:00, one catch-up run fires when you wake it. Older misses are dropped.
- If you close the laptop for a week, you get one brief on your return, not seven.

**If you need it to run whether or not your laptop is open**, that is a cloud routine rather than a local one, and it is a good thing to set up at home rather than during the live session.

### 8. Test it before you trust it

Do not schedule four routines and walk away. Set this one to run a couple of minutes from now, watch it fire, and confirm the ping is short and the dashboard regenerated.

**Then** change it back to Monday.

### 9. Save what you set up (at home)

```
Write my-work/growth-analyst/schedule-config.md describing what I just scheduled: the routine name, when it runs, what it produces, how to pause it for a holiday and how to change the time.
```

Six months from now, you will not remember. The file will.

---

## Check it worked

- [ ] `my-work/growth-analyst/` has a brief, an index, `data/numbers.json` and `dashboard.html`
- [ ] The dashboard opens on a double click, with no server
- [ ] You can state the one alarm in a sentence
- [ ] The action is done or in your calendar
- [ ] A routine exists, and **you watched it fire once**
- [ ] `schedule-config.md` records what you set up

---

## If it breaks

**Every number says "no data".**
It could not find your order export. Check the CSV file is inside `brand-brain/` and tell it the file name. If you have no export today, point it at the sample data and re-run on your own numbers at home.

**The brief and my own numbers disagree.**
Good. Read the gaps section. It will tell you which is stale rather than overriding either. Usually your written numbers are older than you think.

**It refused to compute CAC.**
No spend, or no order count. It will not invent a denominator. Connect the ad account or paste the spend.

**The routine did not fire.**
The app was closed, or the machine slept. That is expected for a local routine. Check the Routines sidebar for the last run status.

**The routine fired but sent me four pages.**
Your instructions did not cap the reply. Edit the routine and put the "three things only" paragraph back in.

---

## What good looks like

[`examples/gur-and-ghee/my-work/growth-analyst/`](examples/gur-and-ghee/my-work/growth-analyst/), including the dashboard. Open the dashboard file in a browser to see the shape you are aiming at.

**Read both briefs in that folder, the June one and the October one.** Same brand, four months apart. The June brief is built from exported files and says which numbers are estimates. The October brief is on live data and can see something June could not. That is the argument for scheduling this rather than running it once.

Read [`references/session-09-growth-analyst/monday-brief-spec.md`](references/session-09-growth-analyst/monday-brief-spec.md) for the full spec.

---

## Take-home

After four weeks you have four archived numbers files, and the brief can finally show you trends instead of snapshots. That is when this teammate becomes the most valuable one you have. Do not delete the archive.

**Next:** [Session 10, Chief of Staff](session-10-chief-of-staff.md)
