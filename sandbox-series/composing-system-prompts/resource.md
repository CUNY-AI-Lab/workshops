# Composing System Prompts (Fall 2026)

**Companion Worksheet**

*Use this sheet during Session 1 of the Sandbox Workshop Series. Keep your inputs, model IDs, and responses so you can compare them later.*

## Definitions

| Term | What it means |
|------|---------------|
| **System prompt** | Setup instructions that describe how a model should behave |
| **User prompt** | Questions or tasks you enter in chat |
| **Custom model** | A base model (such as Gemma) plus instructions and documents for it to use |

## Compare Models

Open the model selector at the bottom right of the message box, select **Compare**, and choose two models.

**Model A:** ______________________  **Model B:** ______________________

### Who Was Late?

```text
The nurse yelled at the doctor because she was late. Who was late?
```

Either person could be late. Which person does each model choose, and what assumption supports its answer?

| | Model A | Model B |
|---|---|---|
| Who it says was late | | |
| Assumption it relies on | | |
| Does it acknowledge ambiguity? | | |

### Going to the Car Wash

```text
The car wash is 50 meters from me. Should I walk or take the car? Explain your reasoning.
```

What do you think this person wants to accomplish?

------------------------------------------------------------------------

## Add System Prompt

Select **Controls** at the top right of chat. Paste these instructions into **System Prompt**, then close Controls:

```text
Identify purpose and separate facts from assumptions. Ask one clarifying question when needed. Answer concisely.
```

Select **Regenerate** beneath each original response, then **Try Again**. Keep your question, models, and other settings unchanged.

| Criterion | Model A evidence | Model B evidence |
|-----------|------------------|------------------|
| Identifies the stated goal or acknowledges a missing purpose | | |
| Distinguishes stated facts from assumptions | | |
| Gives reasons that support its recommendation | | |
| Changes after the system prompt instructions were added | | |

**What changed in each answer after you added the instructions?**

------------------------------------------------------------------------

## Try, Clone, and Compare

Choose one example: [STEM Adventure Games](https://chat.ailab.gc.cuny.edu/?model=stem-adventure-games) (teaching) or [Compare Wikipedia Edits](https://chat.ailab.gc.cuny.edu/?model=compare-wikipedia-revisions) (research). Open its settings and find **Purpose, Procedure, Constraints, and Format** in its system prompt.

**Which instruction explains something you noticed in its response?**

------------------------------------------------------------------------

**Clone it:** Workspace → Models → ⋯ → Clone. Rename your copy, revise **one** instruction, keep the base model and other settings unchanged, and select **Save & Create**.

**The instruction I revised (before → after):**

------------------------------------------------------------------------

**Compare:** New chat → model selector → Compare → original and copy, same request.

- What did you change?
- Did your intended revision prove effective?
- How could you imagine testing custom models like this in the future?

------------------------------------------------------------------------

## Draft Your Own System Prompt

```text
Purpose
What should your model help you accomplish?

Procedure
What steps should it follow?

Constraints
What limits should it observe?

Format
How should it present responses?
```

**Purpose:**

------------------------------------------------------------------------

**Procedure:**

------------------------------------------------------------------------

**Constraints:**

------------------------------------------------------------------------

**Format:**

------------------------------------------------------------------------

**Create it:** Workspace → Models → Create. Name it, choose a base model, paste your draft into System Prompt, Save & Create, and try one request.

**Model name and base model:** ______________________

## Before the Next Session

Keep your draft. Choose the source documents you want your model to draw on for **Curating Knowledge Collections** (October 1, 2026). Use documents you are permitted to upload and share.

## Resources

- [Sandbox documentation](https://ailab.gc.cuny.edu/sandbox-docs/) (Getting Started, Basic Concepts, Custom Models)
- [Open WebUI Models](https://docs.openwebui.com/features/workspace/models/)
- [Model Registry](https://ailab.gc.cuny.edu/models/) and [monthly usage](https://tools.ailab.gc.cuny.edu/model-access)
- [Full workshop copy](https://cuny-ai-lab.github.io/sandbox-series/basics/workshop-copy.html)
