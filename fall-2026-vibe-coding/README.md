# Vibe Coding Series (Fall 2026)

_A CUNY AI Lab series on building software by describing it: two workshops, a bring-your-own-project clinic, and three drop-in coworking sessions, all in the Graduate Center's New Media Lab._

The Fall 2026 series reworks the Spring 2026 CAIL Spotlight pair ([Foundations](../gen-dev-foundations/) and [Vibe-Coding Prototypes](../vibe-coding-prototypes/)) around **Pi**, an open-source coding agent for the terminal that participants connect to the Lab's own models with a personal CUNY AI Lab API key. Gemini CLI and VS Code are gone; participants inspect what the agent builds with the apps already on their computers, and every model call goes through the CAIL Gateway with the participant's own quota.

**Workshops:** Tuesdays, September 22 and September 29, 2026, 2:30–4:00 p.m.
**Clinic:** Tuesday, October 13, 2026, 2:30–4:00 p.m. (Vibe Coding III: Bring Your Own Project)
**Coworking sessions:** Thursday, October 29; Tuesday, November 17; Thursday, December 3, 2026, 2:00–4:00 p.m. (drop-in)
**Location:** New Media Lab, Room 7388.01, CUNY Graduate Center
**Facilitators:** Stefano Morello and Stephen Zweibel (CUNY AI Lab)

_This series was originally conducted at the CUNY Graduate Center in Fall 2026, alongside the [Sandbox Workshop Series](../sandbox-series/). The coworking sessions are shared by both series._

## About the CUNY AI Lab

The **CUNY AI Lab** is a faculty and staff-led incubator for experimentation with AI by CUNY researchers across disciplines, strengthening CUNY's position at the leading edge of technological innovation. Located at the CUNY Graduate Center and led by experienced scholars and technologists who have built widely used open publishing platforms, the Lab fosters momentum for AI experimentation while foregrounding ethical practices and values that reinforce CUNY's mission of accessible, equitable, and transformative education.

This series is part of the CUNY AI Lab's commitment to developing critical AI literacy among faculty, staff, and students across the university system.

## Sessions

| # | Session | Date | Entry |
|---|---------|------|-------|
| I | **Vibe Coding I: Foundations** | Tuesday, September 22, 2026 | [vibe-coding-i-foundations/](./vibe-coding-i-foundations/) |
| II | **Vibe Coding II: Building a Prototype** | Tuesday, September 29, 2026 | [vibe-coding-ii-building-a-prototype/](./vibe-coding-ii-building-a-prototype/) |
| III | **Vibe Coding III: Bring Your Own Project Clinic** | Tuesday, October 13, 2026 | No deck; prerequisite Vibe Coding I and II or comparable experience |
| | **Coworking Sessions** (in-person drop-in) | October 29, November 17, December 3, 2026 | Continue Sandbox and vibe-coding projects with time to build and troubleshoot together |

## What Changed from Spring 2026

- **Pi replaces Gemini CLI.** One command (`npx @cuny-ai-lab/cail-pi`) installs Pi and connects it to CUNY AI Lab models with the participant's personal key. A `--doctor` health check and a no-`sudo` rule handle the common failure modes.
- **A Lab key and quota replace a Google login.** Participants create a key in the CUNY AI Lab Dashboard; all of a person's keys share one allowance, and the decks tell them to mind it between sessions.
- **Native apps replace VS Code.** Finder and TextEdit, or File Explorer and Notepad, are enough to inspect what the agent builds; an outlook slide names editors to grow into.
- **A CV website replaces the focus timer.** Session II turns a participant's own CV into a published GitHub Pages site, with a prompt builder for layout, style, colors, fonts, and sections, and a `.gitignore` rule that keeps the CV itself out of the repository unless the participant chooses a download button.
- **Git basics are folded in.** Session I keeps navigation commands and GitHub CLI login; the commit-and-push steps are done by the agent in Session II, with the participant reading what it runs.

## Interactive Tools

- **[Pi](https://pi.dev)** - Open-source AI coding agent for the terminal
- **[CUNY AI Lab × Pi](https://github.com/CUNY-AI-Lab/cail-pi)** - Setup, `--doctor` health check, troubleshooting, and uninstall
- **[CUNY AI Lab API keys](https://ailab.gc.cuny.edu/docs/api-keys/)** - Creating a personal key and checking usage
- **[GitHub CLI](https://cli.github.com)** and **[GitHub Pages](https://docs.github.com)**
- **[AGENTS.md](https://agents.md)** - The project-documentation file Pi loads automatically
- **[Workshop registration](https://cail-workshop-registration.ailab-452.workers.dev/)** and **[events](https://ailab.gc.cuny.edu/events/)**

## Technical Details

### Slide Decks

- **[Vibe Coding I: Foundations](https://cuny-ai-lab.github.io/fall-2026-vibe-coding-i/)** · [repository](https://github.com/CUNY-AI-Lab/fall-2026-vibe-coding-i) (forked from [gen-dev-foundations](https://github.com/CUNY-AI-Lab/gen-dev-foundations))
- **[Vibe Coding II: Building a Prototype](https://cuny-ai-lab.github.io/fall-2026-vibe-coding-ii/)** · [repository](https://github.com/CUNY-AI-Lab/fall-2026-vibe-coding-ii) (forked from [vibe-coding-prototypes](https://github.com/CUNY-AI-Lab/vibe-coding-prototypes))

Both decks are single-page HTML with no build step, a copy button on every command line, a QR code to the deck on the title slide, and a generative canvas artifact (an infinite wheel, Chladni figures).

### Related

- **[Co-Developing with Generative AI](../co-developing-with-generative-ai/)** - The first vibe-coding workshop, November 2025
- **[Foundations: Coding with Generative AI](../gen-dev-foundations/)** and **[Vibe-Coding Prototypes](../vibe-coding-prototypes/)** - Spring 2026
- **[Vibe Coding How-To](../vibe-coding-how-to/)** - Operational guide

## License

All materials are licensed under a **Creative Commons Attribution-ShareAlike (CC-BY-SA) 4.0 International Public License** unless otherwise noted.
