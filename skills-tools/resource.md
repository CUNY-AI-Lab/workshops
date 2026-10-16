# Customizing Skills & Tools

**Companion Worksheet**

*This worksheet guides you through writing one skill for a pedagogical move from your course and adding it to your custom model on the CUNY AI Lab Sandbox.*

## Pre-Flight

- ☐ **System prompt:** role and constraints set; revised or tested since Week 1
- ☐ **Knowledge collection:** attached; the model draws on it when tested
- ☐ **One pedagogical move** that follows a repeatable pattern: ______________________

## Skill vs. Tool

| | Skill | Tool |
|---|---|---|
| What it is | Plain text you write: a procedure the model follows | Code, pre-built or imported: a function the model calls |
| What it does | Shapes *how* the model handles a specific move | Gives the model a capability it lacks (search, files, code, images) |
| Where | Workspace → Skills, toggled on in the model card | Per chat (controls icon) or per model (model card → Tools) |

## Choose Your Move

- ☐ **Establishing stasis** - narrow a research topic one question at a time
- ☐ **Sourcing a document** - quote, then ask who, when, for whom
- ☐ **Reading the frame** - describe → analyze → interpret
- ☐ **Something else:** ______________________

## 1. Trigger

What student action starts this? A draft, a question about a source, an uploaded image? Automatic or on request?

```text
Skill: [Skill Name]
When a student [specific action or input], follow this procedure:
```

**My trigger:**

------------------------------------------------------------------------

## 2. Procedure

Write 3–5 numbered steps in the sequence you follow yourself. Mark where the model should wait for the student before continuing. Say whether it should quote, cite, or reference specific materials.

```text
Procedure:
1. [First step -- what does the model do or ask?]
2. [After the student responds, what comes next?]
3. [Continue the sequence -- include wait points]
4. [Final step -- synthesis, next action, or handoff]
```

**My procedure:**

1. ______________________
2. ______________________
3. ______________________
4. ______________________
5. ______________________

## 3. Format

What should each response look like? Should it quote the student's text? End with a question? How long?

```text
Format:
> [quoted excerpt from student work or source document]

[1-2 sentences: what you observe]
[One question for the student]
```

**My format:**

------------------------------------------------------------------------

## Add It to Your Model

1. ☐ **Workspace → Skills → + New Skill:** paste your skill text
2. ☐ **Workspace → Models → your model card → Skills:** toggle it on
3. ☐ **Bottom of your system prompt:** "Follow the [Skill Name] skill when a student [trigger]."

## Test It

Open a new chat and trigger the skill with realistic student input.

**Student input I used:**

------------------------------------------------------------------------

**Did it follow the procedure?** ☐ Yes ☐ Skipped steps ☐ Dumped everything at once

**Fix:** if it skips steps, add wait points. If it dumps everything, add "one per turn."

**What I changed and what happened next:**

------------------------------------------------------------------------

## What You've Built

| Layer | Week | Contains |
|-------|------|----------|
| System prompt | 1 | Role, constraints, tone |
| Knowledge collection | 2 | Syllabus, rubric, readings, sources |
| Skill | 3 | Step-by-step recipe for a specific move |

Test the configuration as a whole, then refine one layer at a time so you can see what each contributes before introducing it in the classroom.

## Resources

- [CUNY AI Lab Sandbox](https://chat.ailab.gc.cuny.edu/)
- [Open WebUI community tools](https://openwebui.com/search?sort=top&t=all&page=1&type=tool)
- [Composing System Prompts](https://cuny-ai-lab.github.io/system-prompting/) (Week 1) and [Curating Knowledge Collections](https://cuny-ai-lab.github.io/knowledge-collections/) (Week 2)
