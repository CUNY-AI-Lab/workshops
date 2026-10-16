# Curating Knowledge Collections

_A CUNY AI Lab workshop on grounding custom AI models in course materials through knowledge collections._

This workshop teaches instructors how to build a knowledge collection -- the set of documents a custom model retrieves from when responding to students -- and how to curate it with pedagogical intent. Through three progressive examples across composition, history, and literature, participants learn what retrieves well, what goes wrong with omnibus files, and how to layer course framework, assignment materials, and source materials for a single assignment.

**Workshop Date:** Monday, March 23, 2026
**Duration:** 90 minutes
**Format:** Interactive workshop (Week 2 of a 3-week series)
**Facilitators:** Stefano Morello & Zach Muhlbauer (CUNY AI Lab)

_This workshop is part of a three-week series on using the CUNY AI Lab Sandbox in the classroom. It was revised for the Fall 2026 [Sandbox Workshop Series](../sandbox-series/curating-knowledge-collections/)._

## About the CUNY AI Lab

The **CUNY AI Lab** is a faculty and staff-led incubator for experimentation with AI by CUNY researchers across disciplines, strengthening CUNY's position at the leading edge of technological innovation. Located at the CUNY Graduate Center and led by experienced scholars and technologists who have built widely used open publishing platforms, the Lab fosters momentum for AI experimentation while foregrounding ethical practices and values that reinforce CUNY's mission of accessible, equitable, and transformative education.

This workshop is part of the CUNY AI Lab's commitment to developing critical AI literacy among faculty, staff, and students across the university system.

## Overview

The system prompt tells the model how to behave; the knowledge collection tells it what to draw on. The workshop opens with model setup (create or reopen a model card, attach the system prompt from Week 1, test it in chat), explains what a knowledge collection is and how retrieval-augmented generation chunks, searches, and injects passages, then contrasts weak, getting-warmer, and strong collections in three disciplines. Part II condenses curation best practices and common pitfalls. Part III is a hands-on build: participants pick one assignment and assemble a collection in three layers using copyable templates, then test whether the model answers a question only the collection could answer.

## Learning Objectives

- Distinguish the system prompt (behavior) from the knowledge collection (context) and explain how they work together on a model card
- Describe how retrieval-augmented generation chunks documents, matches a question against passages, and injects the closest matches into the model's context
- Evaluate a knowledge collection through progressive examples (weak, getting warmer, strong) across composition, history, and literature
- Apply curation best practices: one document, one purpose; metadata and headings; meta documents that signpost use; per-unit updates
- Build a three-layer collection (course framework, assignment materials, source materials) for one assignment and test it

## Workshop Series

| Week | Date | Topic |
|------|------|-------|
| Week 1 | March 16 | [Composing System Prompts](../system-prompting/) |
| **Week 2** | March 23 | **Curating Knowledge Collections** (this workshop) |
| Week 3 | March 30 | [Customizing Skills & Tools](../skills-tools/) |

## Workshop Structure

### Model Setup (slides 3–5)

Sign in at chat.ailab.gc.cuny.edu, open Workspace, create or reopen a model card, name it for your course, select a base model, paste last week's system prompt, save, and test it in a new chat.

### What, Where, Why, Upload (slides 6–10)

- What a knowledge collection is: the reading list for your AI tool
- Where it lives: Workspace → Knowledge, attached to a model under Knowledge
- Why it matters: generic midterm advice versus advice grounded in the assignment prompt and the course's SOAPS framework
- What you can upload: syllabi, assignment prompts, rubrics, readings, lecture notes, style guides, sample work, data sets, glossaries, problem sets, lab protocols, case studies
- How the model uses documents: chunking, search, injection, response; short, focused documents with clear headings retrieve better

### Part I: What Makes a Good Collection? (slides 11–22)

1. **Composition & Writing** - From a lone 14-page syllabus to a three-layer collection that grounds revision (syllabus, revision philosophy, essay prompt, common feedback, MLA guide, strong-intro examples, revision checklist)
2. **Primary Source Analysis** - From a 42-page textbook chapter to a collection that fosters historical thinking (SOAPS framework, two Reconstruction-era primary sources with metadata, source-context notes, timeline, common analysis errors, Chicago guide)
3. **Close Reading & Literary Analysis** - From a 180-page course reader to a collection that fosters close reading (New Criticism framework, close-reading assignment, annotated passage example, Baldwin's "Sonny's Blues," passage selections)

### Part II: Best Practices & Pitfalls (slides 23–24)

One document, one purpose; add metadata and headings; supply what's not in the documents; update per unit. Watch out for dumping everything in, one giant PDF, forgetting the system prompt, and assuming full coverage.

### Part III: Hands-On Exercise (slides 25–28)

Pick one assignment and build a collection one layer at a time, each with a copyable template: Layer 1 course framework, Layer 2 assignment materials, Layer 3 source materials.

### Prompt + Collection and Closing (slides 29–30)

A paired system prompt and collection for an ENGL 101 revision scaffold; test with a question only the collection can answer. The road ahead: Skills & Tools next week.

## Interactive Tools

- **[CUNY AI Lab Sandbox](https://chat.ailab.gc.cuny.edu/)** - Self-hosted chat platform; documents are stored on CUNY's self-hosted servers and private by default
- **[Model Registry](https://ailab.gc.cuny.edu/models/)** - Base models available in the Sandbox

## Technical Details

### Built With

- Custom single-page HTML deck with a hand-rolled engine (no framework, no build step); 30 slides
- Step reveals, streamed bullets, an auto-advancing screenshot carousel, a lightbox for screenshots, and an ARIA slider scrubber
- WCAG 2.1 AA target: slide roles and labels, live-region announcements, focus management, reduced-motion support
- Fraunces, DM Sans, and JetBrains Mono from Google Fonts

### Slide Deck

- **[Live Slides](https://cuny-ai-lab.github.io/knowledge-collections/)** - Interactive slideshow
- **[GitHub Repository](https://github.com/CUNY-AI-Lab/knowledge-collections)** - Source code and materials

### Related Workshops

- **[Composing System Prompts](../system-prompting/)** - Week 1
- **[Customizing Skills & Tools](../skills-tools/)** - Week 3
- **[Curating Knowledge Collections (Fall 2026)](../sandbox-series/curating-knowledge-collections/)** - The revised session in the Sandbox Workshop Series

## License

All materials are licensed under a **Creative Commons Attribution-ShareAlike (CC-BY-SA) 4.0 International Public License** unless otherwise noted.
