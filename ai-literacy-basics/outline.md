# AI Literacy Basics - Workshop Outline

## Workshop Information

**Title:** AI Literacy Basics
**Date:** Tuesday, May 26, 2026
**Venue:** Teach@CUNY Summer Institute 2026, CUNY Graduate Center
**Format:** Hands-on session with two activities and debriefs
**Facilitators:** Zach Muhlbauer & Stefano Morello (CUNY AI Lab)

**Learning Objectives:**
- Connect everyday algorithmic thinking to how a model builds an answer
- Explain at a basic level how a large language model predicts the next token
- Compare the same prompt in two models and describe what each attended to and assumed
- Set a system prompt and compare responses with and without it
- Consider classroom uses of comparison and system-prompt writing

## Detailed Agenda

### Workshop Agenda

1. Start with an everyday algorithm
2. Compare two model responses
3. Set one system prompt
4. Test and discuss

### Icebreaker: Describe an Algorithm You Already Know

Write a routine in three steps or fewer:

- **If X then Y (conditional):** "If it's raining, grab an umbrella; otherwise, wear sunglasses."
- **Repeat until done (loop):** wash the dishes step by step until the sink is empty.
- **First A then B (sequence):** preheat the oven, mix the batter, pour it into a pan, then bake.

**Prompt:** In three steps or less, describe something you do in your everyday life and frame it as a conditional, a loop, or a sequence.

### The Bridge: Why Start with an Algorithm?

Algorithmic thinking is how you'll make sense of AI.

- A model builds an answer one step at a time, the same sequence logic you just used
- Seeing it as a procedure makes the model less mysterious, and easier to question
- A prompt is an algorithm you hand the model: clear steps, conditions, a finish line

Two payoffs: **demystify** (see the model as steps, not magic) and **prompt better** (give it clear steps and conditions).

### Concept: What Is a Large Language Model?

A model that predicts the next token.

| Step | What happens |
|------|--------------|
| 01 Tokens | Text splits into pieces |
| 02 Vectors | Pieces map to numbers |
| 03 Attention | Context gets weighted |
| 04 Probabilities | Next tokens get scores |
| 05 Output | One token appears, then the process repeats |

Key terms: token (piece of text), vector (token as numbers), attention (weighted context), prediction (likely next token).

### Discussion Prompt: Revisiting the Digital Divide

Who gets access to AI tools, and under what conditions? How does this shape AI literacy?

### Sandbox Setup: Access the Sandbox

Start with a fresh chat.

1. Open chat.ailab.gc.cuny.edu
2. Sign in with your CUNY account
3. Open a new chat
4. Find the model menu and controls (the Controls panel holds the System Prompt field above advanced settings)

### Activity 1: Model Comparison

> The car wash is 50 yards away. Do I walk or do I drive?

1. Open the model selector
2. Choose two available models
3. Run the same prompt with each model
4. Evaluate responses across models

Illustrative contrast: Model A, "Walk. Fifty yards is close," treats distance as the whole question. Model B, "Drive if you are washing the car. Walk if you are just going there," notices that purpose changes the answer.

### Activity 1 Debrief: What Did the Comparison Show?

1. **Notice:** what did each model pay attention to?
2. **Missing:** what did one response assume that another response questioned?
3. **Teach:** where could this help students read an AI answer more carefully?
4. **Try:** what would you change in the next prompt?

### System Prompts: What Is a System Prompt?

Setup instructions for a language model, set before the chat: what task it handles, how it should operate, what guardrails to follow, what's out of scope. Example: a system prompt that says "You are a writing scaffold..." shapes the reply to a student's "I'm stuck on my intro" into "What's the main argument you want your reader to encounter first?" The system prompt shapes the response across the conversation.

### Activity 2: Set a System Prompt

**System prompt (in Controls):**

```text
Read input twice. Do not jump to conclusions.
```

**User prompt:**

> The car wash is 50 yards away. Do I walk or do I drive?

Compare with the Activity 1 responses.

### Activity 2 Debrief: Discussion Questions

- How can students learn by comparing responses and writing system prompts?
- How could this help students read AI output more critically?
- Could you see yourself applying these sorts of activities in your classes? If so, how?

### Resources

- CUNY AI Lab: [ailab.gc.cuny.edu](https://ailab.gc.cuny.edu/)
- CUNY AI Lab Sandbox: [chat.ailab.gc.cuny.edu](https://chat.ailab.gc.cuny.edu/)
- AI tools for research, teaching, and creative work: [tools.ailab.gc.cuny.edu](https://tools.ailab.gc.cuny.edu/)
- Open-source projects and workshop code: [github.com/cuny-ai-lab](https://github.com/cuny-ai-lab)
- Examples, projects, workshops, and resources: [cuny-ai-lab.github.io/links](https://cuny-ai-lab.github.io/links/)
- Workshop slides: [cuny-ai-lab.github.io/ai-literacy-basics](https://cuny-ai-lab.github.io/ai-literacy-basics/)

## Materials Needed

- Laptop/projection for demos
- Participant access to the CUNY AI Lab Sandbox with CUNY sign-in
- The car-wash prompt and the two-sentence system prompt, ready to paste
