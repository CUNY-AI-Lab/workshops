# Curating Knowledge Collections (Fall 2026)

_Session 2 of the CUNY AI Lab Sandbox Workshop Series: organize source documents in knowledge collections._

Participants clone the STEM Adventure Games custom model, choose sources for a topic they want players to explore, build their own private knowledge collection from pasted excerpts, write an instructions file that tells the model how to use each source, revise the cloned system prompt to consult it, and test the result against the original. The session introduces retrieval-augmented generation (RAG) and ends with participants checking citations, comparing responses, and revising one source or instruction.

**Workshop Date:** Thursday, October 1, 2026
**Time:** 2:30–4:00 p.m. (90 minutes)
**Location:** New Media Lab, Room 7388.01, CUNY Graduate Center
**Format:** Hands-on workshop (Session 2 of 3; can also be taken independently)
**Facilitators:** Zach Muhlbauer and Meha Gupta (CUNY AI Lab)
**Required access:** Session 1 access, plus Workspace and Knowledge collection access

_This session was originally conducted as part of the [Sandbox Workshop Series](../) at the CUNY Graduate Center. It revises the Spring 2026 workshop [Curating Knowledge Collections](../../knowledge-collections/)._

## About the CUNY AI Lab

The **CUNY AI Lab** is a faculty and staff-led incubator for experimentation with AI by CUNY researchers across disciplines, strengthening CUNY's position at the leading edge of technological innovation. Located at the CUNY Graduate Center and led by experienced scholars and technologists who have built widely used open publishing platforms, the Lab fosters momentum for AI experimentation while foregrounding ethical practices and values that reinforce CUNY's mission of accessible, equitable, and transformative education.

This workshop is part of the CUNY AI Lab's commitment to developing critical AI literacy among faculty, staff, and students across the university system.

## Overview

A knowledge collection holds documents a custom model can search. RAG retrieves relevant passages and adds them to the model's context alongside the request and the system prompt. Rather than discussing collection design in the abstract, the session has every participant clone one working model, inspect the example collection it draws on (an instructions file plus three Wikipedia article files), and then rebuild that structure for a topic of their own: a Wikipedia article as the grounding source, a secondary source for interpretation, a heuristic source for decision rules, and an instructions file that says which is which. Testing is built in: ask the model which passage supports a scene, open the citation, compare with the original model, revise, and retest.

## Learning Objectives

- Explain retrieval-augmented generation (parse, chunk, embed; retrieve, add context, generate) and what it means for how sources are organized
- Clone a custom model and inspect the knowledge collection it uses
- Create a private knowledge collection with a directory of source excerpts, each with its link, plus secondary and heuristic sources
- Write an instructions file and revise a system prompt so the model consults it before retrieving passages
- Test a grounded model by checking citations, comparing responses with the original, and revising one source or instruction

## Workshop Structure

1. **Workshop Agenda** - Explore and clone (15 min), select new sources (25 min), create and populate collections (20 min), revise system prompts (10 min), test and revise (20 min)
2. **Retrieval-Augmented Generation** - Search documents → retrieve passages → generate response
3. **RAG Under the Hood** - Processing documents (parse, chunk, embed) and responding to requests (retrieve, add context, generate)
4. **Explore STEM Adventures** - A text adventure with numbered choices that uses source documents
5. **Clone and Name Your Copy** - Workspace → Models → ⋯ → Clone; base model, system prompt, and settings carry over
6. **Try the Custom Model** - Ask for four adventure options, choose one, try its numbered choices
7. **Example Sources** - The Sandbox Workshop Collection: instructions.txt at the root, a Wikipedia directory with three article files
8. **Choose Purpose and Find Sources** - A topic, an audience, a question players can investigate; start with one article
9. **Create Your Collection** - Workspace → Knowledge → Create; keep access Private
10. **Add Source Text** - New directory, Add text content, article title as filename, paste excerpts with the link, Save
11. **Add Source Guidance** - A secondary source and a heuristic source in separate, clearly named files
12. **Add Instructions** - instructions.txt at the collection root; attach the collection; revise Purpose, Audience, and the retrieval directions in the system prompt
13. **Test, Check Citations, Compare** - New chat with the saved copy; "Which passage supports this scene?"; same request to the original
14. **Revise and Retest** - Change one source or instruction, wait for processing or Save & Update, repeat the request
15. **Share Custom Model** - Read access to the model and its collection; parting questions and resources

## Interactive Tools

- **[CUNY AI Lab Sandbox](https://chat.ailab.gc.cuny.edu/)** - Workspace → Models and Workspace → Knowledge
- **[STEM Adventure Games](https://chat.ailab.gc.cuny.edu/?model=stem-adventure-games)** - The example model participants clone
- **[Sandbox Knowledge documentation](https://ailab.gc.cuny.edu/sandbox-docs/knowledge-bases/)** and **[Open WebUI Knowledge](https://docs.openwebui.com/features/workspace/knowledge/)**
- **[Sandbox Roles & Permissions](https://ailab.gc.cuny.edu/sandbox-docs/roles-permissions/)** - Sharing models and collections

## Technical Details

### Slide Deck

- **[Live Slides](https://cuny-ai-lab.github.io/sandbox-series/knowledge/)** - Interactive slideshow
- **[Full workshop copy](https://cuny-ai-lab.github.io/sandbox-series/knowledge/workshop-copy.html)** - Complete text and alt text
- **[Presenter lesson plan](https://cuny-ai-lab.github.io/sandbox-series/WORKSHOP.html)** - Timed plan, preparation notes, and additional knowledge entries
- **[GitHub Repository](https://github.com/CUNY-AI-Lab/sandbox-series)** - Source code and materials

### Example Collection and Additional Entries

The example collection contains three Wikipedia imports (List of experiments, Scientific method, Women in science) with an instructions file. The repository adds four knowledge entries that can be used for testing: Newton's _Light and Colour_, Newton's experimental variants, a game-procedure evaluation, and a source register documenting a repaired import.

### Related Sessions

- **[Composing System Prompts](../composing-system-prompts/)** - Session 1, September 17, 2026
- **[Configuring Skills and Tools](../configuring-skills-tools/)** - Session 3, October 15, 2026

## Notes from Delivery

During preparation on September 29, 2026, the Sandbox's **Add webpage** option returned an error for Wikipedia URLs through a non-admin account. The session therefore has participants copy excerpts and source links through **Add text content**. Live Wikipedia retrieval with tools was deferred to Session 3.

## License

All materials are licensed under a **Creative Commons Attribution-ShareAlike (CC-BY-SA) 4.0 International Public License** unless otherwise noted.
