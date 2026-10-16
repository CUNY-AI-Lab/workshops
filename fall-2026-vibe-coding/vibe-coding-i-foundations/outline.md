# Vibe Coding I: Foundations (Fall 2026) - Workshop Outline

## Workshop Information

**Title:** Vibe Coding I: Foundations
**Date:** Tuesday, September 22, 2026, 2:30–4:00 p.m.
**Location:** New Media Lab, Room 7388.01, CUNY Graduate Center
**Duration:** 90 minutes
**Format:** Hands-on workshop (Session I of the Vibe Coding Series)
**Facilitators:** Stefano Morello and Stephen Zweibel (CUNY AI Lab)

**Learning Objectives:**
- Define vibe coding, explain how a model generates code, and describe the agent loop
- Explain context and its limits
- Open a terminal and use the five navigation commands
- Distinguish Git from GitHub and log into GitHub with the GitHub CLI
- Create a CUNY AI Lab API key, install Pi, connect it, and run the health check

## Preparation

- Participants need a laptop they can install software on, a GitHub account, and CUNY AI Lab access to create an API key.
- On macOS everything goes through Homebrew (`brew install node`, `brew install gh`); the Homebrew installer also brings the developer tools, so Git is present. On Windows use `winget install OpenJS.NodeJS.LTS`, `winget install Git.Git`, and `winget install GitHub.cli`. Avoid the nodejs.org installer on macOS: it puts npm's global prefix in a root-owned folder and leads people to `sudo`.
- Recovery for anyone who used `sudo`: `sudo chown -R $(whoami) ~/.npm ~/.pi`, then `brew install node`, then `npm install -g @earendil-works/pi-coding-agent`.
- Test the Pi setup flow (`npx @cuny-ai-lab/cail-pi`, `npx.cmd` on Windows) on a clean machine before the session.

## Detailed Agenda

### Part 1: Concepts & Context (30 min)

**Icebreaker (10 min).** Where does coding live in your imagination? Pick one and talk to a neighbor: what would you make if coding were as familiar as writing? Or share a challenge you often face in your research, technical or otherwise.

**Vibe Coding in Action.** Live walkthrough: a conversation with Pi turns a plain-language idea into working code, step by step, in the terminal.

**What Is Vibe Coding?** A way of making software by describing what you want in natural language and iterating on what the system produces. The human expresses an intention rather than writing every instruction as code; the system generates or modifies software; the process is conversational and iterative; the practice spans many models and applications.

**How Does a Language Model Generate Code?** The same way it generates prose: one token at a time, using patterns from training and the current context. Prompt and context → tokens → next-token probabilities → generated code. Generating code and executing it are separate: a model by itself cannot open files, run commands, or test what it writes.

**What Makes It a Coding Agent?** A coding agent combines a language model with context, tools, and a feedback loop: the human states the goal; the model uses the available context to choose an action; tools read or edit files and run commands; the environment returns output or an error. The agent is the whole system.

**What Is Context?** The information available to the model when it makes its next prediction: your request (goal, constraints, examples), the conversation, the project (files and instructions the agent has read), and tool results (command output, errors, tests). Context is finite and constructed; the agent does not automatically know everything in the project or on the computer.

### Part 2: Development Environment (25 min)

**Inspecting Your Code.** No extra software needed. macOS: browse in Finder, press Space to peek, open with TextEdit (turn on "Display HTML files as HTML code" in its settings), double-click `index.html` to see it run. Windows: File Explorer with file name extensions shown, open with Notepad, double-click `index.html`.

**Leveling Up.** As projects grow you will want an IDE (highlighting, error checking, a built-in terminal, Git, AI assistants). Options: Visual Studio Code, Zed, Cursor or Windsurf, JetBrains IDEs. Not needed today.

**What Is the Command Line?** A text-based interface for controlling your computer; more powerful and precise, essential for development work, and how AI coding agents interact with your system. Open Terminal (Cmd+Space, "Terminal") or PowerShell (Windows key, "PowerShell").

**Command Line Basics.** `pwd` (print your location), `ls` (list the folder), `mkdir my-project` (make a folder), `cd my-project` (move into it), `cd ..` (go up one level).

**What Is Git? What Is GitHub?** Git is a version control system on your computer that tracks every change so you can go back, undo, and work in parallel. GitHub stores Git repositories online to share, collaborate, and host websites.

**Installing the GitHub CLI.** macOS: install Homebrew from brew.sh and run the "Next steps" commands it prints, then `brew install gh`. Windows: `winget install GitHub.cli`, then open a new PowerShell window. Check with `gh --version`.

**Logging into GitHub.** `gh auth login` → GitHub.com → HTTPS → Login with a web browser → copy the one-time code, press Enter, approve in the browser → "Logged in as your-username".

### Part 3: Installation & Setup (35 min)

**Your CUNY AI Lab API Key & Quota.** The CUNY AI Lab Gateway connects Pi to the models available through the Lab; your personal key identifies your account and applies your quota. Create a key in the CUNY AI Lab Dashboard and copy it when it appears (it cannot be revealed again). Paste it only into Pi's hidden prompt; never into chat, GitHub, screenshots, or email. All your keys share one allowance; check usage in the Dashboard.

**Installing Pi.** Windows: `winget install OpenJS.NodeJS.LTS` and `winget install Git.Git`, open a new window, check `node --version` and `git --version`, then `npx.cmd @cuny-ai-lab/cail-pi`. macOS: Homebrew if needed, `brew install node`, new window, check versions, then `npx @cuny-ai-lab/cail-pi`. Permission error? Don't use `sudo`; raise your hand.

**Connect Pi to CUNY AI Lab.** When LazyPi asks, choose Install everything (warnings and a note about `/login` are normal). At `CUNY AI Lab API key:` paste your key. Make a folder for today (`pwd`, `mkdir workshop-demo`, `cd workshop-demo`). Start Pi with `pi` (`pi.cmd` on Windows). Type `/model` and choose a CUNY AI Lab model. Something off? Run `npx @cuny-ai-lab/cail-pi --doctor`.

**Troubleshooting.** Terminal, GitHub CLI, Git, Pi: fix anything that didn't work together. Raise a hand; help a neighbor; no issue too small.

**Upcoming Workshops.** Vibe Coding II: Building a Prototype (Tuesday, September 29, 2:30–4:00 p.m.); Vibe Coding III: Bring Your Own Project Clinic (Tuesday, October 13); coworking sessions (October 29, November 17, December 3, 2:00–4:00 p.m.). Register, experiment with Pi in the meantime, and mind your quota.

**Links & References.** ailab.gc.cuny.edu, its events and resources pages, the CAIL Sandbox and Tools, the New Media Lab, the GC AI Toolkit, the Lab's GitHub, the Vibe Coding II deck, pi.dev, cail-pi, and the GitHub docs.

## Materials Needed

- Projection and a presenter machine with Pi installed and a Lab key
- Participant laptops with permission to install software
- GitHub accounts and CUNY AI Lab access for API keys
- The Pi recovery commands, ready to paste
