# Curating Knowledge Collections (Fall 2026) - Workshop Outline

## Workshop Information

**Title:** Curating Knowledge Collections
**Date:** Thursday, October 1, 2026, 2:30–4:00 p.m.
**Location:** New Media Lab, Room 7388.01, CUNY Graduate Center
**Duration:** 90 minutes
**Format:** Hands-on workshop (Session 2 of the Sandbox Workshop Series; can be taken independently)
**Facilitators:** Zach Muhlbauer and Meha Gupta (CUNY AI Lab)

**Learning Objectives:**
- Explain retrieval-augmented generation and what it means for how sources are organized
- Clone a custom model and inspect the knowledge collection it uses
- Create a private knowledge collection with source excerpts, secondary and heuristic sources, and an instructions file
- Revise a system prompt so the model consults the instructions file before retrieving passages
- Test a grounded model by checking citations, comparing with the original, and revising one source or instruction

## Preparation

- Confirm Workspace and Knowledge collection access for participants, including a non-admin check that directory creation and Add text content work.
- Settings are prepared on the example model before participants clone it. STEM Adventure Games uses its chat-only system prompt with the **STEM Wikipedia Experiments** collection attached; Skills and Tools stay unselected. The participant deck does not walk through Function Calling, Advanced Params, or capability switches.
- Show the original collection before the customization activity. Newly created collections contain no sources until participants add text. Cloning does not create personal copies of shared sources; participants replace the inherited attachment with their own collection.
- Use documents you are permitted to upload and share. Verify sharing through an ordinary participant account.

## Lesson Plan

| Minutes | Activity | Evidence to examine |
|---------|----------|---------------------|
| 0–15 | Introduce RAG, explore STEM Adventure Games, clone and rename it, and try an initial interaction. | Saved copy and an initial response |
| 15–40 | View the example collection. Choose a purpose and audience, then locate Wikipedia pages for an adapted version. Read relevant passages and keep the URLs. | Participant-selected pages and intended use for each |
| 40–60 | Create a private collection and a Wikipedia directory. Use Add text content to paste substantial excerpts and source URLs into separate files. Check saved text, then create instructions.txt at the collection root with directions for using each source. | Excerpt files with source links and instructions.txt |
| 60–70 | Attach the new collection to the clone. Edit Purpose and Audience, then replace source and retrieval directions above the numbered game steps with directions to consult instructions.txt. Retain numbered steps, Constraints, and Format, and save. | Prompt instructions that match the new source material |
| 70–90 | Start a blank chat, select the saved copy, and choose an adventure. Check citations. Open the original in another tab to compare the same opening request. Revise one source file or instruction, save, then test the copy in a new chat. | Source-supported details, gaps, and effects of customization |

## Detailed Agenda

### Workshop Agenda (slide)

- Explore and clone · 15 minutes
- Select new sources · 25 minutes
- Create and populate collections · 20 minutes
- Revise system prompts · 10 minutes
- Test and revise · 20 minutes

### Retrieval-Augmented Generation

A Knowledge collection contains documents a custom model can search. **RAG** combines information retrieval with text generation: it retrieves relevant source passages and adds them to a model's context alongside your request and system prompt instructions. **Search documents → Retrieve passages → Generate response.**

**Under the hood.** Processing documents: **Parse** (extract usable text), **Chunk** (divide text into smaller passages), **Embed** (represent passages numerically so they can be searched by similarity). Responding to requests: **Retrieve** (search for relevant passages), **Add context** (append passages to prompt instructions), **Generate** (produce a response using that context).

### Explore and Clone STEM Adventures

**STEM Adventure Games** uses source documents to guide a text adventure with numbered choices. Select **Workspace → Models**, search for STEM Adventure Games, open ⋯ and select **Clone**. Give your copy a unique name and model ID; base model, system prompt, and settings carry over. Scroll to the bottom and select **Save & Create**.

Open **New Chat**, select the original STEM Adventure Games, ask for four adventure options, choose one, and try its numbered choices. Ask for another menu to see new options.

### Example Sources

Select **Workspace → Knowledge** and open **Sandbox Workshop Collection**. At its root, **instructions.txt** describes how sources guide play. The **Wikipedia** directory contains three article files (Women-in-science.txt, Scientific-method.txt, List-of-experiments.txt), each with its text and source link. For your adapted version, start with one article and add more as needed.

### Choose Purpose and Find Sources

What should players learn or explore? Choose a topic and audience for your adaptation. Identify a question players could investigate through their choices. Start with one Wikipedia article about the topic; choose substantial passages that give players something to investigate.

### Create Your Collection

Select **Workspace → Knowledge → Create**. Name your collection and describe what your sources cover. Keep access **Private** and select **Create Knowledge**.

### Add Source Text

Select **Add Content → New directory**, name it **Wikipedia**, select **Create**, then open it. Select **Add Content → Add text content**. Use the article title as the filename. Copy and paste several paragraphs or complete sections, including the article link. Select **Save**. Keep additional articles in separate files with their links. Wait for processing, then open each file to check its text.

### Add Source Guidance

Before testing, add two short sources alongside the Wikipedia material, in separate, clearly named files at the collection root:

- **Secondary source** - an explanation or analysis that helps interpret your topic
- **Heuristic source** - questions or rules of thumb that guide player decisions

### Add Instructions

Return to the collection root. Select **Add Content → Add text content** and enter **instructions** as the title (the Sandbox adds .txt). Use your page titles and filenames to explain which material grounds scenes, which helps interpret them, and which guides player choices. Select **Save**.

In **Workspace → Models**, open **⋯ → Edit** beside your saved copy. Under **Knowledge**, replace STEM Wikipedia Experiments with your own collection. In **System Prompt**, revise **Purpose** and **Audience** for your topic. Under **Procedure**, replace the source and retrieval directions above the numbered steps with:

> Offer four adventure options immediately. After a player chooses, retrieve instructions.txt from the attached Knowledge collection and use its directions to find relevant source passages. Use article passages for details, secondary sources for interpretation, and heuristic sources for questions or decision rules during play.

Remove instructions that refer to sources you replaced, including any one-retrieval-call limit. Keep the numbered game steps, **Constraints**, and **Format**. Select **Save & Update**.

### Test, Check Citations, Compare

Select **New Chat**, choose your saved copy, ask for four adventure options about your topic, and choose one. In the same chat ask, "Which passage supports this scene? Quote it and cite your source." Select a citation beside a response: does its source passage support the response? Open the original STEM Adventure Games in another tab and send the same opening request. How do responses differ? Does your copy use new sources as instructed?

### Revise and Retest

Choose one problem you observed. Revise source guidance or system prompt instructions; add another article only if needed. For source changes, update the excerpts and instructions.txt and wait for processing. For prompt changes, select **Save & Update**. Open a new chat, select your copy, and repeat your request. Did the change resolve the problem?

### Share Custom Model

In your copy's editor, open **Access** and grant intended users or groups **Read** access. Give those same users Read access to its Knowledge collection. Ask someone to try your copy and check its citations.

### Parting Questions

- How else could you see yourself using knowledge collections in the future?
- What are the limitations of this approach?

### Next Steps

- Choose another topic or experiment
- Update copied excerpts and instructions
- Check responses against saved sources
- Next session introduces tools that retrieve Wikipedia content live

## Materials Needed

- Projection and a presenter account with Workspace Models and Knowledge access
- Participant access to the Sandbox with Workspace and Knowledge collection permissions
- The shared STEM Adventure Games model and Sandbox Workshop Collection with Read access for participants
- The replacement Procedure paragraph, ready to paste
