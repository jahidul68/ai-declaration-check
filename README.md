# AI declaration check

Feedback on the part of your DTU thesis or report where you declare your use of generative AI.

You get a table with 8 checks, based on DTU's rules (declare, take responsibility, document). Each check is marked **Done**, **Half done**, **Missing** or **Not relevant**, with one hint on what to add. It never writes the declaration for you.

This is feedback, not an official DTU assessment. Your supervisor and DTU's rules decide.

---

## Option A — Copy-paste (any AI chat, no setup)

1. Open [`PROMPT.md`](PROMPT.md) and copy everything below the line.
2. Paste it into a new chat in any AI assistant (Microsoft Copilot, ChatGPT, Claude, Gemini).
3. Paste your declaration section and write: **Check my AI declaration.**

## Option B — VS Code with GitHub Copilot (install once, reuse)

Copilot is free for verified students through [GitHub Education](https://education.github.com/).

**Install once (about 5 minutes)**

1. On this page, click **Code → Download ZIP** and unzip it.
2. Copy the folder `skills/ai-declaration-check` into your personal skills folder:
   - Windows: `C:\Users\<your-name>\.copilot\skills\`
   - Mac/Linux: `~/.copilot/skills/`

   Create the `.copilot` and `skills` folders if they do not exist. You should end up with `.copilot/skills/ai-declaration-check/SKILL.md`.
3. Restart VS Code.

**Each time you want feedback**

1. Get your thesis into VS Code. The simplest way: in Overleaf, **Menu → Download → Source**, unzip, and open the folder in VS Code (**File → Open Folder**).
2. Open Copilot Chat, switch to **Agent** mode, and write: **Check my AI declaration.**
3. Fix what the table says, download again, and ask again.

If Copilot does not seem to use the skill, check that Agent Skills are enabled in VS Code settings (search for "skills"), or type `/ai-declaration-check` in the chat.

## What you will see

```
AI declaration check — section: "Declaration of use of generative AI"

| # | Check                          | Status       | What to add or fix                                   |
|---|--------------------------------|--------------|------------------------------------------------------|
| 1 | Use is declared                | Done         | —                                                    |
| 2 | Tool named                     | Done         | —                                                    |
| 3 | Version and date               | Missing      | Add the model/version and when you used it.          |
| 4 | What it was used for           | Half done    | Say concretely what the tool did, not only "helped". |
| 5 | Where in the report            | Missing      | Say which chapters, sections or code were affected.  |
| 6 | Responsibility                 | Missing      | State the content is your responsibility and how you checked the AI output. |
| 7 | Prompts and outputs documented | Missing      | Say where your saved prompts and outputs can be found. |
| 8 | Copied AI output cited         | Not relevant | —                                                    |

Score: 2.5 of 7
Start with: Row 6 — responsibility is one of DTU's three core requirements.
```

## Rules it is based on

See [`skills/ai-declaration-check/references/dtu-rules.md`](skills/ai-declaration-check/references/dtu-rules.md), summarised from DTU Library and the DTU AI Info Hub.

## Research

This check is part of an MSc thesis study at DTU on GenAI feedback. On the first check the assistant asks whether you want an anonymous summary line you can choose to paste into the study's form. Saying no changes nothing. Nothing is sent anywhere automatically.
