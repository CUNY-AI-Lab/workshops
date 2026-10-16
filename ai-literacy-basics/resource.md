# AI Literacy Basics

**Companion Worksheet**

*Use this sheet during the Teach@CUNY Summer Institute session to record your algorithm, your model comparison, and what a system prompt changed.*

## Icebreaker: An Algorithm You Already Know

In three steps or less, describe something you do in your everyday life and frame it as a conditional, a loop, or a sequence.

☐ Conditional (If X then Y) ☐ Loop (Repeat until done) ☐ Sequence (First A then B)

1. ______________________
2. ______________________
3. ______________________

## What Is a Large Language Model?

A model that predicts the next token: **tokens** (text splits into pieces) → **vectors** (pieces map to numbers) → **attention** (context gets weighted) → **probabilities** (next tokens get scores) → **output** (one token appears, then it repeats).

**A prompt is an algorithm you hand the model.** What clear steps, conditions, and finish line would you give it for a task in your course?

------------------------------------------------------------------------

## Discussion: Revisiting the Digital Divide

Who gets access to AI tools, and under what conditions? How does this shape AI literacy?

------------------------------------------------------------------------

## Activity 1: Model Comparison

Open [chat.ailab.gc.cuny.edu](https://chat.ailab.gc.cuny.edu/), sign in, open a new chat, and choose two models from the model menu. Run this prompt in each:

```text
The car wash is 50 yards away. Do I walk or do I drive?
```

| | Model A: __________ | Model B: __________ |
|---|---|---|
| Its recommendation | | |
| What it paid attention to | | |
| What it assumed | | |

**Debrief**

- **Notice:** what did each model pay attention to?
- **Missing:** what did one response assume that another questioned?
- **Teach:** where could this help students read an AI answer more carefully?
- **Try:** what would you change in the next prompt?

------------------------------------------------------------------------

## Activity 2: Set a System Prompt

Open **Controls** and paste this into **System Prompt**:

```text
Read input twice. Do not jump to conclusions.
```

Send the same car-wash question again.

**What changed in the response?**

------------------------------------------------------------------------

**Did the model ask about purpose, or explain its assumptions, before answering?** ☐ Yes ☐ No

**Write your own two-sentence system prompt for a task in your course:**

------------------------------------------------------------------------

## Debrief

- How can students learn by comparing responses and writing system prompts?
- How could this help students read AI output more critically?
- Could you see yourself applying these sorts of activities in your classes? If so, how?

------------------------------------------------------------------------

## Resources

- [CUNY AI Lab](https://ailab.gc.cuny.edu/) · [Sandbox](https://chat.ailab.gc.cuny.edu/) · [Tools](https://tools.ailab.gc.cuny.edu/)
- [github.com/cuny-ai-lab](https://github.com/cuny-ai-lab) · [cuny-ai-lab.github.io/links](https://cuny-ai-lab.github.io/links/)
- [Workshop slides](https://cuny-ai-lab.github.io/ai-literacy-basics/)
