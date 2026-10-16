# Vibe Coding I: Foundations (Fall 2026)

**Companion Checklist**

*Work through this sheet during Session I. Every command is on the slides with a copy button; this sheet is the version you keep.*

## Concepts in One Line Each

| Term | What it means |
|------|---------------|
| **Vibe coding** | Making software by describing what you want in natural language and iterating on what the system produces |
| **Language model** | Generates code one token at a time from patterns and context; it cannot open files or run commands by itself |
| **Coding agent** | A model plus context, tools, and a feedback loop: goal → model chooses an action → tools act → environment reports back |
| **Context** | Your request, the conversation, the files and instructions the agent has read, and tool results; finite and constructed |

**Icebreaker.** What would you make if coding were as familiar as writing? Or what challenge do you face in your research?

------------------------------------------------------------------------

## Part 2: Development Environment

- ☐ Opened my terminal (Terminal on macOS; PowerShell on Windows)
- ☐ Ran `pwd`, `ls`, `mkdir my-project`, `cd my-project`, `cd ..`
- ☐ Installed the GitHub CLI (`brew install gh` or `winget install GitHub.cli`) and checked `gh --version`
- ☐ Logged in with `gh auth login` (GitHub.com → HTTPS → browser) and saw "Logged in as ______________________"

## Part 3: Installation & Setup

### API key

- ☐ Created a personal key in the CUNY AI Lab Dashboard and copied it immediately
- ☐ Pasted it only into Pi's hidden prompt (never chat, GitHub, screenshots, or email)
- ☐ Know where to check my usage; all my keys share one allowance

### Install Pi

| macOS (Terminal) | Windows (PowerShell) |
|------------------|----------------------|
| Install Homebrew from brew.sh, run its "Next steps" commands | `winget install OpenJS.NodeJS.LTS` |
| `brew install node` | `winget install Git.Git` |
| New window; `node --version`, `git --version` | New window; `node --version`, `git --version` |
| `npx @cuny-ai-lab/cail-pi` | `npx.cmd @cuny-ai-lab/cail-pi` |

Never use `sudo`. If you did: `sudo chown -R $(whoami) ~/.npm ~/.pi`, then `brew install node`, then `npm install -g @earendil-works/pi-coding-agent`.

### Connect and run

- ☐ Chose **Install everything** and waited for the key prompt
- ☐ Pasted my key at `CUNY AI Lab API key:`
- ☐ `mkdir workshop-demo`, `cd workshop-demo`, `pi` (`pi.cmd` on Windows)
- ☐ `/model` → chose a CUNY AI Lab model: ______________________
- ☐ Health check if anything is off: `npx @cuny-ai-lab/cail-pi --doctor`

**First thing I asked Pi to build, and what happened:**

------------------------------------------------------------------------

## Before Session II

- Experiment with Pi on your own, and mind your quota
- Bring your CV as a PDF or Word file (Session II turns it into a website)
- Register: [cail-workshop-registration.ailab-452.workers.dev](https://cail-workshop-registration.ailab-452.workers.dev/)

## Links

- [pi.dev](https://pi.dev) · [CUNY AI Lab × Pi](https://github.com/CUNY-AI-Lab/cail-pi) · [API keys guide](https://ailab.gc.cuny.edu/docs/api-keys/)
- [ailab.gc.cuny.edu/events](https://ailab.gc.cuny.edu/events/) · [chat.ailab.gc.cuny.edu](https://chat.ailab.gc.cuny.edu) · [tools.ailab.gc.cuny.edu](https://tools.ailab.gc.cuny.edu)
- [Vibe Coding II deck](https://cuny-ai-lab.github.io/fall-2026-vibe-coding-ii/) · [docs.github.com](https://docs.github.com)
