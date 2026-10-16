# Slide Index: Critical Play with Large Language Models

> Slide index for the CUNY AI Lab archive copy of this workshop (Thursday, October 16, 2025). Source: [zmuhls/critical-play](https://github.com/zmuhls/critical-play) and [CUNY-AI-Lab/critical-play](https://github.com/CUNY-AI-Lab/critical-play).

A slide-by-slide reference for the Reveal.js workshop deck (`index.html`).

---

## Slide 1 — Title

- **Section:** Intro
- **Timing:** 1 min
- **Content:** Workshop title, date (Thursday, October 16, 2025), facilitator (Zach Muhlbauer), affiliation (Teaching and Learning Center | Interactive Technology & Pedagogy Lab)
- **Visualization:** Animated network graph canvas

---

## Slide 2 — Welcome and Introductions

- **Section:** Intro
- **Timing:** 10 min
- **Content:** Icebreaker prompts — name and pronouns, field of study or work, a favorite game played with family, friends, or students
- **Visualization:** Retro arcade game canvas

---

## Slide 3 — Game Mechanics as Analytical Scaffolds

- **Section:** Demo
- **Timing:** 10 min
- **Content:** Framing game mechanics as tools that reveal AI limitations in situ. Example: Chess.com blogger "Nightly-Knight" played against ChatGPT, which repeatedly made illegal moves (e.g., moving a pawn horizontally to capture). ChatGPT "forgets the position of the game" and violates basic chess rules rather than accepting disadvantageous positions.
- **Visualization:** Chess board canvas showing illegal move attempts

---

## Slide 4 — Jeopardy! Board Emulator (vertical stack, 3 sub-slides)

### 4a — Jeopardy! Board Emulator Overview

- **Section:** Demo
- **Content:** Introduction to the interactive Jeopardy! emulator. The format requires the LLM to generate coherent categories, sliding difficulty levels, and factual clues — making confabulation immediately visible when it fails.

### 4b — Prompting AI-generated Jeopardy! Board

- **Section:** Demo
- **Content:** Link to the live demo at zmuhls.github.io/jeopardy-lm. Three category types to progressively stress the model's knowledge boundaries: (1) simple category for an accurate baseline, (2) obscure real category for mixed results, (3) fictitious category as a confabulation trigger.

### 4c — Debrief Discussion

- **Section:** Demo
- **Content:** Chat-based debrief. Prompts: what did you notice from the demonstration? What was most striking? What other games offer similar affordances for exposing LLM limitations?
- **Image:** Screenshot of the Jeopardy board interface (`img/jeopardy-board.png`)

---

## Slide 5 — Critical Play with Mary Flanagan

- **Section:** Playful
- **Content:** Mary Flanagan's "critical play" framework — using game design to challenge conventions and reveal hidden systems, applied here to expose AI limitations through playful constraints. Traditional iterative game design model: set a design goal, develop rules, develop playable prototype, playtest, revise goal, repeat.
- **Image:** Iterative game design model diagram (`img/design-model.png`)

---

## Slide 6 — Playful Interactions with LLMs

- **Section:** Playful
- **Content:** Taxonomy of six playful interaction types drawn from Petridis et al. (2023) study of r/ChatGPT:

| Type | What it does | Try this |
|------|-------------|----------|
| Reflecting | Prompting AI to self-represent and express "opinions" | Ask about self-understanding |
| Jesting | Generating humor and nonsensical exchanges | Request absurd combinations |
| Imitating | Requesting persona or character mimicry | Ask it to role-play |
| Challenging | Testing capabilities until failure | Push logical limits |
| Tricking | Attempting deception/boundary bypassing | Try jailbreak techniques |
| Contriving | Creating impossible or fabricated content | Request non-existent things |

---

## Slide 7 — Quick Demo Session (vertical stack, 2 sub-slides)

### 7a — Quick Demo Session Overview

- **Section:** Demo
- **Timing:** 10 min
- **Content:** LLMs generate responses through vector similarity — finding statistically likely associations from training data. When given "teacher," the model maps to nearby concepts like "classroom," "student," "education." Poses the question: what happens when game rules constrain these associations?
- **Visualization:** Word vector semantic space canvas

### 7b — Exquisite Corpse System Prompt

- **Section:** Demo
- **Content:** Full system prompt for an Exquisite Corpse word game: respond only to the user's most recent word, reply with exactly one word per turn, label responses in sequence (Turn 2, Turn 3, etc.), continue until Turn 20, then compose a short poem using only the words from the conversation. Link to Open WebUI platform for live demo.

---

## Slide 8 — Critical Design Activity (vertical stack, 4 sub-slides)

### 8a — Critical Design Activity Overview

- **Section:** Activity
- **Timing:** 15 min
- **Content:** Participants use a linked Google Doc worksheet to design a game that reveals AI limitations using 2-3 types of playful interactions. Game format options: 20 Questions, Exquisite Corpse, Two Truths and a Lie, Word Association, Trivia/Quiz Games, Riddles/Puzzles, Chess/Game Annotation, Role Play/Improv, Debate/Argument, Mad Libs.

### 8b — Target AI Limitations

- **Section:** Activity
- **Content:** Checklist of AI weaknesses participants can target: hallucination/confabulation, logic inconsistency/reasoning failures, sycophancy (excessive agreement), instruction following failures, semantic breakdown. Includes a sycophancy example.

### 8c — Craft Your Prompts

- **Section:** Activity
- **Content:** Guidance for writing system prompts (configuring AI behavior and constraints) and user prompts (conversation starters). Includes a Mad Libs example: system prompt that asks the AI to provide both a probable word and a statistically improbable word for each blank.

### 8d — Expected Outcomes

- **Section:** Activity
- **Content:** Reflection prompts — what do you want to reveal about AI abilities/limitations? What do you predict will happen? What failure modes might emerge? How will game mechanics make limitations visible?
- **Visualization:** Domino ripple causation canvas

---

## Slide 9 — Shareback and Playtest

- **Section:** Playtest
- **Timing:** 15 min
- **Content:** Instructions for testing game designs on Open WebUI: select a model, configure system prompt, adjust optional settings (temperature, max tokens), begin with conversation starter. Share discoveries about AI limitations.

---

## Slide 10 — Resources and Q&A

- **Section:** Playtest
- **Content:** Links to interactive tools (Critical Play slides, GitHub repo, Jeopardy LM demo, Open WebUI). Full citations: Flanagan (2009) *Critical Play*, Petridis et al. (2023) on playful ChatGPT interactions, Palisade Research (2025) on AI chess cheating, Nightly-Knight chess blog post, Acher (2024) on GPTs vs. chess engines, r/ChatGPT community discussions.
