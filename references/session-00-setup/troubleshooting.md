# Session 00, Troubleshooting

Everything that goes wrong before you have written a line of brand copy, and what to do about it. Work down the list, the causes are ordered by how often they actually happen.

---

## The app

### "Claude Code requires a paid plan"
Claude Code does not run on the free tier. You need **Pro, Max, Team or Enterprise**. Check which plan you are on at [claude.ai](https://claude.ai) under your account settings. Pro is enough for everything in this bootcamp at Default scope.

If you just upgraded, sign out of the desktop app and back in. The app caches your plan at sign-in.

### I signed in but I am in the wrong place
There are three tabs at the top: **Chat**, **Cowork** and **Code**.

**Everything in this bootcamp happens in Code.** If you are in Chat, your skills will not appear and no files will be created. Click Code.

### The app will not install on Windows
It does not need admin rights, so an admin prompt means something else is intercepting it. Try downloading again from the official quickstart page rather than a copied link, and check your organisation's device policy is not blocking unsigned installs.

### The app is slow, or a run stops halfway through
Type `/usage` to see how much of your plan's allowance is left. If you are close to your limit, the fix is to wait for the reset or run sessions at Default scope rather than Power. A run that stops halfway usually shows why in the Tasks pane.

---

## The folder

### `brand-brain` and the other teammates are not in the `/` list
Two causes.

**1. The app is open in a different folder from the one that was set up.** This is the common one. It happens when a folder was chosen by hand before the setup paste ran. Paste: `Does .claude/skills/brand-brain/SKILL.md exist in the folder this chat is open in? Answer yes or no, and tell me the folder path.` If no, click the folder name under the prompt box and choose the folder your setup answer named on its first line.

**2. The hidden `.claude` folder is missing.** Finder and Explorer hide folders that start with a dot, so it can go missing without anything looking wrong. It is lost when files are moved or copied after downloading. Paste: `The .claude folder is missing here. Download https://github.com/snehilkhanor/d2cinsider-ai-bootcamp/archive/refs/heads/main.zip and copy its .claude folder into this folder, so that .claude/skills/brand-brain/SKILL.md exists here. Then list the folders inside .claude/skills/.`

The `/` list is long and also shows the app's own commands. Type `/brand-brain` to filter it.

### The folder is inside iCloud, OneDrive or Dropbox
Move it. Sync services rewrite files underneath the app while it is working, which produces file-changed errors, reverted edits and work that silently disappears.

Put the folder directly in your home folder:
- Mac: `/Users/yourname/d2cinsider-ai-bootcamp`
- Windows: `C:\Users\yourname\d2cinsider-ai-bootcamp`

Then select it again in the app.

### The ZIP will not download or unzip
Try a different browser. On Windows, right-click the ZIP and choose **Extract All**, do not just double-click it. Then rename the folder to `d2cinsider-ai-bootcamp` and move it into your home folder.

### Do I need Git on Windows?
Normally no. The setup paste downloads the folder without it, and this was tested on a Windows laptop with no Git installed.

Keep it as a backup. If the setup paste fails and downloading the ZIP by hand fails too, or a later session reports that a command could not run, install **Git for Windows** from [git-scm.com/download/win](https://git-scm.com/download/win), accept every default, then quit and reopen the Claude app and try again.

---

## Permissions

### It asks permission for every single thing
Set the permission mode to **Auto**, at the bottom right of the window. It is the app's default. Manual mode asks before every file write, which is right for careful review and wrong for a session where a teammate writes forty files.

The five modes are Auto, Manual, Accept edits, Plan and Bypass permissions. Use Auto for the bootcamp, or Accept edits if you do not see Auto. Never use Bypass permissions.

### I approved something and want to take it back
Change the mode back to Manual and it will start asking again. Approvals are per tool, not permanent contracts.

---

## Skills and agents

### A skill exists but does not trigger when I describe the job in plain English
Its `description` does not contain the words you used. Open the `SKILL.md`, read the description line, and add your phrasing to it. This is the fix nearly every time.

You can always call it directly with `/skill-name` regardless.

### I edited a skill and nothing changed
Skills reload live within a session, but if you are unsure, ask: `Re-read .claude/skills/<name>/SKILL.md and tell me what step 1 says.` If it reports the old text, reopen the folder.

### A subagent started and I cannot see what it is doing
Look at the **Tasks pane**. Each running agent is a row. Click one to watch its live transcript. If there is no row, the agent did not start, and the usual reason is that the agent file has a typo in its frontmatter.

### A subagent stopped partway
Open its row in the Tasks pane and read the last thing it did. Most stops are a missing input file, and it will have said so. Re-run it after fixing the input rather than restarting the whole session.

---

## Connectors

### It connected but returns nothing
Scopes. Disconnect, reconnect, and actually read the permission screen instead of clicking through. Drive in particular needs access to the folders you care about.

### It is connected to the wrong account
**Stop and fix this before running anything else.** Ask `Which account am I connected to?` and confirm the answer names your business. Every report built on a wrong connection looks completely plausible and is completely useless.

### A connector I need is not in the Connectors list
It needs adding as a custom server, which lives in a file called `.mcp.json` at the root of this project. Ask Claude:

```
Add <service> as a project-scoped MCP server in .mcp.json, then tell me exactly what credential I need and where to get it.
```

If that turns into a fight, do not burn a session on it. Export the data to CSV, drop it in `brand-brain/`, and carry on. Every skill in this bootcamp works from files.

---

## Files

### I cannot find what a teammate wrote
Click the file path in the chat. It opens in a file pane inside the app. You do not need Finder or Explorer.

To list everything: `List every file in my-work/, grouped by folder, with the date each was created.`

### A file I expected is not there
Check the teammate's index file first. Most skills write a "what I did not do" section explaining exactly what they skipped and why, and the reason is usually a missing input rather than a failure.

---

## Still stuck

Ask the app itself. It can read this repo:

```
Something is wrong with my setup. Read README.md and session-00-setup.md, check what actually exists in this folder, and tell me what is missing.
```

On Zoom, use **Raise hand**. A TA will take you into a breakout room.
