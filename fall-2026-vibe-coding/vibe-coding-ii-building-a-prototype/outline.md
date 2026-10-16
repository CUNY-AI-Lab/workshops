# Vibe Coding II: Building a Prototype (Fall 2026) - Workshop Outline

## Workshop Information

**Title:** Vibe Coding II: Building a Prototype
**Date:** Tuesday, September 29, 2026, 2:30–4:00 p.m.
**Location:** New Media Lab, Room 7388.01, CUNY Graduate Center
**Duration:** 90 minutes
**Format:** Hands-on workshop (Session II of the Vibe Coding Series)
**Facilitators:** Stefano Morello and Stephen Zweibel (CUNY AI Lab)
**Prerequisite:** Vibe Coding I, or familiarity with the command line and Git/GitHub

**Learning Objectives:**
- Use `/plan` so the agent reads and proposes before editing
- Build a small site from a structured prompt and verify it
- Write an `AGENTS.md` the agent loads automatically
- Have the agent create, commit, and push a repository, and read what it runs
- Publish with GitHub Pages while keeping private files out

## Preparation

- Participants bring a CV as a PDF or Word file (a fictional sample is the fallback), a GitHub account, and a CUNY AI Lab API key.
- Pi's installer needs Node.js 22.19 or newer and Git. Homebrew on macOS; winget on Windows. Never the nodejs.org installer on macOS.
- Anyone who used `sudo` last time: `sudo chown -R $(whoami) ~/.npm ~/.pi`, `brew install node`, `npm install -g @earendil-works/pi-coding-agent`.
- Planning uses `/plan` from LazyPi's pi-plan package; Pi auto-loads `AGENTS.md`.

## Detailed Agenda

### Part 0: Review (5 min)

Foundations review in Session I's terms: what is vibe coding; what makes it a coding agent; what is context; which commands move you around (`pwd`, `ls`, `cd`, `cd ..`) and what Git does.

### Part 1: Setup (25 min)

**Your CUNY AI Lab API Key & Quota.** Create a personal key in the Dashboard; copy it when it appears; paste it only into Pi's hidden prompt; all keys share one allowance.

**Install Node.js & Git.** macOS: Homebrew if needed, `brew install node`, new Terminal window, `node --version` and `git --version`. Windows: `winget install OpenJS.NodeJS.LTS`, `winget install Git.Git`, new PowerShell window, check versions.

**Install and Launch Pi.** `npx @cuny-ai-lab/cail-pi` (`npx.cmd` on Windows); choose Install everything; paste the key; start with `pi` (`pi.cmd`); `/model` and choose a CUNY AI Lab model. Never use `sudo`; run `--doctor` or ask.

### Part 2: Plan + Act (35 min)

**Set Up Your Project.** From your projects folder: `mkdir cv-site`, `cd cv-site`, `pi`. Ask Pi to find the CV (probably in Downloads), copy it into the folder as `cv.pdf` or `cv.docx`, and save its text as `cv.txt` (for a PDF: `npx --yes pdf-parse text cv.pdf -o cv.txt`). Check that `cv.txt` looks like your CV. No CV handy? Ask Pi to write a sample one for a fictional researcher.

**Design Your Site.** Pick options in the prompt builder:
- Layout: single scrolling page, sidebar profile, minimal business card, several pages
- Style: clean and minimal, academic and classic, bold and modern, warm and approachable, creative and playful
- Colors: ink and paper, navy and gold, forest and cream, terracotta and sand, ocean and teal, plum and blush, or let Pi choose
- Fonts: serif headings with sans body, all sans, all serif, sans with monospace accents
- Light or dark: follow system with a toggle, light, dark
- Sections: About, Education, Experience, Publications, Contact on by default; Research, Teaching, Projects, Skills, Awards optional
- Hide phone number and home address (on); add a "Download CV" button (off; when off, the prompt tells Pi to keep `cv.*` out of the repo with `.gitignore`)

The output is a one-line prompt starting with `/plan` that tells Pi to use only facts from `cv.txt`, build plain HTML/CSS/JS that works on GitHub Pages, and make it responsive and accessible.

**Planning Stage.** Paste the prompt. Because it starts with `/plan`, Pi only reads: it studies `cv.txt` and proposes a plan without changing files. Answer its questions. Wrong facts or a missing section? Tell Pi before you approve.

**Acting Stage.** Choose Approve and execute now, or Continue from proposed plan to adjust it. One possible result: `index.html`, `css/style.css`, `js/main.js`, `.gitignore`, `cv.pdf`, `cv.txt`.

**Open and Test Your Site.** Ask Pi to open `index.html`. Check every fact against your CV: names, titles, dates. Narrow the window to phone size. Check the console (Cmd+Option+J or Ctrl+Shift+J). Tell Pi exactly what to fix.

**Create `AGENTS.md`.** "Create an AGENTS.md that documents this site: its purpose, file structure, design choices (layout, colors, fonts), and that all content must come from cv.txt." Pi loads it automatically whenever you start it in this folder.

### Part 3: Prototype + Publish (25 min)

**Make It Yours.** One change at a time (a photo, a Projects section, profile links); reload and check after each; fix anything untrue; before publishing, ask Pi to check for anything you don't want public; keep it simple enough to publish today.

**Install and Authenticate GitHub CLI.** `brew install gh` or `winget install GitHub.cli`; `gh --version`; `gh auth login` → GitHub.com → HTTPS → browser; `gh auth status`.

**Create Remote Repository.** "Make this folder a git repository with main as the branch name, then create a public GitHub repository called cv-site for it with the gh CLI and connect the two." Watch Pi run `git init` and `gh repo create`.

**Push to GitHub.** "List the files that will be published, then commit them and push to GitHub. If git doesn't know my name and email yet, set them from my GitHub account, using my GitHub noreply email." Check the list: no `cv.pdf` or `cv.txt` unless you chose the download button. Ask Pi for the link.

**Enable GitHub Pages.** github.com/USERNAME/cv-site → Settings → Pages → Source: Deploy from a branch → main, / (root) → Save → visit USERNAME.github.io/cv-site.

**Links & References.** Vibe Coding III: Bring Your Own Project Clinic (Tuesday, October 13, 2:30–4:00 p.m.); coworking sessions (October 29, November 17, December 3, 2:00–4:00 p.m.); mind your quota; register; CAIL sites; pi.dev, cail-pi, cli.github.com, docs.github.com, agents.md.

## Materials Needed

- Projection and a presenter machine with Pi and a sample CV
- Participant laptops with Node.js, Git, Pi, and a Lab key from Session I
- GitHub accounts
- The copyable prompts (CV import, repository creation, push) ready to paste
