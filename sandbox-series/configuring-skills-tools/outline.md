# Configuring Skills and Tools (Fall 2026) - Workshop Outline

## Workshop Information

**Title:** Configuring Skills and Tools
**Date:** Thursday, October 15, 2026, 2:30–4:00 p.m. Eastern
**Location:** New Media Lab, Room 7388.01, CUNY Graduate Center
**Duration:** 90 minutes
**Format:** Hands-on workshop (Session 3 of the Sandbox Workshop Series)
**Facilitators:** Zach Muhlbauer and Meha Gupta (CUNY AI Lab)

**Learning Objectives:**
- Define skills (trigger, procedure, output) and tools (input, execution, result) and explain tool calling
- Configure a model card for tool calling: base model, filter, skill, tool, and a prompt clause that names them
- Verify from call details that a saved skill loaded and a tool function ran
- Revise or create a skill or tool with CAIL Workspace Support while preserving the original
- Add a new version to the model card and compare behavior with identical inputs

## Preparation

- Continue participants' existing models and their actual system prompts. Those prompts define adventure setting, goals, and rules; the reusable tool and skills contain no fixed story or genre.
- Confirm Skills and Tools access and Workspace authoring permissions for participants who will create or edit resources. Verify participant visibility of Adventure Panel, Adventure Panel Play, Adventure Outcomes, and Conclude Adventure Game without expanding permissions.
- Choose a base model that supports tool calling (DeepSeek V4 Flash 0731 was used). Keep the Model Bound Tool Enabler filter available; it restores model-attached tool IDs when chat state omits them.
- Preserve originals. Compare matching prompts, models, sources, and settings. Label any test that was not run.

## Lesson Plan

| Minutes | Time Eastern | Action | Slides |
|---------|--------------|--------|--------|
| 0–10 | 2:30–2:40 | Continue or clone; define skills and tools; select a base model | 1–5 |
| 10–20 | 2:40–2:50 | Enable the filter and select Adventure Panel Play | 6–7 |
| 20–30 | 2:50–3:00 | Select Adventure Panel; check the model card; add the prompt clause and save | 8–10 |
| 30–45 | 3:00–3:15 | Run the adventure, inspect calls, and play | 11–12 |
| 45–55 | 3:15–3:25 | Experiment with other available skills | 13 |
| 55–60 | 3:25–3:30 | Choose a revision or creation task | 14 |
| 60–75 | 3:30–3:45 | Work with CAIL Workspace Support | 15–16 |
| 75–90 | 3:45–4:00 | Add a new version, retest, and reflect across the series | 17–18 |

## Detailed Agenda

### Choose Your Own Adventure

1. Continue your saved model, or clone **STEM Adventure Games** in **Workspace → Models → ⋯ → Clone**.
2. Open **Workspace → Models → Edit** and review your system prompt's setting, goals, and rules.
3. Keep your model card open to add a skill and a tool.

### What Is a Skill?

**Skills** contain plain-text instructions for repeatable tasks.

- **Trigger:** request or condition that starts a procedure
- **Procedure:** steps, checks, and points that require a question
- **Output:** required response content and form

### What Is a Tool?

When a model calls a **tool**, it is given the ability to execute a function and return its result, usually through a Python script. This is called **tool calling** (also **function calling**).

- **Input:** information passed to a function
- **Execution:** code that applies specified rules
- **Result:** returned output for a model to inspect

### Update Model for Tool Calling

On the model card, set **Base Model** to a model that supports tool calling (DeepSeek V4 Flash 0731 in the session).

### Enable Filter

Under **Filters → Select Filter**, enable **Model Bound Tool Enabler**, which binds assigned tools to the model's operations.

### Add Your Skill

1. Open **Workspace → Models → Edit → Skills → Select Skill**.
2. Choose **Adventure Panel Play** and read its saved instructions. This orchestration skill coordinates Adventure Panel according to your model's system prompt.
3. Keep your model card open to add **Adventure Panel**.

### Add the Adventure Panel Tool

1. Open **Tools → Select Tool** on the same model card.
2. Choose **Adventure Panel** and keep **Adventure Panel Play** selected.
3. Add the system-prompt clause below, then select **Save & Update**.

### Model Card Check-In

Confirm **Adventure Panel** (tool), **Adventure Panel Play** (skill), and **Model Bound Tool Enabler** (filter) are selected. Keep your knowledge collection attached.

### Add Skill Instructions

Add this clause to the bottom of your system prompt:

```text
Load the attached Adventure Panel Play skill (extend-adventure-games) and follow it on every turn. Use show_scene from the Adventure Panel tool to display each scene and its choices. Follow this system prompt's setting, goals, rules, and source instructions.
```

Confirm both the skill and the tool are selected, then **Save & Update**. The prompt, skill, and tool must be saved before testing.

### Test Your Adventure

Run your updated adventure game (the example run begins with `initiate adventure`). Verify that the configured skill and tool are called appropriately, then play the rest of the game. Check the opening menu or scene against your system prompt and any required source passages.

| Check | What to inspect |
|-------|-----------------|
| Skill | Saved Adventure Panel Play instructions actually loaded |
| Orchestration | Skill coordinates Adventure Panel using your prompt's setting, goals, and rules |
| Tool call | Actual function and supplied arguments match the reviewed adventure |
| Result | Tool returns a usable result and an interactive player appears inside chat |
| Play | A selected choice reaches chat, the next scene follows the rules, and a stop request ends play |

### Observe Game Results

1. Check the **Adventure Panel Play** skill call (native discovery may show `view_skill`; confirm the actual saved-skill name and ID).
2. Check the **Adventure Panel** tool call (open details to confirm the `show_scene` function and its arguments).

A direct `$` mention injects skill content and need not produce a `view_skill` call; label which path you used. Naming a skill does not establish that its instructions loaded. Try a choice before and after its stated prerequisite. Ask to stop before the goal is met.

### Explore Other Skills

After your first adventure works, read **Adventure Outcomes** or **Conclude Adventure Game**. Change one skill, save your model card, run your adventure again, and compare results. Leave out required information and check for a question. Judge actual behavior rather than the model's claim that it used a skill.

### Choose Your Task

- **Revise one item:** copy the complete tool code or skill instructions; describe an observed problem and one change.
- **Create your own:** choose a task for your tool or skill; specify its purpose, required input, and expected result.

### Work With Support

Open [CAIL Workspace Support](https://chat.ailab.gc.cuny.edu/?model=cail-workspace-support) and confirm its name below the message box. Support does not inherit your model or previous chats. Supply complete original content, your system prompt, current scenario and play record, required source passages, and the observed problem. Ask for complete content, an explanation, and one test with its expected result; label any unrun test.

### Adapt Your Adventure

Give Support your lesson plan, learning outcome, or disciplinary focus, and ask it to adapt or create a skill or tool that extends your adventure toward that outcome. If live retrieval is unavailable, supply a dated source. Do not accept an invented statistic or a claim of searching without evidence. Review the proposal before saving.

### Add Tools or Skills

Use **Workspace → Tools → Create** or **Skills → Create**. Enter a new Name and ID; preserve the original. Paste complete reviewed code or instructions. Review Access, then **Save & Create**. Select the new item on the model card, turn off the older version, update the prompt clause, and **Save & Update**. Retest with the same model, prompt, settings, scene, and record.

| Test | Expected result |
|------|-----------------|
| Prompt goals | Proposed behavior follows supplied rules |
| Required input absent | Focused question or explicit missing-input result |
| Contradictory instructions | Ask before play |
| Explicit stop | Immediate acknowledgment, no false completion |

### Reflect Across the Series

- What task in your teaching or research could benefit from a skill or tool?
- What would you develop next with the prompts, knowledge collections, skills, and tools you have explored?
- Join the coworking session on October 29, 2026 (2–4 p.m.) to build your adventure into a collection.

### Coworking Sessions

Continue Sandbox and Vibe Coding projects in CUNY AI Lab coworking sessions, with time to build and troubleshoot together. Workshop materials and guides: [ailab.gc.cuny.edu/guides](https://ailab.gc.cuny.edu/guides/).

## Materials Needed

- Projection and a presenter account with Skills and Tools access and authoring permissions
- Participant models saved from Sessions 1 and 2 (or the shared STEM Adventure Games to clone)
- Shared Adventure Panel tool, Adventure Panel Play skill, and optional Adventure Outcomes and Conclude Adventure Game skills with participant Read access
- The system-prompt clause and the two Support request templates, ready to paste
