# Sessions 02 and 03, Competitive Analyst and Customer Researcher

**Time:** 60 minutes, 11:05 to 12:05
**Pace:** look at a skill in 5 minutes, Competitive Analyst in 25, Customer Researcher in 25, one finding back into `CLAUDE.md` in 5
**Primitive:** Skills, reusable playbooks Claude loads on its own
**Teammates hired:** 02 Competitive Analyst (`/market-analyst`), 03 Customer Researcher (`/voice-of-customer`)
**You walk out with:** a competitor intelligence report and a customer voice report in `my-work/`

---

## Before you start

- [ ] `CLAUDE.md` exists and passed its voice test in Session 01
- [ ] `brand-brain/reviews.md` has real reviews in it, or you have some ready to paste
- [ ] `brand-brain/competitors.md` names at least three competitors

---

## What this teaches

A skill is a folder with a `SKILL.md` file in it. The file has a description at the top and instructions below.

Claude reads every description when your project loads. When something you ask matches one, it loads that skill's instructions and follows them. You can also call one directly by typing its name after a slash.

**Why this matters more than it sounds.** Without skills, you get a good answer that you then have to re-explain next week. With skills, the method is written down. The same question next month runs the same playbook, reads the same files, applies the same safety checks, and saves to the same place.

You are not prompting. You are writing job descriptions.

---

## Steps

### 1. Look at a skill before you run one

In the prompt, type:

```
Show me .claude/skills/market-analyst/SKILL.md
```

Click the file path to open it in the file pane. Read the top four lines.

Notice the structure: a `name`, a `description` that lists the phrases that should trigger it, then numbered steps, then a section at the bottom called "How you work" that sets the standard. That shape is the whole trick. **The description decides when it runs. The steps decide what it does. The standard decides whether the output is any good.**

### 2. Run the Competitive Analyst

```
/market-analyst
```

It will read `CLAUDE.md`, then say back which competitors it is about to research, over what window, and where it will save. **It waits for you to confirm.** Change the list or the window here if you want.

Say go, and it researches each competitor across pricing, positioning, content, organic presence and paid activity, then writes to `my-work/market-analyst/<date>-intel-report.md`.

**While it runs, watch what it says it cannot see.** It will tell you if a competitor's site is unreachable or if it could not find ad activity. That honesty is the point. A competitor report that never says "I could not check this" is guessing.

### 3. Read the report properly

Open the file. Go straight to two sections:

- **Where they beat us.** This is the one that stings and the one that is useful.
- **What only you can answer.** Two or three questions that would sharpen the next run. Answer them into `brand-brain/competitors.md` and the next run is better.

### 4. Run the Customer Researcher

```
/voice-of-customer
```

It asks where your customer text is. **Point it at your reviews file** by typing `@brand-brain/reviews.md`, or paste text straight into the chat.

It will count what it received and tell you honestly whether that is enough:

> "Under 30 messages, treat these as signals rather than patterns. Fifty or more makes the next run much sharper."

Then it confirms the run and waits. Say go.

It clusters five to eight themes with real counts, cuts sentiment three ways, builds two or three persona cards from the customers actually in your data, and saves to `my-work/voice-of-customer/`.

### 5. Read the one section that matters most

Open the report and find **"Where the data disagrees with your profile"**.

This is the most valuable page in the session. It lists every place your customers contradict what you believe about them. Founders are wrong about their own customers constantly, and this is the cheapest way to find out where.

**Take at least one finding from it back into `CLAUDE.md`.** Run `/brand-brain --rebuild` and update Section 5.

## What good looks like

Compare [`gur-and-ghee/my-work/voice-of-customer/`](examples/gur-and-ghee/my-work/voice-of-customer/) against [`little-lab/my-work/voice-of-customer/`](examples/little-lab/my-work/voice-of-customer/). Same skill, a food brand and a cosmetics brand, and the themes it surfaces are nothing alike.

---

## Check it worked

- [ ] `my-work/market-analyst/` has a dated intel report
- [ ] `my-work/voice-of-customer/` has a dated customer voice report
- [ ] You answered at least one "what only you can answer" question back into `brand-brain/`

---

## If it breaks

**The skill did not trigger when I described the job in plain English.**
Its `description` does not carry the words you used. Open the SKILL.md and add your phrasing to the description line. That is the fix, every time.

**Customer Researcher says my sample is too small.**
It will still run, it just labels the output as signals rather than patterns. Believe it. Go and export your full review set before the next run.

**The Competitive Analyst could not reach a competitor's site.**
It will say so in the report and mark the price as unverified. That is correct behaviour, not a failure. Check that one price by hand and paste it into `brand-brain/competitors.md`.

---

## Take-home

Write your own skill. It takes 20 minutes and it is the step that makes this team yours: [`after-the-bootcamp/write-your-own-skill.md`](after-the-bootcamp/write-your-own-skill.md).

Run `/market-analyst` again in a week with the same competitor set. The second report is where the value is, because it can tell you what moved.

**Next:** [Session 04, Content Director](session-04-content-director.md)
