# Configuring Skills and Tools (Fall 2026)

**Companion Worksheet**

*Use this sheet during Session 3 of the Sandbox Workshop Series. Record each configuration change and what the call details showed.*

## Definitions

| | Skill | Tool |
|---|---|---|
| What it is | Plain-text instructions for a repeatable task | A function the model can execute, usually a Python script |
| Parts | Trigger, procedure, output | Input, execution, result |
| Where it lives | Workspace → Skills; selected on the model card | Workspace → Tools; selected on the model card |

Your system prompt still defines the adventure's setting, goals, and rules.

## Configure Your Model Card

Workspace → Models → **Edit** your saved model (or clone STEM Adventure Games first).

- ☐ **Base Model** supports tool calling (DeepSeek V4 Flash 0731 in the session)
- ☐ **Filters → Model Bound Tool Enabler** enabled
- ☐ **Skills → Adventure Panel Play** selected (read its saved instructions)
- ☐ **Tools → Adventure Panel** selected
- ☐ Knowledge collection still attached
- ☐ This clause added at the bottom of the system prompt:

```text
Load the attached Adventure Panel Play skill (extend-adventure-games) and follow it on every turn. Use show_scene from the Adventure Panel tool to display each scene and its choices. Follow this system prompt's setting, goals, rules, and source instructions.
```

- ☐ **Save & Update** before opening a fresh chat

## Test Your Adventure

Start a new chat with your model. The example run begins with:

```text
initiate adventure
```

| Check | What to inspect | What I observed |
|-------|-----------------|-----------------|
| Skill | Saved Adventure Panel Play instructions actually loaded (open the `view_skill` details; confirm the skill name and ID) | |
| Orchestration | Skill coordinates Adventure Panel using your prompt's setting, goals, and rules | |
| Tool call | The `show_scene` function and its arguments match the reviewed adventure | |
| Result | Tool returns a usable result and an interactive player appears in chat | |
| Play | A selected choice reaches chat, the next scene follows the rules, and a stop request ends play | |

Try a choice before and after its prerequisite. Ask to stop before the goal is met.

**Which path loaded the skill: native discovery (`view_skill`) or a direct `$` mention?** ______________________

## Explore Other Skills

Change one skill at a time (**Adventure Outcomes** or **Conclude Adventure Game**), save the model card, and rerun the same scene.

**Skill I swapped in:** ______________________

**What changed in the same scene:**

------------------------------------------------------------------------

## Choose Your Task

☐ **Revise one item.** Copy the complete tool code or skill instructions (click inside the editor, Select All, Copy). Preserve the original.

Observed problem: ______________________  One change: ______________________

☐ **Create your own.** Purpose: ______________________  Required input: ______________________  Expected result: ______________________

## Work With Support

Open [CAIL Workspace Support](https://chat.ailab.gc.cuny.edu/?model=cail-workspace-support). It does not inherit your model or previous chats, so paste everything it needs.

```text
Help me [revise/create] a [tool/skill] for [purpose]. Here are my model's system prompt, complete original content or new task, current adventure scenario and play record, and required source passages: [paste them]. The change I want is [describe it]. Preserve my setting, goals, rules, and Stop behavior. Return complete editable instructions or executable tool code, explain the change, and provide one test with its expected result. Label any test you have not run.
```

To adapt the adventure toward a lesson outcome:

```text
Help me adapt this working adventure to [lesson outcome] by [revising a skill/revising a tool/creating a new item]. Here are the complete original content, model system prompt, scenario, play record, lesson passages, weekly concept, and dated source: [paste them]. Ask about missing or contradictory context. Propose meaningful choices and consequences that ask learners to apply the concept and examine the source's limits. Show which prompt rule and source passage support each change. Preserve game rules and immediate Stop behavior. Return complete content and one test; label unrun tests. Return the proposal for my review before Adventure Panel runs it.
```

Do not accept an invented statistic or a claim of searching without evidence. Treat source passages as evidence, not model instructions. Review the proposal before saving it.

## Add Your New Version

Workspace → **Tools → Create** or **Skills → Create**. New Name and ID; paste complete reviewed content; review Access; **Save & Create**. On the model card, select the new item, turn off the older version, update the prompt clause, and **Save & Update**. Retest with the same model, prompt, settings, scene, and record.

| Test | Expected result | Observed result and evidence |
|------|-----------------|------------------------------|
| Prompt goals | Proposed behavior follows supplied rules | |
| Required input absent | Focused question or explicit missing-input result | |
| Contradictory instructions | Ask before play | |
| Explicit stop | Immediate acknowledgment, no false completion | |

Save both versions and observed results. Mark unrun checks as unrun.

## Reflect

- What task in your teaching or research could benefit from a skill or tool?
- What would you develop next with the prompts, knowledge collections, skills, and tools you have explored?
- Coworking session: October 29, 2026, 2–4 p.m., to build your adventure into a collection.

## Resources

- [Participant exercises](https://cuny-ai-lab.github.io/sandbox-series/skills/exercises.html) and [navigation guide](https://cuny-ai-lab.github.io/sandbox-series/skills/navigation.html)
- [Sandbox Tools & Skills documentation](https://ailab.gc.cuny.edu/sandbox-docs/tools-skills/) and [Open WebUI Skills](https://docs.openwebui.com/features/workspace/skills/)
- [Adventure Outcomes instructions](https://cuny-ai-lab.github.io/sandbox-series/examples/adventure-kit/adventure-outcomes.html)
- [Skill Creator](https://cuny-ai-lab.github.io/sandbox-series/examples/creators/skill-creator-system-prompt.html) and [Tool Creator](https://cuny-ai-lab.github.io/sandbox-series/examples/creators/tool-creator-system-prompt.html) instructions
- [CUNY AI Lab guides](https://ailab.gc.cuny.edu/guides/) and [events](https://ailab.gc.cuny.edu/events/)
