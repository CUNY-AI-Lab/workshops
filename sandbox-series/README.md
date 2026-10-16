# Sandbox Workshop Series (Fall 2026)

_A three-session CUNY AI Lab series on configuring the CAIL Sandbox for teaching and research: system prompts, knowledge collections, and skills and tools._

The Fall 2026 series reworks the Spring 2026 three-week sequence ([Composing System Prompts](../system-prompting/), [Curating Knowledge Collections](../knowledge-collections/), [Customizing Skills & Tools](../skills-tools/)) into one shared deck site with a single example that carries across all three sessions. Participants compare models, clone and revise a custom model, build a knowledge collection for it, then extend it with a skill and a tool. Each session also stands on its own.

**Series Dates:** Thursdays, September 17, October 1, and October 15, 2026
**Time:** 2:30–4:00 p.m. Eastern (90 minutes each)
**Location:** New Media Lab, Room 7388.01, CUNY Graduate Center
**Developed by:** Zach Muhlbauer (CUNY AI Lab)
**Facilitators:** Zach Muhlbauer (all sessions) and Meha Gupta (sessions 2 and 3)

_This series was originally conducted at the CUNY Graduate Center in Fall 2026, alongside the [Vibe Coding Series](../fall-2026-vibe-coding/), with shared drop-in coworking sessions on October 29, November 17, and December 3, 2026._

## About the CUNY AI Lab

The **CUNY AI Lab** is a faculty and staff-led incubator for experimentation with AI by CUNY researchers across disciplines, strengthening CUNY's position at the leading edge of technological innovation. Located at the CUNY Graduate Center and led by experienced scholars and technologists who have built widely used open publishing platforms, the Lab fosters momentum for AI experimentation while foregrounding ethical practices and values that reinforce CUNY's mission of accessible, equitable, and transformative education.

This series is part of the CUNY AI Lab's commitment to developing critical AI literacy among faculty, staff, and students across the university system.

## Sessions

| # | Session | Date | Facilitators | Entry |
|---|---------|------|--------------|-------|
| 1 | **Composing System Prompts** | Thursday, September 17, 2026 | Zach Muhlbauer | [composing-system-prompts/](./composing-system-prompts/) |
| 2 | **Curating Knowledge Collections** | Thursday, October 1, 2026 | Zach Muhlbauer, Meha Gupta | [curating-knowledge-collections/](./curating-knowledge-collections/) |
| 3 | **Configuring Skills and Tools** | Thursday, October 15, 2026 | Zach Muhlbauer, Meha Gupta | [configuring-skills-tools/](./configuring-skills-tools/) |

The sessions were announced in the Fall 2026 flyer and the [GCDI Orientation](../gcdi-orientation/) as Getting Started with the CUNY AI Lab Sandbox, Building Custom Models with Knowledge Collections, and Extending Custom Models with Skills & Tools.

### Workshop Roadmap

| Session | Activity | Required access | Next steps |
|---------|----------|-----------------|------------|
| Composing System Prompts | Configure model behavior with system prompts | Active Sandbox account and Workspace Models access | Draft original instructions; create a configuration; select source documents |
| Curating Knowledge Collections | Organize source documents in knowledge collections | Session 1 access, Workspace, Knowledge collection access | Save retrieval tests; request Skills and Tools access |
| Configuring Skills and Tools | Extend model capabilities with skills and tools | Session 1 access, Skills and Tools access; Workspace authoring for creation and editing | Save configurations; verify shared access; retest after changes |

## What Changed from Spring 2026

- **One running example.** The Spring decks taught through weak, mediocre, and strong examples across composition, history, and literature. The Fall series replaces them with an actual custom model, **STEM Adventure Games** (a text adventure with numbered choices grounded in source documents), plus a research counterpart, **Compare Wikipedia Edits**. Participants clone, revise, ground, and extend the same model across the three sessions.
- **Participant-facing copy.** Slide headings are two or three words; instructions address participants directly; agendas begin with action verbs. Presenter directions live in the published lesson plans rather than on slides.
- **Current interface.** Screenshots were recaptured in Firefox in September and October 2026, with provenance, crop coordinates, and hashes recorded in the repository's review files.
- **Evidence discipline.** The materials distinguish source instructions, observed interface behavior, and model results, and label any test that was not run.

## Interactive Tools

- **[CUNY AI Lab Sandbox](https://chat.ailab.gc.cuny.edu/)** - Self-hosted chat platform (Open WebUI) with open-weight models behind CUNY Login
- **[Model Registry](https://ailab.gc.cuny.edu/models/)** - Available models, licenses, abilities, and limits
- **[Model Access](https://tools.ailab.gc.cuny.edu/model-access)** - Monthly usage and allowance
- **[Sandbox Documentation](https://ailab.gc.cuny.edu/sandbox-docs/)** - Getting Started, Quick Tour, Models, Knowledge Bases, Tools & Skills, Roles & Permissions
- **[STEM Adventure Games](https://chat.ailab.gc.cuny.edu/?model=stem-adventure-games)** - Teaching example used across the series
- **[Compare Wikipedia Edits](https://chat.ailab.gc.cuny.edu/?model=compare-wikipedia-revisions)** - Research example used in session 1
- **[CAIL Workspace Support](https://chat.ailab.gc.cuny.edu/?model=cail-workspace-support)** - Support model used in session 3 to revise or create skills and tools

## Technical Details

### Built With

- Static HTML, CSS, and JavaScript; no build step and no runtime dependencies
- Light and dark themes that persist across workshop and reading pages
- Keyboard, slider, and touch navigation; an Outline view links every session, the full workshop copy, and the Model Registry
- A checker script keeps the complete transcript, per-session mirrors, and copy diffs synchronized and verifies local links, screenshot hashes, accessible slide labels, and article-free agendas

### Slide Decks and Materials

- **[Series Landing Page](https://cuny-ai-lab.github.io/sandbox-series/)**
- **[Composing System Prompts](https://cuny-ai-lab.github.io/sandbox-series/basics/)** · [Full copy](https://cuny-ai-lab.github.io/sandbox-series/basics/workshop-copy.html)
- **[Curating Knowledge Collections](https://cuny-ai-lab.github.io/sandbox-series/knowledge/)** · [Full copy](https://cuny-ai-lab.github.io/sandbox-series/knowledge/workshop-copy.html)
- **[Configuring Skills and Tools](https://cuny-ai-lab.github.io/sandbox-series/skills/)** · [Slides PDF](https://cuny-ai-lab.github.io/sandbox-series/skills/Tools-and-Skills-Slides.pdf) · [Participant exercises](https://cuny-ai-lab.github.io/sandbox-series/skills/exercises.html) · [Facilitator notes](https://cuny-ai-lab.github.io/sandbox-series/skills/facilitator.html)
- **[Presenter lesson plans and access requirements](https://cuny-ai-lab.github.io/sandbox-series/WORKSHOP.html)**
- **[GitHub Repository](https://github.com/CUNY-AI-Lab/sandbox-series)** - Source, review history, screenshot provenance, and example artifacts

### Workshop Artifacts

- [STEM Adventure tool](https://cuny-ai-lab.github.io/sandbox-series/examples/tools/stem_adventure.html) and [playable preview](https://cuny-ai-lab.github.io/sandbox-series/examples/adventure/preview.html)
- [Extend STEM Adventures skill](https://cuny-ai-lab.github.io/sandbox-series/examples/stem-game-skill.html)
- [STEM Adventure Games system prompt](https://cuny-ai-lab.github.io/sandbox-series/examples/stem-system-prompt.html)
- [Prism Laboratory scenario](https://cuny-ai-lab.github.io/sandbox-series/examples/adventure/prism.html), [aperture variation](https://cuny-ai-lab.github.io/sandbox-series/examples/adventure/aperture.html), and [winning commands](https://cuny-ai-lab.github.io/sandbox-series/examples/adventure/winning-commands.html)
- [Additional knowledge entries](https://cuny-ai-lab.github.io/sandbox-series/WORKSHOP.html#additional-knowledge-entries) (Newton's optical experiments, procedural variants, game procedure evaluation, source register)
- [Skill Creator instructions](https://cuny-ai-lab.github.io/sandbox-series/examples/creators/skill-creator-system-prompt.html) and [Tool Creator instructions](https://cuny-ai-lab.github.io/sandbox-series/examples/creators/tool-creator-system-prompt.html)

## Sources

Developed by Zach Muhlbauer from the Spring 2026 repositories [system-prompting](https://github.com/CUNY-AI-Lab/system-prompting), [knowledge-collections](https://github.com/CUNY-AI-Lab/knowledge-collections), and [skills-tools](https://github.com/CUNY-AI-Lab/skills-tools). Platform instructions follow the [CUNY AI Lab Sandbox documentation](https://ailab.gc.cuny.edu/sandbox-docs/) and the Open WebUI documentation for [Models](https://docs.openwebui.com/features/workspace/models/), [Knowledge](https://docs.openwebui.com/features/workspace/knowledge/), and [Skills](https://docs.openwebui.com/features/workspace/skills/).

## License

All materials are licensed under a **Creative Commons Attribution-ShareAlike (CC-BY-SA) 4.0 International Public License** unless otherwise noted.
