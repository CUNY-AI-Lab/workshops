# Vibe Coding II: Building a Prototype (Fall 2026)

_Session II of the CUNY AI Lab Vibe Coding Series: plan, build, test, document, and publish a personal website with Pi._

Participants turn their own CV into a professional website and publish it on GitHub Pages in one session. Pi reads the CV, proposes a plan without touching files, builds plain HTML, CSS, and JavaScript from an interactive prompt builder, documents the project in `AGENTS.md`, then creates the repository, commits, and pushes, with the participant reading what it runs at every step.

**Workshop Date:** Tuesday, September 29, 2026
**Time:** 2:30–4:00 p.m. (90 minutes)
**Location:** New Media Lab, Room 7388.01, CUNY Graduate Center
**Format:** Hands-on workshop (Session II of the Vibe Coding Series)
**Facilitators:** Stefano Morello and Stephen Zweibel (CUNY AI Lab)
**Prerequisite:** Vibe Coding I, or familiarity with the command line and Git/GitHub

_This session was originally conducted as part of the [Vibe Coding Series](../) at the CUNY Graduate Center. It revises the Spring 2026 workshop [Vibe-Coding Prototypes](../../vibe-coding-prototypes/)._

## About the CUNY AI Lab

The **CUNY AI Lab** is a faculty and staff-led incubator for experimentation with AI by CUNY researchers across disciplines, strengthening CUNY's position at the leading edge of technological innovation. Located at the CUNY Graduate Center and led by experienced scholars and technologists who have built widely used open publishing platforms, the Lab fosters momentum for AI experimentation while foregrounding ethical practices and values that reinforce CUNY's mission of accessible, equitable, and transformative education.

This workshop is part of the CUNY AI Lab's commitment to developing critical AI literacy among faculty, staff, and students across the university system.

## Overview

After a one-slide review of Session I, participants set up (API key, Node.js and Git, Pi), then move through a plan-act-test-document cycle. A prompt builder on the slide lets each person choose layout, style, colors, fonts, light or dark mode, and sections, and emits a one-line `/plan` prompt that tells Pi to use only facts from the CV, build plain HTML/CSS/JS that works on GitHub Pages, and make it responsive and accessible. Pi reads first and proposes; the participant corrects wrong facts before approving; Pi builds; the participant opens the site, checks every fact, narrows the window, and reads the console. An `AGENTS.md` file records the site's purpose, structure, and design rules so later sessions keep them. Publishing goes through the GitHub CLI and GitHub Pages, with a check that the CV file itself stays out of the repository unless a download button was chosen.

## Learning Objectives

- Use `/plan` to have an agent read a project and propose changes before it edits anything
- Build a small website from a structured prompt and verify its facts, responsiveness, and console
- Write an `AGENTS.md` that an agent loads automatically in later sessions
- Ask the agent to create a repository, commit, and push, and read what it runs
- Publish with GitHub Pages while keeping private files out of the repository

## Workshop Structure

### Part 0: Review (5 min)
1. **Foundations Review** - Vibe coding, the agent loop, context, and the navigation commands

### Part 1: Setup (25 min)
2. **Your CUNY AI Lab API Key & Quota**
3. **Install Node.js & Git** - Homebrew on macOS; winget on Windows; a fix for anyone who used `sudo` last time
4. **Install and Launch Pi** - `npx @cuny-ai-lab/cail-pi`, Install everything, paste the key, `pi`, `/model`

### Part 2: Plan + Act (35 min)
5. **Set Up Your Project** - `mkdir cv-site`, `cd cv-site`, `pi`; have Pi find the CV and save its text as `cv.txt`
6. **Design Your Site** - Interactive prompt builder: layout, style, colors, fonts, mode, sections, privacy options
7. **Planning Stage** - Paste the prompt; `/plan` reads only; answer questions; correct the plan
8. **Acting Stage** - Approve and execute, or continue from the proposed plan
9. **Open and Test Your Site** - Check every fact, phone width, and the console
10. **Create `AGENTS.md`** - Purpose, file structure, design choices, and the rule that content comes from `cv.txt`

### Part 3: Prototype + Publish (25 min)
11. **Make It Yours** - One change at a time; fix anything untrue; check for anything you don't want public
12. **Install and Authenticate GitHub CLI**
13. **Create Remote Repository** - Pi runs `git init` and `gh repo create`
14. **Push to GitHub** - Pi lists files, commits, and pushes; confirm `cv.pdf` and `cv.txt` are not listed
15. **Enable GitHub Pages** - Settings → Pages → Deploy from a branch → main → / (root)
16. **Links & References** - The clinic, coworking sessions, registration, and docs

## Interactive Tools

- **[Pi](https://pi.dev)** and **[CUNY AI Lab × Pi](https://github.com/CUNY-AI-Lab/cail-pi)**
- **[GitHub CLI](https://cli.github.com)** and **[GitHub Pages](https://docs.github.com)**
- **[AGENTS.md specification](https://agents.md)**
- **Prompt builder** (`src/cv-builder.js` in the deck) - Generates the `/plan` prompt from the participant's choices

## Technical Details

### Slide Deck

- **[Live Slides](https://cuny-ai-lab.github.io/fall-2026-vibe-coding-ii/)** - 22 slides
- **[GitHub Repository](https://github.com/CUNY-AI-Lab/fall-2026-vibe-coding-ii)** - Source code and materials

### Related Sessions

- **[Vibe Coding I: Foundations](../vibe-coding-i-foundations/)** - September 22, 2026 (prerequisite)
- **Vibe Coding III: Bring Your Own Project Clinic** - October 13, 2026
- **[Vibe-Coding Prototypes](../../vibe-coding-prototypes/)** - The Spring 2026 version of this session

## License

All materials are licensed under a **Creative Commons Attribution-ShareAlike (CC-BY-SA) 4.0 International Public License** unless otherwise noted.
