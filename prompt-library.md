# Reusable Prompt Library

Every prompt from the bootcamp in one file, in the order you used them. Copy, change the details, paste.

Each heading links to the session it came from, where the surrounding steps explain when to use it and what to check afterwards.

---

## [Setup](session-00-setup.md)

**Set up the bootcamp folder with one paste**

```
Set up the D2C Insider AI Bootcamp on this computer.

1. Decide where it goes. If this chat is open in a folder of mine and that folder is empty, use that folder. Otherwise create a folder called d2cinsider-ai-bootcamp inside my home folder and use that. If the folder you would use already has files in it, stop and ask me.
2. Download https://github.com/snehilkhanor/d2cinsider-ai-bootcamp/archive/refs/heads/main.zip and unpack it directly into that folder, so that README.md sits at the top level of the folder and not inside a subfolder. Do not use git and do not install anything.
3. Check the hidden folder came with it: .claude/skills/ must contain 11 folders and .claude/agents/ must contain 3 files. If not, fix it.
4. Copy templates/brand-brain to brand-brain inside that folder, keeping every file.
5. Finish with exactly three lines and nothing else. Line one: the full path of the folder. Line two: "Skills: 11, Agents: 3" if the check passed. Line three: if this chat is already open in that folder, write "Ready. Type /brand-brain and check it appears in the list. Do not press Enter." Otherwise write "Next: click the folder name under the prompt box, choose the folder above, then type /brand-brain and check it appears in the list. Do not press Enter."
```

**Your first run**

```
Read README.md and examples/little-lab/CLAUDE.md, then tell me in five lines what this repo is for and what a finished CLAUDE.md looks like.
```

**Fill your brand folder**

```
Open brand-brain/README.md and tell me which file to fill first.
```

**If it breaks**

```
Does .claude/skills/brand-brain/SKILL.md exist in the folder this chat is open in? Answer yes or no, and tell me the folder path.
```

---

## [Practice lab](practice-lab.md)

**Ask about one file**

```
Read examples/little-lab/sample-inputs/reviews-export.csv and give me a five line summary of what customers are saying. Split it into what is working and what is not.
```

**Ask across several files**

```
Some reviews say the Bath and Hair Wash "doesn't lather". Check the other files in examples/little-lab/sample-inputs/ as well. How often does this come up, and what is the customer actually worried about?
```

**Have it write a file**

```
Write a one-page summary of Little Lab's top three customer complaints, with one real quote for each, and save it as my-work/practice/complaints.md
```

**Have it change a file**

```
In my-work/practice/complaints.md, add a short line under each complaint suggesting what the brand could say on the product page to prevent it.
```

**Push back**

```
The second suggestion sounds like marketing. Rewrite it the way a founder would say it to a customer on WhatsApp.
```

**Clean up**

```
Delete the folder my-work/practice/
```

---

## [Catch-up kit](catch-up.md)

**Situation 2: the app works, but `brand-brain/` is empty**

```
Copy templates/brand-brain to brand-brain/ if it does not exist yet. Then build a first draft of my brand-brain from my website: https://your-brand.com. Read the home page, the about page and my top three product pages. Fill positioning.md, products.csv and competitors.md with what you find. Mark every line you guessed with [CONFIRM]. Then ask me five questions, one at a time, to fix the most important guesses.
```

**Situation 2: the app works, but `brand-brain/` is empty**

```
Save everything below into brand-brain/reviews.md exactly as written. Do not tidy or summarise it.
```

**Situation 2: the app works, but `brand-brain/` is empty**

```
Save each of the pieces below as its own file in brand-brain/voice-dna/. Do not edit a word.
```

**Situation 3: you have nothing to paste**

```
Copy examples/little-lab/brand-brain to brand-brain/, keeping every file.
```

---

## [01 Brand Strategist](session-01-brand-strategist.md)

**Check it worked**

```
Write me a two line Instagram caption announcing that we are back in stock.
```

---

## [02 Competitive Analyst and 03 Customer Researcher](session-02-03-competitive-analyst-customer-researcher.md)

**Look at a skill before you run one**

```
Show me .claude/skills/market-analyst/SKILL.md
```

**Run the Competitive Analyst**

```
/market-analyst
```

**Run the Customer Researcher**

```
/voice-of-customer
```

---

## [04 Content Director](session-04-content-director.md)

**Look at the subagent definition**

```
Show me .claude/agents/content-lead.md
```

**Start it**

```
Use the content-lead agent to produce this month's content.
```

**Pick your scope**

```
Use the content-lead agent with FULL_RUN=yes to produce this month's content.
```

---

## [05 Ad Creative Lead](session-05-ad-creative-lead.md)

**Run it**

```
Use the performance-marketer agent to build this month's ads.
```

**Run it**

```
Use the performance-marketer agent with ANGLES=1,3
```

**Run it**

```
Use the performance-marketer agent with FULL_RUN=yes
```

**Turn one angle into a creative brief**

```
/creative-brief
```

---

## [06 Marketplace Manager](session-06-marketplace-manager.md)

**Rewrite two product pages**

```
/pdp-writer
```

**Read the gap analysis before the rewrite**

```
The page leads with: ...
Customers actually care about: ... (with a count)
Competitors emphasise, and we do not: ...
Unanswered here, but asked constantly in support: ...
Biggest conversion blocker, best guess: ...
```

**Rewrite the marketplace listings**

```
/marketplace-editor
```

---

## [07 Ops Lead and 08 Support and Retention Manager](session-07-08-ops-lead-support-retention.md)

**Write the operations down**

```
/ops-manager
```

**Build the retention flows**

```
/retention-manager
```

**Write the support playbook**

```
Using my latest customer voice report and the retention templates you just wrote, write my-work/retention-manager/support-playbook.md. Include the eight questions and complaints customers raise most, with a count for each from my data, and an approved reply for each in my brand voice. Then add when to refund, when to replace and when to escalate to me, following the compliance rules in CLAUDE.md. Flag any reply where you had to guess my policy.
```

---

## [09 Growth Analyst](session-09-growth-analyst.md)

**Run the brief**

```
/growth-analyst
```

**Schedule it**

```
Run the growth-analyst skill for this brand. Regenerate the brief, the numbers file and the dashboard for the last 7 days.

Then reply with three things only: the headline sentence, the one alarm in a single line, and the path to the dashboard. Nothing else. The full read lives in the file.
```

**Save what you set up (at home)**

```
Write my-work/growth-analyst/schedule-config.md describing what I just scheduled: the routine name, when it runs, what it produces, how to pause it for a holiday and how to change the time.
```

---

## [10 Chief of Staff](session-10-chief-of-staff.md)

**Check the chain is alive**

```
For each folder in my-work/, tell me the most recent file and how many days old it is. Flag anything older than 14 days.
```

**Run the Chief of Staff**

```
Use the captain agent to produce my 90 day roadmap.
```

**Settle the standing schedule**

```
Use the captain agent with WIRE_SCHEDULE=yes and DELIVERY=email to set up the recurring runs.
```

**Build your command center**

```
Create my-work/command-center.md. One page. At the top: this week's one alarm from the Growth Analyst, and my Monday ship. Then a table with one row per teammate: what they last produced, the date, and a link to their latest index file. Then my three priorities for this month from the roadmap, and the standing schedule. Use only what is in the index files, do not open raw outputs.
```

---

## [After the bootcamp: write your own skill](after-the-bootcamp/write-your-own-skill.md)

**Steps**

```
I want to write my own skill called write-in-brand-voice. It should write or rewrite any customer-facing copy in my brand's voice: emails, captions, product blurbs, WhatsApp replies. It must read CLAUDE.md Section 7 for the voice rules and 3 to 5 matching samples from brand-brain/voice-dna/ before writing anything. Create .claude/skills/write-in-brand-voice/SKILL.md. Ask me questions about my voice before you write it, do not guess.
```

**Steps**

```
/write-in-brand-voice write a two line note for the card that goes in the box
```

---

## [After the bootcamp: connectors](after-the-bootcamp/connectors.md)

**Connect your store**

```
Add the Shopify MCP server to this project as a project-scoped server in .mcp.json, then tell me exactly what I need to authenticate and where I get it.
```

**Verify the connection points at the right place**

```
Which store am I connected to? Give me the store name, the domain and the currency.
```

**Pull something real**

```
Using the connected store, show me my top 10 products by orders over the last 30 days, with conversion rate and average rating for each.
```

**Re-run Voice of Customer on live data**

```
/voice-of-customer

Use the connected store for order and customer data, and search Gmail for customer support threads from the last 60 days. Cross-reference the themes against my product performance.
```

**Point it at your nominated SKUs**

```
Re-run the sentiment cut for only the five SKUs in brand-brain/nominated-skus.md, and tell me which of the five has the biggest gap between its rating and its conversion rate.
```

---

## [After the bootcamp: Influencer Scout](after-the-bootcamp/influencer-scout.md)

**Get a creator pool**

```
Use references/after-bootcamp-influencer-scout/sample-creator-pool.json as my creator pool.
```

**Run it**

```
/influencer-scout
```

**Run it**

```
/influencer-scout give me ten creators and a four week ladder
```
