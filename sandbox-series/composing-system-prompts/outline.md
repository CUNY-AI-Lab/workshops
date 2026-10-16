# Composing System Prompts (Fall 2026) - Workshop Outline

## Workshop Information

**Title:** Composing System Prompts
**Date:** Thursday, September 17, 2026, 2:30–4:00 p.m.
**Location:** New Media Lab, Room 7388.01, CUNY Graduate Center
**Duration:** 90 minutes
**Format:** Hands-on workshop (Session 1 of the Sandbox Workshop Series)
**Facilitator:** Zach Muhlbauer (CUNY AI Lab)

**Learning Objectives:**
- Distinguish system prompts, user prompts, and custom models
- Compare two models on the same input and describe the assumptions each makes
- Add in-chat system prompt instructions and regenerate responses
- Clone a shared custom model, revise one instruction, and compare it with the original
- Draft a system prompt using Purpose, Procedure, Constraints, and Format, and save a configuration

## Preparation

- Confirm participants have individual Sandbox access and Workspace Models access before the cloning and creation exercises.
- Choose two available models for the opening demonstration. Record their exact identifiers and settings rather than treating screenshot labels as a current inventory.
- Check personal defaults, folder instructions, memory, and optional features that may add context. Keep these consistent during comparisons.
- Prepare the **Examine Assumptions** instructions (the short system prompt below) with a tested base model.
- Configure **STEM Adventure Games** with its chat-only system prompt (no skills or tools attached) and confirm **Compare Wikipedia Edits** is shared with participants.

## Lesson Plan

| Minutes | Activity | Evidence to retain |
|---------|----------|--------------------|
| 0–5 | Introduce yourselves: name, pronouns, role at CUNY, and what brings you to this workshop. | Workshop interests |
| 5–10 | Review access requests and sign-in, define system prompts, and locate the model selector. | Account readiness and prompt distinction |
| 10–25 | Demonstrate models on the nurse question and car-wash question. Examine assumptions before showing the saved responses. | Exact inputs, model IDs, and responses |
| 25–45 | Compare the car-wash responses, paste the short in-chat system prompt, then choose Regenerate → Try Again on each original response. Keep the question and other settings unchanged. | Original and regenerated responses |
| 45–52 | Choose one example, try it in chat, and review its system prompt and base model. | Original request and instruction to revise |
| 52–65 | Follow the Clone screenshot, revise one instruction, save, and test the copy in a new chat. | Original and revised instruction |
| 65–75 | Discuss what you changed, whether your revision was effective, and how you might test custom models in future work. | Both responses and evidence of change |
| 75–85 | Draft original instructions using Purpose, Procedure, Constraints, and Format. Select Create in Workspace Models, choose a base model, add the draft, and save. Try one request if time remains. | Original system prompt and saved configuration |
| 85–90 | Review workshop resources and choose source documents to bring to the next workshop. | Draft prompt, model configuration, and source documents |

## Detailed Agenda

### Workshop Agenda (slide)

- Introduce yourselves
- Request access and sign in
- Compare model outputs
- Revise system prompts
- Create custom models

Check monthly usage at [Model Access](https://tools.ailab.gc.cuny.edu/model-access).

### Sandbox Access

**Request access:** Open the [access application](https://ailab.gc.cuny.edu/request-access/). Choose **My own access** and sign in with **CUNY Login**. Enter your details and intended use, complete verification, and select **Submit Application**. Watch your verified CUNY email for approval.

**Sign in:** Open the [Sandbox](https://chat.ailab.gc.cuny.edu/). Select **Continue with CUNY Login**, enter your CUNY credentials, and complete two-factor authentication if prompted. No API key is needed for these chat exercises.

### Definitions

- **System prompts** are setup instructions that describe how a model should behave.
- **User prompts** are questions or tasks you enter in chat.
- **Custom models** are created by choosing a base model, such as Gemma, and adding instructions and documents for it to use.

### Chat Features

- **Upload Files (+):** attach images, PDFs, or documents.
- **Integrations:** enable tools that perform operations and skills that give reusable instructions.
- **Message actions:** beneath each response, copy, edit, or regenerate it; open More (⋯) for additional actions.

### Select and Compare Models

Find the model selector at the bottom right of the message box, then select Gemma 4 26B A4B IT. Reopen the selector and select **Compare** beside the search field. Choose Gemma and another model, such as Mistral Large 3.

### Who Was Late?

> The nurse yelled at the doctor because she was late. Who was late?

Send exactly this question to both models with matching context. Either person can be the referent of "she"; the sentence does not establish a unique answer. Ask which interpretation each response chooses and whether it acknowledges ambiguity. A plausible interpretation differs from information established by the wording. Avoid turning this single item into a claim about model-wide bias or ability.

**Winograd Schema Challenge:** this challenge tests how models interpret ambiguous pronouns using context and common-sense reasoning (Levesque, Davis, and Morgenstern, 2012).

### Going to the Car Wash

> The car wash is 50 meters from me. Should I walk or take the car? Explain your reasoning.

Ask "What do you think this person wants to accomplish?" Show the archival Gemma 3 27B response (recommending walking) and Qwen3.5 27B response (recommending driving) without treating screenshot labels or timings as reliable model identifiers or comparative measurements. Then participants start a new chat, select two models, and send the question themselves.

### Add System Prompt

Select **Controls** at the top right of chat. Paste these instructions into **System Prompt**, then close Controls:

```text
Identify purpose and separate facts from assumptions. Ask one clarifying question when needed. Answer concisely.
```

Select **Regenerate** beneath each original response, then choose **Try Again**. Keep the original question, selected models, and other settings unchanged.

### Debrief Questions

- What changed in each model's answer to your car wash question after you added system prompt instructions?
- Did either model ask about your purpose or explain its assumptions before recommending walking or driving?

### Try Examples

Choose one example and experiment with it in chat:

- **Teaching:** [STEM Adventure Games](https://chat.ailab.gc.cuny.edu/?model=stem-adventure-games) explores scientific experiments through a text adventure with numbered choices.
- **Research:** [Compare Wikipedia Edits](https://chat.ailab.gc.cuny.edu/?model=compare-wikipedia-revisions) compares Wikipedia revisions and examines changes in wording, claims, and citations.

Review **Base Model** and **System Prompt** for your chosen example. Find Purpose, Procedure, Constraints, and Format in its instructions. Which instruction explains something you noticed in its response?

### Clone Models

Select **Workspace** in the left sidebar, then **Models**. Open ⋯ beside your chosen example and select **Clone**.

- Rename your copy.
- Revise one instruction in **System Prompt**; keep **Base Model** and other settings unchanged.
- Scroll to the bottom and select **Save & Create**.
- Open your copy in a new chat and repeat your original request.

### Compare Configurations

Start a new chat. Select the model ID at the bottom right of the message box, then **Compare**. Choose your original model and your copy.

- What did you change?
- Did your intended revision prove effective?
- How could you imagine testing custom models like this in the future?

### Draft System Prompts

Use the remaining time to begin drafting instructions for your own teaching or research task:

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

### Create Models

Select **Workspace → Models → Create**. Name your configuration, select **Base Model**, paste your draft into **System Prompt**, scroll to the bottom and select **Save & Create**. Start a new chat with your model and try one request.

### Workshop Resources

Keep your draft and choose source documents for the next workshop. Resources: the full workshop copy, [Sandbox documentation](https://ailab.gc.cuny.edu/sandbox-docs/), [Open WebUI Models](https://docs.openwebui.com/features/workspace/models/), the [Model Registry](https://ailab.gc.cuny.edu/models/), [monthly usage](https://tools.ailab.gc.cuny.edu/model-access), and [AI Lab guides](https://ailab.gc.cuny.edu/guides/).

## Materials Needed

- Projection and a presenter account with Workspace Models access
- Participant access to the CUNY AI Lab Sandbox (chat.ailab.gc.cuny.edu)
- Shared example models (STEM Adventure Games, Compare Wikipedia Edits) with Read access for participants
- The short in-chat system prompt and the Purpose/Procedure/Constraints/Format template, ready to paste
