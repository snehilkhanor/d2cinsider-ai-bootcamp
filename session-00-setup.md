# Session 0, Setup (pre-work)

**Time:** 30 minutes at home, before bootcamp day. This is mandatory pre-work. The live day starts with a short check, not an install.
**Live help:** there is a setup session on Zoom the evening before bootcamp day. Do as much of this as you can beforehand, and bring whatever is stuck. The time is in your email.
**You need:** a Mac or Windows laptop. A phone, tablet or Chromebook will not work.
**Primitive:** none yet, this is plumbing
**You walk out with:** the Claude Code desktop app installed, this repo open inside it, and one successful run

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

**On Windows:** run the downloaded `.exe`. It does not need admin rights.

> **Windows only, do this too.** Install **Git for Windows** from [git-scm.com/download/win](https://git-scm.com/download/win). It is a normal installer, you never open it afterwards. Accept every default. Without it some tools in the app fall back to a weaker mode. Mac already has what it needs.

## 2. Sign in

Open the app. Sign in with the same Anthropic account your Pro or Max plan is on.

You will see three tabs at the top: **Chat**, **Cowork** and **Code**.

**Click Code.** Everything in this bootcamp happens in the Code tab. If you find yourself in Chat, you are in the wrong place and skills will not appear.

## 3. Get the bootcamp folder onto your machine

No commands needed. You download a ZIP file and unzip it.

1. Open **[github.com/snehilkhanor/d2cinsider-ai-bootcamp](https://github.com/snehilkhanor/d2cinsider-ai-bootcamp)** in your browser.
2. Click the green **Code** button, then **Download ZIP**.
3. Find the ZIP in your Downloads folder and unzip it. On Mac, double-click it. On Windows, right-click it and choose **Extract All**.
4. Rename the unzipped folder to exactly `d2cinsider-ai-bootcamp` (GitHub adds `-main` to the end, remove that).
5. Move the folder into your home folder.

You end up with a folder at `~/d2cinsider-ai-bootcamp` on Mac, or `C:\Users\you\d2cinsider-ai-bootcamp` on Windows.

> **Do not put it in iCloud Drive, OneDrive or Dropbox.** Sync services rewrite files under the app while it is working. Put it directly in your home folder.

> **Windows: check for a folder inside a folder.** Extract All sometimes creates `d2cinsider-ai-bootcamp-main` with another `d2cinsider-ai-bootcamp-main` inside it. The one you want is the inner one, the one that directly contains `README.md`.

## 4. Open the folder in the app

In the **Code** tab, click **Select folder** and choose `d2cinsider-ai-bootcamp`.

The app will ask you to trust the folder. Say yes. Trust is what allows the skills in `.claude/skills/` to load, so if you decline, none of your teammates will exist.

## 5. Meet your teammates

Click into the prompt box and type a single forward slash:

```
/
```

A list appears. You should see `brand-brain`, `interview-me`, `market-analyst`, `voice-of-customer`, `ops-manager` and more. **That list is your roster.** Every one of those is a teammate defined in a file inside `.claude/skills/`.

If the list is empty or has none of those names, jump to troubleshooting at the bottom.

Press Escape to close the list without running anything.

## 6. Your first run

Type this into the prompt box and send it:

```
Read README.md and examples/little-lab/CLAUDE.md, then tell me in five lines what this repo is for and what a finished CLAUDE.md looks like.
```

Watch what happens. Claude will ask permission to read files, then answer. Two things to notice:

- **The permission card.** Claude asks before it touches anything. You can choose "Allow once" or "Always allow". For reading files inside this folder, "Always allow" is safe and will save you a hundred clicks on bootcamp day.
- **The file paths in the answer.** Click one. It opens in a file pane inside the app. You never need Finder or Explorer to read your teammates' work.

## 7. Set your permission mode

Find the permission mode selector near the prompt box. There are four:

| Mode | What it does | Use it when |
|---|---|---|
| **Manual** | Asks before every edit, shows you a diff | You are nervous, or reviewing someone else's work |
| **Accept edits** | Auto-approves file edits and safe commands | **Use this for the bootcamp** |
| **Plan** | Reads and proposes, never edits | You want a plan before any change |
| **Auto** | Fewer prompts, a safety classifier watches | Later, once you trust the setup |

**Set it to Accept edits** for the bootcamp. Your teammates write a lot of files and approving each one individually will eat your session.

## 8. Copy the brand-brain template

In the app prompt, type:

```
Copy the templates/brand-brain folder to the repo root as brand-brain/, keeping every file.
```

Then open `brand-brain/README.md` and start filling the files with your real data. This is the pre-work. Whatever you get done before Session 01 makes every session after it better.

---

> **Got 15 minutes more?** Do the optional [`practice-lab.md`](practice-lab.md). It teaches the five moves you will repeat all day.

> **Running out of time?** If bootcamp day arrives and this is not done, open [`catch-up.md`](catch-up.md). It gets you ready in ten minutes.

---

## Check it worked

You are ready for Session 01 when all five are true:

- [ ] The app is open on the **Code** tab
- [ ] The folder `d2cinsider-ai-bootcamp` is selected and trusted
- [ ] Typing `/` shows at least ten teammate names
- [ ] Your first run answered and you clicked a file path to read something
- [ ] A `brand-brain/` folder exists at the repo root

---

## If it breaks

**The `/` list is empty, or missing teammates.**
The folder is not trusted, or you opened the wrong folder. Check the folder path shown in the app is the one containing `.claude/`. Re-select the folder and accept the trust prompt.

**"Claude Code requires a paid plan".**
Free tier will not work. Pro is enough for everything in Default scope.

**Windows: tools fail or commands do nothing.**
Git for Windows is missing. Install it from [git-scm.com/download/win](https://git-scm.com/download/win), then quit and reopen the app.

**Files keep reverting, or the app says a file changed underneath it.**
The repo is inside iCloud, OneDrive or Dropbox. Move it to your home folder and re-select it.

**The app is slow or a run stops halfway.**
Check the usage ring next to the model picker. If you are near your limit, wait for the reset or switch to Default scope for the session.

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
