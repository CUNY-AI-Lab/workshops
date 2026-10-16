# Co-Developing with Generative AI - Workshop Outline

## Workshop Information

**Title:** Co-Developing with Generative AI: Introduction to Command Line Agents
**Date:** Tuesday, November 18, 2025
**Location:** New Media Lab, CUNY Graduate Center
**Format:** Hands-on workshop with a 15–20 minute build
**Facilitators:** Stephen Zweibel, Stefano Morello, and Zach Muhlbauer (CUNY AI Lab)

**Learning Objectives:**
- Explain how language models generate code and name their limitations
- Use basic terminal commands
- Install and authenticate Gemini CLI
- Weigh the critical questions and identify when not to use AI
- Plan in a README, build a scoped prototype, and assess it

## Detailed Agenda

### Today's Tools and Before We Start

Site Studio, Terminal/PowerShell, Gemini CLI. Using lab computers? Sign in now. Brought your own? Make sure you can open a terminal. Tools are installed as we go.

### Ice Breaker: Site Studio

Open Site Studio (powered by Claude Sonnet 4.5 at the time). After the opening demo, share ideas for follow-up prompts.

### Understanding Large Language Models

**How do LLMs work for coding?** Trained on billions of lines of code from open-source projects, documentation, and Stack Overflow; they predict what code should come next from patterns; they can complete functions, suggest implementations, explain code, and debug. Command-line agents such as Gemini CLI can execute commands, read and write files, and iterate, unlike chat interfaces.

**Limitations.** Plausible but broken code; outdated libraries or syntax; security vulnerabilities (SQL injection, XSS); limited context so it cannot see the whole codebase; you must verify and test.

**Prompt engineering basics.** Be specific ("Create a Python function that sorts a list of dictionaries by the 'date' key" rather than "Help me sort some data"); provide context (code, error messages, structure); iterate.

### Command Line Basics

A terminal is a text-based interface for controlling your computer: more powerful and precise, essential for development, and how agents interact with your system. Open Terminal (Cmd+Space) or PowerShell (Windows key). Commands: `ls`, `mkdir <name>`, `cd <name>`, `pwd`, `cd ..`.

### Installing Gemini CLI

Windows: install Node.js from nodejs.org, then `npm install -g @google/gemini-cli`. macOS: install Homebrew, then `brew install gemini-cli`. Run `gemini`, choose Login with Google, follow the browser prompt. Free tier at the time: 60 requests a minute, 1,000 a day.

### Critical Questions

**Ethical challenges.** Academic integrity (how to cite AI-assisted work; collaboration versus skills offloading); bias and fairness; environmental impact.

**Power and labor.** Who builds these systems (underpaid data labelers and moderators); who controls AI; privacy (what data you share and how it is used).

**Why use AI coding tools, then?** Speeds repetitive tasks; helps learn new languages by example; debugging and explanation; documentation; prototyping; less context switching; access for people without CS backgrounds.

**When not to use AI.** Learning fundamentals for the first time; sensitive or confidential data; guaranteed-accuracy contexts; when the goal is your own problem solving; when it would violate policy. Use AI as a tool, not a replacement for understanding.

### Choose Your Project Track

- **Website:** portfolio, link tree, small HTML/CSS/JS pages
- **Visualization:** a simple map, chart, or interactive element
- **Program/Script:** a basic Python task (text parsing, data cleanup, a small utility)

### Start with a README

Ask the agent to create a README.md first: describe the project idea, outline the structure, list key features or goals. Approve the workflow before building.

### Hands-On Activity (15–20 min)

After approving the README, work with the agent to implement its plan. Facilitators walk the room.

### Let's Reflect

**Your experience.** What worked well? What didn't? Surprises? Trust and verification: how did you know the generated code was correct?

**Critical assessment.** When is AI-assisted coding appropriate for your work? When inappropriate? How would you document or cite AI use? What skills do you still need to develop yourself?

### Resources

Claude Code; Google AI for Students; GitHub Copilot; GitHub Desktop.

## Materials Needed

- Lab computers or participant laptops with permission to install Node.js or Homebrew
- Google accounts for Gemini CLI login
- Projection for the Site Studio demo
