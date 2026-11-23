# AI Declaration Coach

Feedback for DTU students on the part of a thesis or report that says how they used generative AI. The coach lists what to fix and asks for the details only the student can add. **It never writes the declaration for them.**

**Open the coach:** https://jahidul68.github.io/ai-declaration-check/ai-declaration-coach.html

> Thesis research tool. **Not an official DTU guide.** The feedback can be wrong; the supervisor and department have the final say.

---

## Contents

- [Who it is for](#who-it-is-for)
- [How to use it](#how-to-use-it)
- [What it checks](#what-it-checks)
- [What you get back](#what-you-get-back)
- [Privacy and data](#privacy-and-data)
- [Without CampusAI: copy-paste prompt](#without-campusai-copy-paste-prompt)
- [How it works](#how-it-works)
- [DTU sources](#dtu-sources)
- [For teachers and supervisors](#for-teachers-and-supervisors)
- [Research context](#research-context)
- [Feedback and survey](#feedback-and-survey)
- [Limitations](#limitations)

---

## Who it is for

- **DTU students** writing a project report, bachelor thesis or master's thesis who used generative AI and need to declare it.
- **Teachers and supervisors** who want students to check their own declarations before handing in, so they don't have to check every one themselves.

You need a **DTU account**. The coach runs on DTU CampusAI.

## How to use it

1. Open the coach at the link above.
2. Pick where you are:
   - **I have written it:** check my declaration and show me how to fix it.
   - **I haven't written it yet:** show me what it needs, with examples.
3. Paste your AI declaration (LaTeX is fine), **or** add your whole report as PDF, Word (`.docx`) or `.tex`. If you add the whole report, the coach finds the declaration itself.
4. **Sign in with DTU** when asked.
5. Press **Check my declaration**. It usually takes 2–3 minutes. Keep the page open.
6. Fix each point in your own words and tick it off. Then paste your new version and check again.

## What it checks

Six checks, based on DTU's rules:

| # | Check | Based on |
|---|-------|----------|
| 1 | You say clearly that you used AI, where a reader will find it | Study Announcement s1906 |
| 2 | You name the tool, its version or model, and when you used it | DTU Library |
| 3 | You say what you used it for, task by task | DTU Library |
| 4 | You say how you used it and what you did with the output | DTU Health Tech template |
| 5 | You say the work and the decisions are yours (AI is never an author) | Study Announcement s1906 |
| 6 | You reference and mark anything taken from AI | DTU Library |

Each check gets a level: **Covered**, **Partly**, **Not yet** or **Not needed**. These levels show where you stand. **They are not a grade.**

## What you get back

- **Up to 4 fixes**, most important first. Each fix has:
  - what to do, in a few words
  - the words from your text it is about
  - one plain sentence on why it matters
  - the detail **only you can add**
  - a good example from a **made-up project**, so you can't paste it in unchanged
  - a link to the DTU rule behind it
- **Where your declaration stands** on each of the six checks
- **What is already good**
- **Your own text, coloured** by what is covered, partly covered or against a rule
- **Short notes** on other DTU rules, but only when your text gives a reason (for example sensitive data, AI images, or AI used as part of your method)
- A **Copy feedback** button

## Privacy and data

- Your text is read **in your browser** and sent **only to DTU CampusAI**, DTU's own AI service, using your DTU sign-in.
- **GitHub only hosts the page.** It never receives your text.
- The page **stores nothing**. Your sign-in is kept only for the browser session, and the page remembers only which mode you picked.
- **Don't paste** personal, interview, patient or confidential company data.
- Keep your own AI chats (prompts, answers, dates, versions). Your supervisor can ask for them.

## Without CampusAI: copy-paste prompt

If you can't sign in to CampusAI, [`PROMPT.md`](PROMPT.md) has an older, text-only version of the check. Copy everything below the line into a new chat in any AI assistant, paste your declaration and write **Check my AI declaration**.

- It uses **8 checks** and gives a table, so its results differ from the coach.
- Your text then goes to that assistant's provider, not to DTU. Use a DTU-approved tool such as Microsoft Copilot with your DTU account.

## How it works

| Part | What it does |
|------|--------------|
| `ai-declaration-coach.html` | The whole app in one file: page, styles, script, prompt and DTU rules |
| DTU CampusAI | Signs you in with your DTU account and runs the model (`chat:think`) |
| pdf.js, JSZip (cdnjs) | Read PDF and Word files in your browser |
| GitHub Pages | Serves the static page |

There is no server, no database and nothing to build or install.

### Run it locally

Download `ai-declaration-coach.html` and open it in a browser. The DTU sign-in still works.

### Deploy your own copy

1. Fork or copy this repository.
2. Go to **Settings → Pages** and choose **Deploy from a branch**, then `main` and `/ (root)`.
3. Open `https://<your-name>.github.io/<repo>/ai-declaration-coach.html` and **test the DTU sign-in** before you share it.

## DTU sources

Every check and note links to one of these pages:

- [Study Announcement s1906: GenAI in project reports and final projects](https://student.dtu.dk/en/messages/studiemeddelelser/arkiv/study-announcement-s1906-guidelines-on-the-use-of-generative-ai-in-project-reports-and-final-project-assignments?lmsgid=98eeba12-9c99-478a-aced-b0e36071efa2)
- [DTU Library: How to declare the use of generative AI](https://www.bibliotek.dtu.dk/en/publishing/reference-management/kunstig-intelligens/eksempler)
- [DTU Library: Referencing when using generative AI](https://www.bibliotek.dtu.dk/en/publishing/reference-management/kunstig-intelligens)
- [DTU rules: Cheating at exams and other forms of assessment](https://student.dtu.dk/en/rules/exam/cheating-at-exams-and-other-forms-of-assessment)
- [DTU's code of honour](https://student.dtu.dk/en/exam/exam-cheating/dtu-code-of-honour)
- [DTU: guidelines for students on AI (Jan 2024)](https://www.dtu.dk/english/newsarchive/2024/01/dtu-opens-up-for-the-use-of-artificial-intelligence-in-teaching)
- [DTU AI Info Hub: Rules and FAQ](https://www.ai.dtu.dk/faq/)
- [DTU Health Tech: GAI declaration template](https://www.bardram.net/wp-content/uploads/2025/11/3.b.GAI-Declaration-Template-DTU-Health-Tech.pdf) (one department's form)

## For teachers and supervisors

- Share the link with students before hand-in, for example in DTU Learn or the course page.
- The coach gives formative feedback only. It **does not grade** and **does not decide** whether AI use was allowed.
- Your own course rules come first. If you expect something extra, such as a prompt appendix or a department form, tell students directly.

## Research context

The AI Declaration Coach is part of the master's thesis of **Jahid (s240010)**, MSc Human-Centered Artificial Intelligence, DTU. It sits within the **Erasmus+ HEGenAI project** on generative AI for feedback and assessment in higher education.

Supervisor: Md Saifuddin Khalid, DTU.

## Feedback and survey

Used the coach? Please answer the **[3-minute anonymous survey](https://forms.cloud.microsoft/e/URBh3UbvYw)**. It asks for no name or student number.

Found a bug or a wrong rule? Open an [issue](https://github.com/jahidul68/ai-declaration-check/issues).

## Limitations

- AI feedback can be wrong or miss things. Check it against DTU's rules and your supervisor's advice.
- It follows DTU's general rules. Your course, department or supervisor may ask for more.
- Scanned PDFs without text can't be read. Paste the declaration instead.
- Very long reports are cut at about 180,000 characters. If that happens, paste only the declaration.
- CampusAI usage limits apply. If it is busy, wait a minute and try again.
