# Vibe Coding II: Building a Prototype (Fall 2026)

**Companion Checklist**

*Follow this sheet through the plan-act-test-publish cycle. Record what Pi proposed, what you corrected, and where your site lives.*

## Setup

- ☐ API key created and pasted only into Pi's hidden prompt
- ☐ `node --version` and `git --version` work in a fresh window
- ☐ `npx @cuny-ai-lab/cail-pi` → Install everything → key → `pi` → `/model`
- ☐ Never `sudo` (recovery: `sudo chown -R $(whoami) ~/.npm ~/.pi`, `brew install node`, `npm install -g @earendil-works/pi-coding-agent`)

## Plan

```text
mkdir cv-site
cd cv-site
pi
```

Ask Pi to import your CV:

```text
Find my CV (a PDF or Word file, probably in my Downloads folder), copy it into this folder as cv.pdf or cv.docx, and save its text as cv.txt. For a PDF you can use: npx --yes pdf-parse text cv.pdf -o cv.txt
```

- ☐ `cv.txt` looks like my CV

**My design choices** (from the prompt builder on the slide):

| Layout | Style | Colors | Fonts | Mode | Sections |
|--------|-------|--------|-------|------|----------|
| | | | | | |

☐ Hide phone and address  ☐ Download CV button (if off, `cv.*` stays out of the repo)

Paste the generated `/plan` prompt. Pi reads only and proposes.

**What I corrected in the plan before approving:**

------------------------------------------------------------------------

## Act and Test

- ☐ Approved and executed (or continued from the proposed plan)
- ☐ Opened `index.html`; checked every name, title, and date against my CV
- ☐ Narrowed the window to phone width
- ☐ Checked the console (Cmd+Option+J / Ctrl+Shift+J) for errors

**Facts Pi got wrong or embellished, and the fix I asked for:**

------------------------------------------------------------------------

## Document

```text
Create an AGENTS.md that documents this site: its purpose, file structure, design choices (layout, colors, fonts), and that all content must come from cv.txt.
```

- ☐ `AGENTS.md` created (Pi loads it automatically in this folder)

## Make It Yours

One change at a time. Reload and check after each.

1. ______________________
2. ______________________
3. ______________________

- ☐ Asked Pi to check the site for anything I don't want public

## Publish

- ☐ `gh --version` · `gh auth login` · `gh auth status`

```text
Make this folder a git repository with main as the branch name, then create a public GitHub repository called cv-site for it with the gh CLI and connect the two.
```

```text
List the files that will be published, then commit them and push to GitHub. If git doesn't know my name and email yet, set them from my GitHub account, using my GitHub noreply email.
```

- ☐ The published list has no `cv.pdf` or `cv.txt` (unless I chose the download button)
- ☐ Settings → Pages → Deploy from a branch → main → / (root) → Save

**My site:** https://______________________.github.io/cv-site

## Next

- Vibe Coding III: Bring Your Own Project Clinic, Tuesday, October 13, 2:30–4:00 p.m.
- Coworking sessions: October 29, November 17, December 3, 2:00–4:00 p.m.
- Mind your quota. [Register](https://cail-workshop-registration.ailab-452.workers.dev/) · [events](https://ailab.gc.cuny.edu/events/)
- [pi.dev](https://pi.dev) · [cail-pi](https://github.com/CUNY-AI-Lab/cail-pi) · [cli.github.com](https://cli.github.com) · [agents.md](https://agents.md)
