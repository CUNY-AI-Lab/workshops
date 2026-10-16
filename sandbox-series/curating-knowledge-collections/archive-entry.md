# Curating Knowledge Collections (Fall 2026) - Workshop Archive Entry

## Workshop Overview

**Title:** Curating Knowledge Collections
**Series:** Sandbox Workshop Series, Session 2 of 3
**Date:** Thursday, October 1, 2026, 2:30–4:00 p.m.
**Location:** New Media Lab, Room 7388.01, CUNY Graduate Center
**Duration:** 90 minutes
**Format:** Hands-on workshop (can be taken independently)
**Facilitators:** Zach Muhlbauer and Meha Gupta (CUNY AI Lab)

## Workshop Categories

- Educational Technology
- AI Pedagogy
- Information Literacy

## Description

Participants clone the STEM Adventure Games custom model, choose sources for a topic they want players to explore, build their own private knowledge collection, and revise the cloned system prompt to use those documents. Cloning retains the example's base model and settings, so the session's time goes to curating sources, writing an instructions file, revising instructions, and testing. Participants introduce retrieval-augmented generation, inspect the example collection (an instructions file and three Wikipedia article files), paste excerpts and links into their own collection through Add text content, add a secondary and a heuristic source, attach the collection, and test by checking citations, comparing with the original model, and revising one source or instruction. The session revises the Spring 2026 workshop of the same name.

## Materials

All materials are licensed under a **Creative Commons Attribution-ShareAlike (CC-BY-SA) 4.0 International Public License**.

This archive contains the workshop plan, slide copy, and companion worksheet.

Materials: [Live Slides](https://cuny-ai-lab.github.io/sandbox-series/knowledge/) | [Full copy](https://cuny-ai-lab.github.io/sandbox-series/knowledge/workshop-copy.html) | [Lesson plan](https://cuny-ai-lab.github.io/sandbox-series/WORKSHOP.html) | [GitHub Repository](https://github.com/CUNY-AI-Lab/sandbox-series)

## Learning Objectives

- Explain retrieval-augmented generation and what it means for how sources are organized
- Clone a custom model and inspect the knowledge collection it uses
- Create a private knowledge collection with source excerpts, secondary and heuristic sources, and an instructions file
- Revise a system prompt so the model consults the instructions file before retrieving passages
- Test a grounded model by checking citations, comparing with the original, and revising one source or instruction

## Workshop Agenda

### Explore and Clone (0–15 min)

RAG: search documents, retrieve passages, generate a response; parse, chunk, embed; retrieve, add context, generate. Explore STEM Adventure Games, clone and rename it, try an opening request and its numbered choices.

### Select New Sources (15–40 min)

View the Sandbox Workshop Collection (instructions.txt plus a Wikipedia directory of three article files). Choose a purpose, audience, and a question players could investigate. Start with one Wikipedia article; keep the URL.

### Create and Populate Collections (40–60 min)

Workspace → Knowledge → Create (Private). New directory "Wikipedia"; Add text content with the article title as filename; paste excerpts and the link; Save and check. Add a secondary source and a heuristic source in separate files. Write instructions.txt at the root.

### Revise System Prompts (60–70 min)

Attach the new collection in place of STEM Wikipedia Experiments. Revise Purpose and Audience. Replace the source and retrieval directions with directions to consult instructions.txt; keep numbered steps, Constraints, and Format; Save & Update.

### Test and Revise (70–90 min)

New chat with the copy; "Which passage supports this scene? Quote it and cite your source."; open citations; compare the same opening request with the original; revise one source or instruction and retest. Share with Read access to the model and its collection. Parting questions on future uses and limitations.

---

## Resources

- [STEM Adventure Games](https://chat.ailab.gc.cuny.edu/?model=stem-adventure-games)
- [Sandbox Knowledge documentation](https://ailab.gc.cuny.edu/sandbox-docs/knowledge-bases/), [Open WebUI Knowledge](https://docs.openwebui.com/features/workspace/knowledge/), [Roles & Permissions](https://ailab.gc.cuny.edu/sandbox-docs/roles-permissions/)
- [Additional knowledge entries](https://cuny-ai-lab.github.io/sandbox-series/WORKSHOP.html#additional-knowledge-entries)
- Previous session: [Composing System Prompts](../composing-system-prompts/); next session: [Configuring Skills and Tools](../configuring-skills-tools/), October 15, 2026
