# Configuring Skills and Tools (Fall 2026) - Workshop Archive Entry

## Workshop Overview

**Title:** Configuring Skills and Tools
**Series:** Sandbox Workshop Series, Session 3 of 3
**Date:** Thursday, October 15, 2026, 2:30–4:00 p.m. Eastern
**Location:** New Media Lab, Room 7388.01, CUNY Graduate Center
**Duration:** 90 minutes
**Format:** Hands-on workshop
**Facilitators:** Zach Muhlbauer and Meha Gupta (CUNY AI Lab)

## Workshop Categories

- Educational Technology
- AI Pedagogy
- Developer Tools

## Description

Participants continue the custom model they built across the series, or clone STEM Adventure Games, and extend it with a skill (Adventure Panel Play, which supplies a repeatable procedure applied on every turn) and a tool (Adventure Panel, which renders each scene as an interactive panel and sends the selected choice to chat). They configure the model card for tool calling, add a one-sentence clause to the system prompt, and test by opening call details to confirm the skill loaded and the show_scene function ran. In the second half, participants copy a tool's code or a skill's instructions, work with the CAIL Workspace Support model to revise it or create their own, add the new version to the model card, and retest with identical inputs. The session closes with reflection across the series and an invitation to a coworking session. It revises the Spring 2026 workshop Customizing Skills & Tools.

## Materials

All materials are licensed under a **Creative Commons Attribution-ShareAlike (CC-BY-SA) 4.0 International Public License**.

This archive contains the workshop plan, slide copy, and companion worksheet.

Materials: [Live Slides](https://cuny-ai-lab.github.io/sandbox-series/skills/) | [Slides PDF](https://cuny-ai-lab.github.io/sandbox-series/skills/Tools-and-Skills-Slides.pdf) | [Participant exercises](https://cuny-ai-lab.github.io/sandbox-series/skills/exercises.html) | [Facilitator notes](https://cuny-ai-lab.github.io/sandbox-series/skills/facilitator.html) | [GitHub Repository](https://github.com/CUNY-AI-Lab/sandbox-series)

## Learning Objectives

- Define skills (trigger, procedure, output) and tools (input, execution, result) and explain tool calling
- Configure a model card for tool calling: base model, filter, skill, tool, and a prompt clause that names them
- Verify from call details that a saved skill loaded and a tool function ran
- Revise or create a skill or tool with CAIL Workspace Support while preserving the original
- Add a new version to the model card and compare behavior with identical inputs

## Workshop Agenda

### Open Your Model (2:30–2:40, slides 1–5)

Continue or clone; read the actual system prompt's setting, goals, and rules; define skills and tools; set a base model that supports tool calling.

### Add Your Skill (2:40–2:50, slides 6–7)

Enable Model Bound Tool Enabler; select Adventure Panel Play and read its saved instructions.

### Add Adventure Panel (2:50–3:00, slides 8–10)

Select the Adventure Panel tool; model card check-in; add the prompt clause; Save & Update.

### Test Your Adventure (3:00–3:15, slides 11–12)

Run the game, inspect the view_skill and show_scene call details, play, try a choice before and after its prerequisite, and ask to stop.

### Explore Other Skills (3:15–3:25, slide 13)

Swap in Adventure Outcomes or Conclude Adventure Game; change one thing; compare the same scene.

### Choose Your Task and Work With Support (3:25–3:45, slides 14–16)

Copy complete content; revise one item or create your own with CAIL Workspace Support; adapt toward a lesson outcome; review before saving.

### Add New Version and Reflect (3:45–4:00, slides 17–18)

Create the tool or skill, select it on the model card, retest with identical inputs, record results, and reflect across the series. Coworking sessions follow.

---

## Resources

- [STEM Adventure Games](https://chat.ailab.gc.cuny.edu/?model=stem-adventure-games) and [CAIL Workspace Support](https://chat.ailab.gc.cuny.edu/?model=cail-workspace-support)
- [Sandbox Tools & Skills documentation](https://ailab.gc.cuny.edu/sandbox-docs/tools-skills/) and [Open WebUI Skills](https://docs.openwebui.com/features/workspace/skills/)
- [Hosted evidence](https://cuny-ai-lab.github.io/sandbox-series/skills/hosted-evidence.html) and [tool calling explainer](https://cuny-ai-lab.github.io/sandbox-series/skills/tool-calling.html)
- Previous sessions: [Composing System Prompts](../composing-system-prompts/) and [Curating Knowledge Collections](../curating-knowledge-collections/)
