# Humanizer v3.4.1

Remove AI writing patterns from B.Tech project reports — and any other writing.

Built for CSE/IT students writing their final year project reports. Works for essays, articles, and documentation too.

---

## The problem

Most B.Tech project reports open with:

> "In today's rapidly evolving technological landscape, this project aims to develop a proposed system that enhances user experience..."

Examiners have read that sentence ten thousand times. It signals immediately that the student didn't write this — and they stop reading carefully.

The Humanizer fixes that. It strips 24 documented AI writing patterns and replaces them with writing that sounds like you actually built something.

---

## What it fixes

**Report-specific patterns:**
- Generic openers ("In today's rapidly evolving technological landscape...")
- Passive voice overload ("it was observed that", "testing was conducted")
- Vague performance claims ("the system performed well") — replaced with real numbers
- "The proposed system" — replaced with what you actually built
- Literature review that just lists papers without connecting them to your problem
- Abstract that describes the report structure instead of the findings
- Conclusion that repeats the introduction

**General AI writing patterns:**
- Overused AI vocabulary (crucial, pivotal, leverages, showcases, underscores...)
- Em dash overuse
- Inline-header bullet lists
- Forced rhetorical structure (rule of three, negative parallelism)
- Promotional language (nestled, breathtaking, groundbreaking...)
- Vague attributions (experts argue, industry observers...)
- Sycophantic tone and chatbot artifacts
- Excessive hedging and filler phrases
- Synonym cycling and false ranges
- And 9 more — see the full file

---

## Files in this repo

| File | What it is | What to do with it |
|---|---|---|
| `humanizer-v3.4.1.md` | Full humanizer instructions | Upload to your Claude project |
| `student-setup-guide.html` | Step-by-step setup guide with UI mockups | Open in browser |
| `README.md` | This file | Read it |
| `LICENSE` | MIT License | Nothing, just legal |

---

## Setup — 5 minutes, free

### Step 1 — Create a Claude.ai account
Go to [claude.ai](https://claude.ai) and sign up. The free tier is enough for an entire project report.

### Step 2 — Create a new Project
In the left sidebar, click **Projects** → **New project**. Name it something like `B.Tech Report`.

### Step 3 — Upload the humanizer file
Inside your project, find the **Files** section. Click **+** and upload `humanizer-v3.4.1.md`.

### Step 4 — Add the standing instructions
Click **+** next to **Instructions**. Paste this exactly:

```
You are a humanizer editor. Apply the humanizer checklist to all writing.
- For B.Tech reports and long-form writing: show draft → audit → final pass
- For short replies: apply silently, just write clean
- For B.Tech reports: every factual claim needs a real number or source
- At session start: ask the user to upload their project synopsis before writing anything
- Full instructions are in the uploaded file humanizer-v3.4.1.md — read it at session start
```

### Step 5 — Test it
Start a new conversation inside the project. Claude will ask for your project synopsis. Upload it. Then paste any report section and say which chapter it is.

You get: **draft → audit → final pass** — with a checklist of anything that still sounds AI-generated.

---

## How to use it

For each report section:

1. Start a new conversation inside your Claude project
2. Upload your project synopsis when Claude asks
3. Paste the section you want to humanize
4. Tell Claude which section it is: *"This is my Introduction. Humanize it."*
5. Get draft → audit → final output
6. Copy the final version into your report

---

## For professors

Download both files and share with your batch:

- `humanizer-v3.4.1.md` — students upload to their Claude project
- `student-setup-guide.html` — students open in browser for the full visual setup guide

The instructions auto-configure to each student's project from their uploaded synopsis. No editing needed between students or projects.

---

## How it works — the session start protocol

At the start of every conversation, Claude asks for your project synopsis (2-3 pages). It reads the document silently, extracts your project title, tech stack, methodology, and key metrics, then confirms before starting.

This means:
- You never type out project details manually
- Every humanized section uses language specific to your actual project
- The instructions work for any project without editing

---

## Version history

| Version | Changes |
|---|---|
| v3.4.1  | B.Tech report quality checklist, preliminary pages section, formatting rules, acknowledgements protocol, clarity fixes |
| v3.4.0 | Synopsis upload session start, fully generic (no hardcoded project names) |
| v3.3.0 | Three-question session start protocol |
| v3.2.0 | Reviewer persona, "did you actually build this" checklist, red flags quick reference |
| v3.1.0 | B.Tech report mode, section tone calibration, report section template |
| v3.0.0 | Soul/personality layer, second voice example, merged overlapping patterns |
| v2.3.0 | Initial release |

---

## License

MIT — free to use, share, and modify. See `LICENSE` for details.

Patterns adapted from [Wikipedia:Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) (CC BY-SA 4.0).
Original instructions, B.Tech additions, and session protocol are original work.
