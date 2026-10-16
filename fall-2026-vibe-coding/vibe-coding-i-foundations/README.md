# Vibe Coding I: Foundations (Fall 2026)

_Session I of the CUNY AI Lab Vibe Coding Series: concepts, a working development environment, and Pi connected to the Lab's models._

Participants leave with a conceptual grounding in how a language model generates code and what turns it into a coding agent, a terminal they can navigate, the GitHub CLI logged in, and Pi installed and connected to CUNY AI Lab models with their own API key. The session opens with a live walkthrough of Pi building something from a plain-language idea and closes with group troubleshooting.

**Workshop Date:** Tuesday, September 22, 2026
**Time:** 2:30–4:00 p.m. (90 minutes)
**Location:** New Media Lab, Room 7388.01, CUNY Graduate Center
**Format:** Hands-on workshop (Session I of the Vibe Coding Series)
**Facilitators:** Stefano Morello and Stephen Zweibel (CUNY AI Lab)

_This session was originally conducted as part of the [Vibe Coding Series](../) at the CUNY Graduate Center. It revises the Spring 2026 workshop [Foundations: Coding with Generative AI](../../gen-dev-foundations/)._

## About the CUNY AI Lab

The **CUNY AI Lab** is a faculty and staff-led incubator for experimentation with AI by CUNY researchers across disciplines, strengthening CUNY's position at the leading edge of technological innovation. Located at the CUNY Graduate Center and led by experienced scholars and technologists who have built widely used open publishing platforms, the Lab fosters momentum for AI experimentation while foregrounding ethical practices and values that reinforce CUNY's mission of accessible, equitable, and transformative education.

This workshop is part of the CUNY AI Lab's commitment to developing critical AI literacy among faculty, staff, and students across the university system.

## Overview

Three parts. **Concepts and context** defines vibe coding (making software by describing what you want and iterating on what the system produces), explains that a model generates code one token at a time and cannot by itself open files or run commands, and shows what makes a coding agent: a model working with context, tools, and a feedback loop. Context is finite and constructed. **Development environment** uses the apps already on the computer to inspect code, opens the terminal, teaches five navigation commands with animated command cards, distinguishes Git from GitHub, and installs and logs into the GitHub CLI. **Installation and setup** creates a CUNY AI Lab API key, explains the quota, installs Node.js and Git through Homebrew or winget, runs the Lab's Pi installer, connects Pi with the key, and chooses a model.

## Learning Objectives

- Define vibe coding, explain how a language model generates code, and describe the agent loop (goal, model, tools, environment)
- Explain what context is and why an agent does not automatically know everything on the computer
- Open a terminal and use `pwd`, `ls`, `mkdir`, `cd`, and `cd ..`
- Distinguish Git from GitHub and log into GitHub from the terminal with the GitHub CLI
- Create a personal CUNY AI Lab API key, keep it private, install Pi, connect it to Lab models, and run a health check

## Workshop Structure

### Part 1: Concepts & Context (30 min)
1. **Icebreaker** - Where does coding live in your imagination? What would you make if coding were as familiar as writing, or what challenge do you face in your research?
2. **Vibe Coding in Action** - Live walkthrough with Pi in the terminal
3. **What Is Vibe Coding?** - Intention expressed in natural language; conversational and iterative
4. **How Does a Language Model Generate Code?** - Prompt and context → tokens → next-token probabilities → generated code; generating and executing are separate
5. **What Makes It a Coding Agent?** - Human goal, model, tools, environment; the agent is the whole system
6. **What Is Context?** - Your request, the conversation, the project, tool results

### Part 2: Development Environment (25 min)
7. **Inspecting Your Code** - Finder and TextEdit, or File Explorer and Notepad; double-click `index.html` to see it run
8. **Leveling Up: Code Editors & IDEs** - VS Code, Zed, Cursor or Windsurf, JetBrains; not needed today
9. **What Is the Command Line?** and **Opening Your Terminal** - Terminal on macOS, PowerShell on Windows
10. **Command Line Basics** - `pwd`, `ls`, `mkdir my-project`, `cd my-project`, `cd ..`
11. **What Is Git? What Is GitHub?** - Version control locally; repositories, collaboration, and hosting online
12. **Installing and Logging into the GitHub CLI** - Homebrew or winget; `gh auth login`

### Part 3: Installation & Setup (35 min)
13. **Your CUNY AI Lab API Key & Quota** - Create a key in the Dashboard; paste it only into Pi's hidden prompt; all keys share one allowance
14. **Installing Pi** - Node.js and Git, then `npx @cuny-ai-lab/cail-pi`; never use `sudo`
15. **Connect Pi to CUNY AI Lab** - Install everything, paste the key, make a project folder, start `pi`, choose a model with `/model`
16. **Troubleshooting** - Group fix-it time, including the recovery for anyone who used `sudo`
17. **Upcoming Workshops** - Vibe Coding II, the clinic, coworking sessions, registration, and a reminder to mind the quota
18. **Links & References**

## Interactive Tools

- **[Pi](https://pi.dev)** and **[CUNY AI Lab × Pi](https://github.com/CUNY-AI-Lab/cail-pi)**
- **[CUNY AI Lab API keys guide](https://ailab.gc.cuny.edu/docs/api-keys/)**
- **[GitHub CLI](https://cli.github.com)** and **[GitHub docs](https://docs.github.com)**
- **[CAIL Sandbox](https://chat.ailab.gc.cuny.edu)** and **[CAIL Tools](https://tools.ailab.gc.cuny.edu)**

## Technical Details

### Slide Deck

- **[Live Slides](https://cuny-ai-lab.github.io/fall-2026-vibe-coding-i/)** - 24 slides
- **[GitHub Repository](https://github.com/CUNY-AI-Lab/fall-2026-vibe-coding-i)** - Source code and materials

### Related Sessions

- **[Vibe Coding II: Building a Prototype](../vibe-coding-ii-building-a-prototype/)** - September 29, 2026
- **[Foundations: Coding with Generative AI](../../gen-dev-foundations/)** - The Spring 2026 version of this session

## License

All materials are licensed under a **Creative Commons Attribution-ShareAlike (CC-BY-SA) 4.0 International Public License** unless otherwise noted.
