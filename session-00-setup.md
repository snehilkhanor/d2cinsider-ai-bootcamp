# Session 0, Setup (pre-work)

**Time:** 15 minutes at home, before bootcamp day. This is mandatory pre-work. The live day starts with a short check, not an install.
**Live help:** there is a setup session on Zoom the evening before bootcamp day. Do as much of this as you can beforehand, and bring whatever is stuck. The time is in your email.
**You need:** a Mac or Windows laptop. A phone, tablet or Chromebook will not work.
**Primitive:** none yet, this is plumbing
**You walk out with:** the Claude Code desktop app installed, the bootcamp folder open inside it, and one successful run

---

## Before you start

- [ ] A Claude **Pro or Max** plan. Claude Code does not run on the free tier. Check at [claude.ai](https://claude.ai) under your account.
- [ ] A Mac or a Windows machine you can install software on.
- [ ] About 2 GB of free disk.

---

## 1. Install the app

Go to the desktop quickstart and download the installer for your machine:

**[code.claude.com/docs/en/desktop-quickstart](https://code.claude.com/docs/en/desktop-quickstart)**

**On Mac:** open the downloaded `.dmg` and drag Claude into Applications. Open it from Applications.

**On Windows:** run the downloaded installer and accept the defaults.

That is the only thing you install. There is no terminal, and nothing else to download by hand.

## 2. Sign in and find the Code tab

Open the app. Sign in with the account your Pro or Max plan is on.

At the top of the window there are tabs. **Click Code.** Everything in this bootcamp happens in the Code tab. If you find yourself in Chat, you are in the wrong place and your teammates will not appear.

**Check where it is running.** The app shows an environment, at the side of the window or under the prompt box. It must say **This computer**. If it offers a cloud or remote environment, do not choose it. Your files have to live on your own laptop.

## 3. Set up the bootcamp folder with one paste

Copy everything in the box below, paste it into the prompt box, and press Enter.

```
Set up the D2C Insider AI Bootcamp on this computer.

1. Decide where it goes. If this chat is open in a folder of mine and that folder is empty, use that folder. Otherwise create a folder called d2cinsider-ai-bootcamp inside my home folder and use that. If the folder you would use already has files in it, stop and ask me.
2. Download https://github.com/snehilkhanor/d2cinsider-ai-bootcamp/archive/refs/heads/main.zip and unpack it directly into that folder, so that README.md sits at the top level of the folder and not inside a subfolder. Do not use git and do not install anything.
3. Check the hidden folder came with it: .claude/skills/ must contain 11 folders and .claude/agents/ must contain 3 files. If not, fix it.
4. Copy templates/brand-brain to brand-brain inside that folder, keeping every file.
5. Finish with exactly three lines and nothing else. Line one: the full path of the folder. Line two: "Skills: 11, Agents: 3" if the check passed. Line three: if this chat is already open in that folder, write "Ready. Type /brand-brain and check it appears in the list. Do not press Enter." Otherwise write "Next: click the folder name under the prompt box, choose the folder above, then type /brand-brain and check it appears in the list. Do not press Enter."
```

It takes a minute or two. If the app asks permission to download or create files, say yes. It ends with three lines, like this:

```
C:\Users\you\d2cinsider-ai-bootcamp
Skills: 11, Agents: 3
Ready. Type /brand-brain and check it appears in the list. Do not press Enter.
```

**If the second line does not say `Skills: 11, Agents: 3`, stop and ask for help.** Do not carry on.

> **Do not make a folder yourself first.** The paste makes it for you. If you have already chosen an empty folder, that is fine, it will use that one.

> **Not in iCloud Drive, OneDrive or Dropbox.** If the path on line one contains any of those words, tell a TA. Sync services rewrite files under the app while it is working.

## 4. Open the folder, if it asks you to

Read the third line of the answer.

- **If it says Ready,** you are already in the right folder. Go to step 5.
- **If it says Next,** click the folder name under the prompt box and choose the folder named on line one. If the app asks whether you trust the folder, say yes.

## 5. Meet your teammates

Click into the prompt box and type this, **without pressing Enter**:

```
/brand-brain
```

A list appears with `brand-brain` at the top. Hover over it and its description ends with **(project)**. That label means the teammate comes from your bootcamp folder. Press Escape to close the list.

If you press Enter by mistake, it starts the brand interview. Reply "stop, I will do this on bootcamp day".

To see everyone, clear the box and type just `/`. The list is long, because it also includes the app's own commands such as `plan`, `usage` and `skills`. Yours are `brand-brain`, `interview-me`, `market-analyst`, `voice-of-customer`, `ops-manager` and the rest. **Those are your roster.**

## 6. Your first run

Start a new chat. Type this into the prompt box and send it:

```
Read README.md and examples/little-lab/CLAUDE.md, then tell me in five lines what this repo is for and what a finished CLAUDE.md looks like.
```

You do not have to type prompts exactly. Close enough works.

Two things to notice:

- **It read the files itself.** You did not upload or paste anything.
- **The file paths in the answer are links.** Click one. It opens inside the app. You never need Finder or Explorer to read your teammates' work.

## 7. Check your permission mode

At the bottom right of the window, next to the model name, is the mode. **It should already say Auto.** That is the app's default and it is the right one for the bootcamp. If it says something else, click it and choose Auto.

| Mode | What the app says | Use it when |
|---|---|---|
| **Auto** | Claude handles permission decisions | **The bootcamp.** It checks each action for risk before running it |
| **Accept edits** | Automatically accept all file edits | You do not see Auto. You will be asked now and then before it runs a command |
| **Manual** | Always ask before making changes | You are reviewing something carefully. Too slow for bootcamp day |
| **Plan** | Create a plan before making changes | You want to see a plan before anything is touched |
| **Bypass permissions** | Accepts all permissions | **Do not use this.** It removes every safety check |

## 8. Fill your brand folder

The paste in step 3 already made a `brand-brain/` folder for you, with empty files to fill. Paste this to open its guide:

```
Open brand-brain/README.md and tell me which file to fill first.
```

Then start filling the files with your real data. This is the pre-work that matters. Whatever you get done before Session 01 makes every session after it better.

---

> **Got 15 minutes more?** Do the optional [`practice-lab.md`](practice-lab.md). It teaches the five moves you will repeat all day.

> **Running out of time?** If bootcamp day arrives and this is not done, open [`catch-up.md`](catch-up.md). It gets you ready in ten minutes.

---

## Check it worked

You are ready for Session 01 when all five are true:

- [ ] The app is open on the **Code** tab, running on **This computer**
- [ ] The setup paste ended with `Skills: 11, Agents: 3`
- [ ] Typing `/brand-brain` shows it in the list, marked (project)
- [ ] Your first run answered and you clicked a file path to read something
- [ ] A `brand-brain/` folder exists and you have started filling it

---

## If it breaks

**`brand-brain` is not in the list.**
The app is open in a different folder from the one that was set up, or the hidden `.claude` folder is missing. You cannot see that folder in Finder or Explorer, so ask. Paste this:

```
Does .claude/skills/brand-brain/SKILL.md exist in the folder this chat is open in? Answer yes or no, and tell me the folder path.
```

If no, click the folder name under the prompt box and choose the folder from line one of your setup answer. Also check you are in the Code tab, not Chat.

**The setup paste failed, or stopped halfway.**
Do it by hand. Open [github.com/snehilkhanor/d2cinsider-ai-bootcamp](https://github.com/snehilkhanor/d2cinsider-ai-bootcamp), click the green **Code** button, then **Download ZIP**. Unzip it, rename the folder to `d2cinsider-ai-bootcamp`, and move the whole folder into your home folder. On Windows, if Extract All made a folder inside a folder, use the inner one, the one that directly contains `README.md`. Choose that folder under the prompt box, then paste: `Copy templates/brand-brain to brand-brain, keeping every file.`

**Windows, and neither of those worked.**
Last resort. Install **Git for Windows** from [git-scm.com/download/win](https://git-scm.com/download/win). It is a normal installer: accept every default, and you never open it afterwards. Quit the Claude app, open it again, and run the setup paste once more.

**"Claude Code requires a paid plan".**
The free plan will not work. Pro is enough for everything in Default scope.

**Files keep reverting, or the app says a file changed underneath it.**
The folder is inside iCloud, OneDrive or Dropbox. Move it to your home folder and choose it again.

**The app is slow or a run stops halfway.**
Type `/usage` to see how much of your plan's allowance is left. If you are near the limit, wait for the reset.

**Anything else.** [`references/session-00-setup/troubleshooting.md`](references/session-00-setup/troubleshooting.md).

---

## Take-home

Fill in as much of `brand-brain/` as you can before bootcamp day. Session 01 is 70 minutes and it runs on what is in this folder. In priority order:

1. `voice-dna/`, five things you actually wrote
2. `reviews.md`, as many real reviews as you can paste, including the bad ones
3. `positioning.md`, one honest paragraph
4. `products.csv`, your real SKUs and numbers
5. everything else

**Next:** [Session 01, Brand Strategist](session-01-brand-strategist.md)
