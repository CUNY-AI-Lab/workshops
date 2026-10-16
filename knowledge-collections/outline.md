# Curating Knowledge Collections - Workshop Outline

## Workshop Information

**Title:** Curating Knowledge Collections
**Date:** Monday, March 23, 2026
**Duration:** 90 minutes
**Format:** Interactive workshop (Week 2 of a 3-week series on the CUNY AI Lab Sandbox)
**Facilitators:** Stefano Morello & Zach Muhlbauer (CUNY AI Lab)

**Learning Objectives:**
- Distinguish the system prompt (behavior) from the knowledge collection (context)
- Describe how retrieval-augmented generation chunks, searches, and injects passages
- Evaluate collections through weak, getting-warmer, and strong examples in three disciplines
- Apply curation best practices and avoid common pitfalls
- Build and test a three-layer collection for one assignment

## Detailed Agenda

### Roadmap: Three Weeks, Three Skills

| Date | Session | Description |
|------|---------|-------------|
| March 16 (last week) | Composing System Prompts | How system prompts orchestrate and constrain models to address specific course goals |
| March 23 (this week) | Curating Knowledge Collections | Upload syllabi, readings, and relevant sources to ground models in course materials |
| March 30 | Customizing Skills & Tools | Build specialized skills, tools, and workflows tailored to your courses |

### Getting Started: Sign In and Navigate to Workspace

1. Go to chat.ailab.gc.cuny.edu and sign in with your CUNY account.
2. Open **Workspace** (top left, three rows below "New Chat").

### Before We Start: Set Up Your Model Card

Knowledge collections attach to a model card in Workspace → Models.

1. **Workspace → Models:** click + New Model, or open the model card you built last week.
2. **Name it** for your course (for example, ENGL 101 Writing Scaffold or History 202 Source Analysis Tool).
3. **Select a base model** from the Sandbox (DeepSeek, Qwen3, Llama, and others).
4. **Add your system prompt** under Model Params; paste the prompt you wrote last week.
5. **Save.** Keep this tab open; you will return to attach the collection you build.

### Dry Run: Test Your Model in Chat

New Chat → model selector → choose your model → send a course-related test message. Does it respond as expected? How has your system prompt shaped its output?

### The Basics: What Is a Knowledge Collection?

A set of documents you upload to ground a model in specific course materials; the model retrieves relevant passages when responding. Think of it as the **reading list** for your AI tool. The system prompt tells the model how to behave; the collection tells it what to draw on.

### Where to Find Knowledge Collections

- **Step 1 (done):** your model file is open in Workspace → Models with the system prompt set.
- **Step 2 (today):** Workspace → Knowledge to create the collection; upload documents; return to the model and attach it under Knowledge.

Order matters: model first, collection second. Both live in the same model file.

### Why Knowledge Collections Matter

A student asks, "What should I focus on for the midterm essay?"

- **Without a collection:** generic advice about thesis statements, evidence, and counterarguments.
- **With a collection:** "Based on the assignment prompt, your essay should analyze one primary source from the Reconstruction unit using the SOAPS framework we practiced. The prompt emphasizes evidence and sourcing. Which document are you considering?"

### What Can You Upload?

Syllabi, assignment prompts, rubrics, course readings, lecture notes, style guides, sample work, data sets, glossaries, problem sets, lab protocols, case studies. Documents are stored on CUNY's self-hosted servers and private by default. Only the most relevant passages are retrieved and injected into a single prompt; source materials are referenced, not exposed.

### Under the Hood: Retrieval-Augmented Generation

- **Chunking:** documents are split into smaller passages when uploaded
- **Search:** the student's question is matched against those passages
- **Injection:** closest matches are appended to the model's context window
- **Response:** the model generates output grounded in retrieved passages

**Implication:** short, focused documents with clear headings retrieve better than long, unstructured files.

### Part I: What Makes a Good Knowledge Collection?

**Example 1: Composition & Writing**

- *Weak:* `syllabus.pdf` (14 pages) only. One large document retrieves poorly; no assignment context; no readings.
- *Getting warmer:* syllabus, essay-1-prompt, mla-style-guide. Separate documents retrieve better and the prompt gives task context; still no readings, feedback patterns, or instructor notes on substantive revision.
- *Strong:* Course framework (syllabus.pdf, revision-philosophy.txt); Assignment materials for Essay 1, Rhetoric in Popular Media (essay-1-prompt.pdf, common-feedback.txt); Reference materials (mla-style-guide.pdf, strong-intro-examples.txt, revision-checklist.pdf).

**Example 2: Primary Source Analysis (History)**

- *Weak:* `textbook-chapter-12.pdf` (42 pages) only. Too long and general; no primary sources; no SOAPS framework.
- *Getting warmer:* syllabus, source-analysis-assignment, a Freedmen's Bureau report (1866), Congressional testimony (1871). Actual sources and task context; still no period background, framework, or source metadata.
- *Strong:* Course framework (syllabus.pdf, soaps-framework.txt); Primary sources for the Reconstruction unit with metadata (freedmens-bureau-report-1866.pdf, congressional-testimony-1871.pdf, source-context-notes.txt); Reference materials (period-timeline.txt, common-analysis-errors.txt, chicago-citation-guide.pdf).

**Example 3: Close Reading & Literary Analysis**

- *Weak:* `course-reader.pdf` (180 pages) only. Retrieves unpredictably; no assignment context or framework; literary texts and criticism not separated.
- *Getting warmer:* syllabus, close-reading-assignment, sonny-blues-baldwin, new-criticism-overview. Individual text and methodological grounding; still no annotated examples, unit key terms, or instructor notes.
- *Strong:* Course framework (syllabus.pdf, new-criticism-framework.txt); Assignment materials (close-reading-assignment.pdf, annotated-passage-example.txt); Literary texts for the current unit (sonny-blues-baldwin.pdf, passage-selections.txt).

### Part II: Best Practices & Pitfalls

**Curation best practices**

- **One document, one purpose:** focused documents retrieve better than omnibus ones
- **Add metadata and headings:** titles, authors, dates, and section headings serve as retrieval anchors
- **Supply what's not in the documents:** meta documents such as common-feedback.txt signpost how to use sources
- **Update per unit:** swap materials as the semester progresses

**Common pitfalls**

- **Dumping everything in:** uploading every reading dilutes retrieval; start small
- **One giant PDF:** a 200-page reader retrieves unpredictably
- **Forgetting the system prompt:** without explicit instructions for drawing on the collection, it is a pile of documents
- **Assuming full coverage:** only retrieved passages appear in each response; give critical items their own file

### Part III: Build Your Collection (Hands-On)

Pick one assignment from your course and build a collection one layer at a time.

**Layer 1: Course Framework.** What are the learning objectives? What analytical framework or methodology is central? Template: syllabus.pdf (schedule, objectives, policies) and [framework-name].txt (the method students use, in plain language with definitions). *Your turn:* write a short document (1–2 pages) explaining your framework in the terms you use with students.

**Layer 2: Assignment Materials.** What does the assignment ask? What does strong work look like? What patterns come up in feedback? Template: [assignment]-prompt.pdf, common-feedback.txt (5–10 patterns you see every semester), strong-examples.txt (optional). *Your turn:* curate the instructions alongside a shortlist of common feedback patterns.

**Layer 3: Source Materials.** What are students reading? Are there reference documents? Can you add brief metadata per source? Template: [reading-title].pdf (one file per text, with a header giving title, author, date, source), context-notes.txt (optional, 2–3 sentences per source), [reference-guide].pdf (citation guide, glossary, or timeline). *Your turn:* upload 1–3 readings; split a single PDF reader into separate files first.

### Putting It Together: Prompt + Collection

**System prompt:** "You are a writing revision scaffold for ENGL 101. When a student shares a draft, ask them to identify which area they want to work on first. Reference the assignment prompt and common-feedback documents before responding."

**Knowledge collection:** syllabus.pdf, revision-philosophy.txt, essay-1-prompt.pdf, common-feedback.txt, mla-style-guide.pdf, strong-intro-examples.txt

**Test it:** ask a question only answerable from your collection. If the model gives generic advice, retrieval isn't working; check your document structure.

### The Road Ahead

The system prompt from Week 1 now drives a model grounded in the collection built today. Week 3 (March 30) extends it with custom skills and tools.

## Materials Needed

- Laptop/projection for demos
- Participant access to the CUNY AI Lab Sandbox with Workspace permissions
- Each participant's system prompt from Week 1
- Course documents participants are permitted to upload (syllabus, one assignment prompt, 1–3 readings)
