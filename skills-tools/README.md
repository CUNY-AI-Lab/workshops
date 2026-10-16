# Customizing Skills & Tools

_A CUNY AI Lab workshop on writing skills -- step-by-step procedures a custom model follows -- and attaching tools to it._

This workshop completes the Spring 2026 three-week series. A **skill** is a structured procedure written in plain text that tells the model how to handle a task the system prompt cannot cover on its own: a recipe for a pedagogical move you make as an instructor. A **tool** is a function the model can call to do something it cannot do with language alone. Through three before-and-after examples (stasis theory in composition, the sourcing heuristic in history, cinematic mise-en-scène in literature), participants learn a three-part anatomy (trigger, procedure, format), write a skill for one move from their own course, and add it to the model they built in Weeks 1 and 2.

**Workshop Date:** Monday, March 30, 2026
**Duration:** 90 minutes
**Format:** Interactive workshop (Week 3 of a 3-week series)
**Facilitators:** Stefano Morello & Zach Muhlbauer (CUNY AI Lab)

_This workshop is part of a three-week series on using the CUNY AI Lab Sandbox in the classroom. It was revised for the Fall 2026 [Sandbox Workshop Series](../sandbox-series/configuring-skills-tools/)._

## About the CUNY AI Lab

The **CUNY AI Lab** is a faculty and staff-led incubator for experimentation with AI by CUNY researchers across disciplines, strengthening CUNY's position at the leading edge of technological innovation. Located at the CUNY Graduate Center and led by experienced scholars and technologists who have built widely used open publishing platforms, the Lab fosters momentum for AI experimentation while foregrounding ethical practices and values that reinforce CUNY's mission of accessible, equitable, and transformative education.

This workshop is part of the CUNY AI Lab's commitment to developing critical AI literacy among faculty, staff, and students across the university system.

## Overview

The system prompt sets general behavior; a skill decomposes a specific task into steps the model will not follow unprompted: walk through stasis one question at a time, quote a passage before asking about it, ask one focused question instead of listing five, build on what the student just said. The workshop shows where skills live in Open WebUI (Workspace → Skills, toggled on in the model card, referenced at the bottom of the system prompt), contrasts a response with and without a stasis-theory skill, explains built-in and custom tools and how to enable them per chat or per model, and then hands participants a four-part template to draft, add, and test their own skill. The closing slide shows the three modular layers assembled: system prompt, knowledge collection, skill.

## Learning Objectives

- Distinguish a skill (a plain-text procedure the model follows) from a tool (code the model calls) and from the system prompt
- Identify a repeatable pedagogical move with a trigger, steps, and output shape that is worth turning into a skill
- Evaluate skills through before-and-after examples in composition, history, and literature
- Write a skill using the three-part anatomy (trigger, procedure, format) with explicit wait points
- Create the skill in Workspace → Skills, toggle it on in a model card, reference it in the system prompt, and test it with realistic student input

## Workshop Series

| Week | Date | Topic |
|------|------|-------|
| Week 1 | March 16 | [Composing System Prompts](../system-prompting/) |
| Week 2 | March 23 | [Curating Knowledge Collections](../knowledge-collections/) |
| **Week 3** | March 30 | **Customizing Skills & Tools** (this workshop) |

## Workshop Structure

### Pre-Flight

Verify the system prompt and knowledge collection from previous weeks, then name one pedagogical move that follows a repeatable pattern.

### The Basics

- **What is a skill?** A recipe for a move you'd make as an instructor, written so the model executes it consistently
- **Activating skills:** create in Workspace → Skills; toggle on in the model card; reference at the bottom of the system prompt (or, less maintainably, paste into the prompt)
- **Why skills matter:** "social media and mental health" with and without a stasis-theory skill
- **The gap skills fill:** what models won't do without a step-by-step recipe
- **What is a tool?** Built-in (Web Search, Code Interpreter) and custom tools; per-chat and per-model enablement; smaller models call tools inconsistently
- **Skills vs. tools:** you write a skill; a tool is pre-built or imported code

### Three Examples (Before → After)

1. **Establishing Stasis** (Composition) - From "walk them through four stages" to a six-step procedure that asks one stasis question at a time, tied to the student's own words
2. **Sourcing a Document** (History) - From "walk them through SOAPS" to a seven-step procedure that quotes a passage with metadata before asking who, when, and for whom
3. **Reading the Frame** (Literature) - From "guide them from describing to interpreting" to a six-step description → analysis → interpretation procedure that isolates one formal element per turn

### Writing Your Own Skills

Anatomy of a skill: **Trigger** (when it activates), **Procedure** (numbered steps with wait points), **Format** (what each response looks like). Exercise: choose your move, draft it with the template, add it to your model, and test it.

## Interactive Tools

- **[CUNY AI Lab Sandbox](https://chat.ailab.gc.cuny.edu/)** - Workspace → Skills, Models, and Tools
- **[Open WebUI community tools](https://openwebui.com/search?sort=top&t=all&page=1&type=tool)** - Importable custom tools
- **[Model Registry](https://ailab.gc.cuny.edu/models/)** - Kimi K2.5 and GLM 5 were recommended for reliable tool use

## Technical Details

### Slide Deck

- **[Live Slides](https://cuny-ai-lab.github.io/skills-tools/)** - Interactive slideshow (28 slides)
- **[GitHub Repository](https://github.com/CUNY-AI-Lab/skills-tools)** - Source code and materials
- **[Original slide copy](https://github.com/CUNY-AI-Lab/sandbox-series/blob/main/review/skills/before.md)** - The complete text of the March 30 deck, preserved in the Fall 2026 series repository as the baseline for its revision

### Related Workshops

- **[Composing System Prompts](../system-prompting/)** - Week 1
- **[Curating Knowledge Collections](../knowledge-collections/)** - Week 2
- **[Configuring Skills and Tools (Fall 2026)](../sandbox-series/configuring-skills-tools/)** - The revised session in the Sandbox Workshop Series

## License

All materials are licensed under a **Creative Commons Attribution-ShareAlike (CC-BY-SA) 4.0 International Public License** unless otherwise noted.
