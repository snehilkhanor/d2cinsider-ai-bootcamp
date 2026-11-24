# Write your own skill

**Time:** 20 minutes, at home
**You walk out with:** a skill in your own handwriting that writes anything in your brand voice

During the live day you used skills somebody else wrote. This is where you write one yourself. Do it in the first week, while the day is fresh.

## Steps

In the prompt, type:

```
I want to write my own skill called write-in-brand-voice. It should write or rewrite any customer-facing copy in my brand's voice: emails, captions, product blurbs, WhatsApp replies. It must read CLAUDE.md Section 7 for the voice rules and 3 to 5 matching samples from brand-brain/voice-dna/ before writing anything. Create .claude/skills/write-in-brand-voice/SKILL.md. Ask me questions about my voice before you write it, do not guess.
```

Answer its questions. When it saves the file, **read it and edit it yourself.** Change a line. Add a rule it missed. It is your skill.

Then test it:

```
/write-in-brand-voice write a two line note for the card that goes in the box
```

If it does not sound like you, open the SKILL.md and fix the rule that let it through. That loop, run, judge, edit the file, is the whole skill of writing skills.

## Check it worked

- [ ] `.claude/skills/write-in-brand-voice/SKILL.md` exists and you edited it by hand
- [ ] Typing `/` now shows `write-in-brand-voice` in the list

## If it breaks

**My new skill runs but ignores my voice rules.**
It is not reading `CLAUDE.md` early enough. Open the SKILL.md and make step 1 explicitly "read CLAUDE.md Section 7 and 3 to 5 samples from brand-brain/voice-dna/ before writing a word".

**The skill did not trigger when I described the job in plain English.**
Its `description` does not carry the words you used. Open the SKILL.md and add your phrasing to the description line.
