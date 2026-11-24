# D2C Insider AI Bootcamp

The student folder for the one-day D2C Insider AI Bootcamp. Download it, open it in the Claude Code desktop app, and work through the sessions in order.

By the end of the day you have ten AI teammates working on your brand, your data and your competitors, plus a 90 day plan for what they do next.

**Lead instructor:** Snehil Khanor

**Start here:** [`student-handbook.md`](student-handbook.md), then [`session-00-setup.md`](session-00-setup.md). Setup is pre-work. Do it at home before bootcamp day.

**Lost in the folder?** Open [`site/index.html`](site/index.html) in any browser for a one-page reference.

---

## How it runs

Everything happens in the **Claude Code desktop app**, the Mac and Windows application. There is no terminal and no command line anywhere in this bootcamp. You install an app, point it at a folder, and type in a chat box.

## The day, 9 AM to 7 PM IST, live on Zoom

| Time | Session | You walk out with |
|---|---|---|
| 9:00 | Welcome, keynote, setup check | Everyone's app open on this folder |
| 9:40 | [01 Brand Strategist](session-01-brand-strategist.md) | `CLAUDE.md` in your voice |
| 10:50 | Break | |
| 11:05 | [02 Competitive Analyst and 03 Customer Researcher](session-02-03-competitive-analyst-customer-researcher.md) | Competitor report, customer voice report |
| 12:05 | [04 Content Director](session-04-content-director.md) | 30 day calendar and ready pieces |
| 1:00 | Lunch | |
| 1:45 | [05 Ad Creative Lead](session-05-ad-creative-lead.md) | Ad copy bank and creative briefs |
| 2:40 | [06 Marketplace Manager](session-06-marketplace-manager.md) | Rewritten PDPs, Amazon and Flipkart listings |
| 3:35 | Break | |
| 3:50 | [07 Ops Lead and 08 Support and Retention Manager](session-07-08-ops-lead-support-retention.md) | SOPs, vendor kit, WhatsApp flows |
| 4:50 | [09 Growth Analyst](session-09-growth-analyst.md) | Weekly brief and unit economics |
| 5:40 | [10 Chief of Staff](session-10-chief-of-staff.md) | 90 day roadmap |
| 6:30 | Share-outs and your Monday plan | One thing chosen to ship on Monday |

## The roster

| # | Teammate | How you call them | Owns |
|---|---|---|---|
| 01 | Brand Strategist | `/interview-me` or `/brand-brain`, writes `CLAUDE.md` | Brand DNA, voice rules, compliance |
| 02 | Competitive Analyst | `/market-analyst` | Competitor intel, pricing, cadence |
| 03 | Customer Researcher | `/voice-of-customer` | Themes, sentiment, persona cards |
| 04 | Content Director | `content-lead` subagent | 30 day calendar, pieces, listings |
| 05 | Ad Creative Lead | `performance-marketer` subagent and `/creative-brief` | Ad angles, variants, briefs |
| 06 | Marketplace Manager | `/pdp-writer` and `/marketplace-editor` | PDPs, landing pages, Amazon and Flipkart listings |
| 07 | Ops Lead | `/ops-manager` | SOPs, vendor kit, returns |
| 08 | Support and Retention Manager | `/retention-manager` | Support playbook, WhatsApp and email flows |
| 09 | Growth Analyst | `/growth-analyst` | Weekly brief, unit economics, dashboard |
| 10 | Chief of Staff | `captain` subagent | Cross-team read, 90 day roadmap |

## Layout

```
d2cinsider-ai-bootcamp/
├── student-handbook.md              the master map, read this first
├── session-00-setup.md              pre-work, do it at home
├── practice-lab.md                  optional 15 minute warm-up
├── catch-up.md                      if you did not do the pre-work
├── prompt-library.md                every prompt from the day, in one file
├── session-01 ... session-10        one file per live session
├── after-the-bootcamp/              connectors and influencer scout, for the weeks after
├── CLAUDE.template.md               the file Session 1 fills in
├── resources.md                     what to add after the bootcamp
├── templates/
│   └── brand-brain/                 copy this to brand-brain/ and fill it
├── .claude/
│   ├── skills/                      11 skills, loaded automatically
│   └── agents/                      3 subagents
├── references/                      optional deep dives and take-home reading
├── site/                            browsable reference, open index.html
└── examples/
    ├── little-lab/                  baby skincare, CDSCO, marketplace-heavy
    └── gur-and-ghee/                jaggery sweets, FSSAI, own site and quick commerce
```

Two folders get created as you work: `brand-brain/`, your inputs, and `my-work/`, your teammates' output. Both stay on your machine. Your business data is never uploaded to this repo.

## Two rules in every session

**Index files, not raw outputs.** Every teammate writes a short index of what it produced. The Chief of Staff reads only those indexes. That is what lets one agent sit across the whole team.

**Default and Power scope.** Every teammate asks you to pick at the start. Default fits a Pro plan and the live session slot. Power is for a Max plan or for re-running at home. Pick Default during the live day.

## The worked examples

Two fictional brands, each taken through all ten teammates.

| Brand | Category | Compliance | Distribution |
|---|---|---|---|
| [`examples/little-lab/`](examples/little-lab/) | Baby skincare | CDSCO | Amazon and Flipkart heavy |
| [`examples/gur-and-ghee/`](examples/gur-and-ghee/) | Jaggery sweets | FSSAI | Own site, quick commerce, corporate gifting |

When a session's instructions are clear but you cannot picture the output, open the matching folder in whichever brand is closer to yours. Start at [`examples/README.md`](examples/README.md).

## What you need

- A Claude **Pro or Max** plan. Claude Code does not run on the free plan.
- The **Claude Code desktop app** on a Mac or Windows laptop. A phone, tablet or Chromebook will not work.
- Your own brand data: reviews, product list, competitor names, and five things you wrote yourself. If something is missing, sample data is provided so you never sit out an exercise.
