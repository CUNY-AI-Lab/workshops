# Configuring Skills and Tools (Fall 2026)

_Session 3 of the CUNY AI Lab Sandbox Workshop Series: extend model capabilities with skills and tools._

Participants continue the custom model they built in the first two sessions (or clone STEM Adventure Games fresh), add a skill that supplies a repeatable procedure and a tool that renders each scene as an interactive panel, and test whether the model actually loads the skill and calls the tool. In the second half they copy a tool's code or a skill's instructions, work with the CAIL Workspace Support model to revise it or create their own, add the new version to their model card, and retest with the same inputs.

**Workshop Date:** Thursday, October 15, 2026
**Time:** 2:30–4:00 p.m. Eastern (90 minutes)
**Location:** New Media Lab, Room 7388.01, CUNY Graduate Center
**Format:** Hands-on workshop (Session 3 of 3)
**Facilitators:** Zach Muhlbauer and Meha Gupta (CUNY AI Lab)
**Required access:** Session 1 access, Skills and Tools access, and Workspace authoring permissions for creation and editing; Knowledge access when a procedure retrieves from a collection

_This session was originally conducted as part of the [Sandbox Workshop Series](../) at the CUNY Graduate Center. It revises the Spring 2026 workshop [Customizing Skills & Tools](../../skills-tools/). A follow-up coworking session on October 29, 2026 invited participants to build their adventures into a collection._

## About the CUNY AI Lab

The **CUNY AI Lab** is a faculty and staff-led incubator for experimentation with AI by CUNY researchers across disciplines, strengthening CUNY's position at the leading edge of technological innovation. Located at the CUNY Graduate Center and led by experienced scholars and technologists who have built widely used open publishing platforms, the Lab fosters momentum for AI experimentation while foregrounding ethical practices and values that reinforce CUNY's mission of accessible, equitable, and transformative education.

This workshop is part of the CUNY AI Lab's commitment to developing critical AI literacy among faculty, staff, and students across the university system.

## Overview

A **skill** contains plain-text instructions for a repeatable task: a trigger, a procedure, and the required output. A **tool** gives the model the ability to execute a function and return its result, usually through a Python script; this is tool calling, also called function calling. Both are attached on the model card, and the adventure's setting, goals, and rules still come from each participant's system prompt. The session walks through the full configuration (base model that supports tool calling, a filter that binds attached tools to the model, the Adventure Panel Play skill, the Adventure Panel tool, and a one-sentence clause at the bottom of the system prompt) and then insists on evidence: open the call details and confirm the skill loaded and the show_scene function ran before judging the game. Skill and tool explanation, addition, and testing precede the open-ended Support activity, where participants revise either resource or create their own.

## Learning Objectives

- Define skills (trigger, procedure, output) and tools (input, execution, result) and explain tool calling
- Configure a model card for tool calling: base model, Model Bound Tool Enabler filter, selected skill and tool, and a system-prompt clause that names them
- Verify from call details that a saved skill loaded and a tool function ran, rather than trusting the model's claim
- Revise an existing skill or tool, or create a new one, with CAIL Workspace Support while preserving the original
- Add a new version to the model card and compare its behavior against the original using identical inputs

## Workshop Structure

1. **Choose Your Own Adventure** - Continue your saved model or clone STEM Adventure Games; review your system prompt's setting, goals, and rules
2. **What Is a Skill?** - Trigger, procedure, output
3. **What Is a Tool?** - Input, execution, result; tool calling
4. **Update Model for Tool Calling** - Select a base model that supports tool calling (DeepSeek V4 Flash 0731 in the session)
5. **Enable Filter** - Model Bound Tool Enabler
6. **Add Your Skill** - Skills → Select Skill → Adventure Panel Play; read its saved instructions
7. **Add the Adventure Panel Tool** - Tools → Select Tool → Adventure Panel
8. **Model Card Check-In** - Tool, skill, filter selected; knowledge collection still attached
9. **Add Skill Instructions** - One clause at the bottom of the system prompt; Save & Update
10. **Test Your Adventure** - Run it; verify the skill and tool are called; play
11. **Observe Game Results** - Open call details for view_skill and show_scene
12. **Explore Other Skills** - Adventure Outcomes or Conclude Adventure Game; change one thing and compare
13. **Choose Your Task** - Revise one item (copy complete code or instructions) or create your own (purpose, input, expected result)
14. **Work With Support** - CAIL Workspace Support: supply complete content, your prompt, scenario, play record, sources, and the observed problem
15. **Adapt Your Adventure** - Toward a lesson outcome or disciplinary focus
16. **Add Tools or Skills** - Workspace → Tools or Skills → Create; select on the model card; signpost in the prompt; retest
17. **Coworking Sessions** - Continue Sandbox and Vibe Coding projects together

## Interactive Tools

- **[CUNY AI Lab Sandbox](https://chat.ailab.gc.cuny.edu/)** - Workspace → Models, Skills, Tools
- **[STEM Adventure Games](https://chat.ailab.gc.cuny.edu/?model=stem-adventure-games)** - The model participants continue or clone
- **[CAIL Workspace Support](https://chat.ailab.gc.cuny.edu/?model=cail-workspace-support)** - Support model for revising or creating skills and tools
- **Adventure Panel** (tool) and **Adventure Panel Play** (skill) - Shared workshop resources on the Sandbox; the tool displays each scene and sends a selected choice to chat, the skill applies the system prompt's rules on every turn
- **[Sandbox Tools & Skills documentation](https://ailab.gc.cuny.edu/sandbox-docs/tools-skills/)** and **[Open WebUI Skills](https://docs.openwebui.com/features/workspace/skills/)**

## Technical Details

### Slide Deck and Materials

- **[Live Slides](https://cuny-ai-lab.github.io/sandbox-series/skills/)** - Interactive slideshow
- **[Slides PDF](https://cuny-ai-lab.github.io/sandbox-series/skills/Tools-and-Skills-Slides.pdf)**
- **[Participant exercises](https://cuny-ai-lab.github.io/sandbox-series/skills/exercises.html)** - Timed, step-by-step instructions with test tables and Support prompts
- **[Facilitator notes](https://cuny-ai-lab.github.io/sandbox-series/skills/facilitator.html)** - Flow, evidence limits, and access notes
- **[Tool calling explainer](https://cuny-ai-lab.github.io/sandbox-series/skills/tool-calling.html)** and **[catalog](https://cuny-ai-lab.github.io/sandbox-series/skills/catalog.html)**
- **[Hosted evidence](https://cuny-ai-lab.github.io/sandbox-series/skills/hosted-evidence.html)** - What the October 14–15 tests established and what they did not
- **[GitHub Repository](https://github.com/CUNY-AI-Lab/sandbox-series)** - Source code and materials

### Workshop Artifacts

- [STEM Adventure tool](https://cuny-ai-lab.github.io/sandbox-series/examples/tools/stem_adventure.html) and [playable preview](https://cuny-ai-lab.github.io/sandbox-series/examples/adventure/preview.html); the engine checks moves, inventory, and prerequisites, and exported records can be restored by replaying commands
- [Extend STEM Adventures skill](https://cuny-ai-lab.github.io/sandbox-series/examples/stem-game-skill.html) and the [Adventure Outcomes](https://cuny-ai-lab.github.io/sandbox-series/examples/adventure-kit/adventure-outcomes.html) and [Conclude Adventure](https://cuny-ai-lab.github.io/sandbox-series/examples/adventure-kit/conclude-adventure.html) skills
- [Prism Laboratory scenario](https://cuny-ai-lab.github.io/sandbox-series/examples/adventure/prism.html), [aperture variation](https://cuny-ai-lab.github.io/sandbox-series/examples/adventure/aperture.html), and [winning commands](https://cuny-ai-lab.github.io/sandbox-series/examples/adventure/winning-commands.html)
- [Skill Creator](https://cuny-ai-lab.github.io/sandbox-series/examples/creators/skill-creator-system-prompt.html) and [Tool Creator](https://cuny-ai-lab.github.io/sandbox-series/examples/creators/tool-creator-system-prompt.html) system prompts; both accept requirements for any suitable task

### Related Sessions

- **[Composing System Prompts](../composing-system-prompts/)** - Session 1, September 17, 2026
- **[Curating Knowledge Collections](../curating-knowledge-collections/)** - Session 2, October 1, 2026

## Notes from Delivery

The facilitator notes record what the preparation tests established: an explicit native `view_skill` call returned the saved skill's instructions in an October 15 test, and the exported Adventure Kit rendered an interactive player in chat. They also record what was not established (a benchmark of autonomous skill discovery, participant access to shared resources, or the necessity of the filter), and ask facilitators to recheck deployed behavior after any Open WebUI upgrade.

## License

All materials are licensed under a **Creative Commons Attribution-ShareAlike (CC-BY-SA) 4.0 International Public License** unless otherwise noted.
