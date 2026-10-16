# Customizing Skills & Tools - Workshop Outline

## Workshop Information

**Title:** Customizing Skills & Tools
**Date:** Monday, March 30, 2026
**Duration:** 90 minutes
**Format:** Interactive workshop (Week 3 of a 3-week series on the CUNY AI Lab Sandbox)
**Facilitators:** Stefano Morello & Zach Muhlbauer (CUNY AI Lab)

**Learning Objectives:**
- Distinguish a skill from a tool and from the system prompt
- Identify a repeatable pedagogical move worth turning into a skill
- Evaluate skills through before-and-after examples in three disciplines
- Write a skill with a trigger, a procedure with wait points, and a format
- Create, attach, reference, and test the skill in the Sandbox

## Detailed Agenda

### Roadmap: Three Weeks, Three Skills

- **March 16:** Composing System Prompts - defined how the AI thinks, responds, and engages with students
- **March 23:** Curating Knowledge Collections - grounded the model in course materials
- **March 30 (this week):** Customizing Skills & Tools - build specialized skills, tools, and workflows

### Pre-Flight

- **System prompt:** what role and constraints did you set? Have you revised or tested it?
- **Knowledge collection:** is it attached? Does the model draw on it when you test?
- **Name one pedagogical move:** something you do as an instructor that follows a repeatable pattern (narrowing a research topic one question at a time, walking a student through a source, guiding them from description to interpretation). Skills enable the model to mimic those moves.

### What Is a Skill?

A **skill** is a structured procedure written in markdown or plain text. It tells the model how to handle a task the system prompt can't cover on its own: a recipe for a move you'd make as an instructor (establishing stasis, sourcing a document, reading a cinematic frame), written so the model executes it consistently. The system prompt sets general behavior; a skill decomposes a *specific* task into steps the model won't follow unprompted.

What you build: Week 1 system prompt (behavior and constraints) + Week 2 knowledge (syllabus, rubric) + a new skill (step-by-step recipe). The student never sees any of it; they see the response that follows the skill's procedure.

### Activating Skills in Open WebUI

A skill is worth making when the move has a repeatable structure (trigger, steps, output shape).

1. **Create the skill:** Workspace → Skills → + New Skill; write or paste the text.
2. **Add it to your model:** open the model card in Workspace → Models, scroll to Skills, toggle it on. It activates in every chat with that model.
3. **Reference it in your system prompt:** at the bottom, for example "Follow the Stasis Theory skill when a student is narrowing a topic."

Alternative: paste skill text directly into the system prompt, which crowds the prompt and is harder to maintain.

### Why Skills Matter

A student types, "I want to write about social media and mental health."

- **Without a skill:** a list of ways to narrow (platform, age group, type of impact) and a reminder to have a thesis. The student still has no method for choosing.
- **With a stasis-theory skill:** "Your topic: social media and mental health. Let's start with the facts. What specific situation are you responding to? What has happened that makes this a question worth asking right now?" One stasis question (conjecture), grounded in the student's words.

### The Gap Skills Fill

What models won't do without a skill: walk through stasis one question at a time; quote a passage from an uploaded source before asking; ask one focused question instead of listing five; build on what the student just said; scaffold from description to analysis to interpretation. System prompt alone: the model knows *what* to do. System prompt + skill: it knows *what* and *how*.

### What Is a Tool?

A **tool** is a function the model can call to do something it can't do with language alone: search the web, query uploaded files, run code, generate an image. Some are built in (Web Search, Code Interpreter); others are custom, written in Python or imported from the Open WebUI community library via Workspace → Tools.

- **Per chat:** click the controls icon next to the message bar to open the tools menu and toggle tools on for that conversation.
- **Per model:** open the model card in Workspace → Models and scroll to Tools to attach custom tools permanently. Capabilities at the bottom are tools native to the Sandbox.
- **Caveat:** smaller models (for example, Gemma 3 27B) call tools inconsistently; use Kimi K2.5 or GLM 5 for reliable tool use.

### Skills vs. Tools

A skill is a document you write in plain text: a procedure the model follows. A tool is code: a function the model calls. Today's focus is skills; tools are ready to use out of the box. Built-in tools: Web Search (current information), Knowledge Query (search uploaded files), Code Execution (run code in a sandbox), Image Generation.

### Example 1: Establishing Stasis (Composition)

**Before:** "When a student is developing a research topic, walk them through four stages -- conjecture, definition, quality, and policy -- to help them narrow their question. Ask one stasis at a time." The model walks through all four stages in one response, treats stasis as a checklist, and skips helping the student see which stasis their argument lives in.

**After:** a skill with a trigger ("When a student is developing or narrowing a research topic"), a six-step procedure (state the topic in one sentence; conjecture; definition; quality; policy; which question does your argument most need to answer?), each step waiting for the student's answer and using it to sharpen the next question, and a format (the topic, one stasis question tied to a phrase the student used, one or two sentences on why it matters).

### Example 2: Sourcing a Document (History)

**Before:** "When a student asks about a primary source, retrieve it from the knowledge collection and walk them through its rhetorical situation using SOAPS. Ask questions one element at a time rather than summarizing." The model paraphrases instead of quoting and rushes through all dimensions.

**After:** a seven-step procedure: retrieve and quote a key passage (never paraphrase); present it as a block quote with metadata from the uploaded file; ask who created it and with what stake; point to a phrase that supports or complicates the answer; ask when and where it was written; ask who the intended audience was; then ask what the source can and can't tell us. Format: the quoted passage with author, title, and date; one sourcing question; one or two sentences tying it to a phrase in the passage.

### Example 3: Reading the Frame (Literature)

**Before:** "When a student shares a film still or visual artifact, guide them from describing formal elements toward interpreting how those choices construct meaning in context." The model describes the image for the student and treats all elements at once.

**After:** a six-step procedure: use the uploaded image or retrieve it from the collection (say so if it isn't there); ask "What do you notice first?"; direct attention to one formal element they haven't mentioned; ask how it shapes the viewer's experience; introduce context, quoting the collection if relevant; guide toward an interpretive claim. Framework: description → analysis → interpretation.

### Anatomy of a Skill

- **Trigger:** when should this skill activate? What student action starts the workflow? Automatic or on request?
- **Procedure:** numbered steps in order, with wait points; whether to quote, cite, or reference specific materials
- **Format:** what the output looks like; whether to quote the student's text; whether each response ends with a question; how long

### Hands-On: Write Your First Skill

**Choose your move:** establishing stasis, sourcing a document, reading the frame, or something else.

**Draft it** with the template:

```text
Skill: [Name]
When a student [trigger action], follow this procedure:

Procedure:
1. [First step]
2. [Second step -- include wait points]
3. [Third step]

Format:
> [quoted text from student or source]

[Observation in 1-2 sentences]
[One question]
```

**Add it:** Workspace → Skills → + New Skill; toggle it on in the model card; reference it in the system prompt.

**Test it:** open a new chat and trigger the skill with realistic student input. Does it follow the procedure? If the model skips steps, add wait points. If it dumps everything, add "one per turn."

### What You've Built

System prompt (role, constraints, tone) + knowledge collection (syllabus, rubric, readings, sources) + your skill (step-by-step recipe) = a custom AI tool with three modular layers that can be tested as a configuration and refined iteratively, so you can see what each component contributes before introducing it in the classroom.

## Materials Needed

- Laptop/projection for demos
- Participant access to the CUNY AI Lab Sandbox with Workspace permissions
- Each participant's model card with system prompt (Week 1) and knowledge collection (Week 2)
- The skill template, ready to paste
