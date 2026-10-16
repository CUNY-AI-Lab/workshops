# Curating Knowledge Collections (Fall 2026)

**Companion Worksheet**

*Use this sheet during Session 2 of the Sandbox Workshop Series. Record your sources, your instructions file, and what each test showed.*

## How Retrieval Works

| Stage | Step | What happens |
|-------|------|--------------|
| Processing documents | **Parse** | Extract usable text from files |
| | **Chunk** | Divide text into smaller passages |
| | **Embed** | Represent passages numerically so they can be searched by similarity |
| Responding to requests | **Retrieve** | Search for passages relevant to a request |
| | **Add context** | Append passages to prompt instructions |
| | **Generate** | Produce a response using that context |

## Step 1: Clone STEM Adventure Games

Workspace → Models → search **STEM Adventure Games** → ⋯ → **Clone**. Give your copy a unique name and model ID, then **Save & Create**.

**My copy's name and model ID:** ______________________

**Opening request I tried, and what happened:**

------------------------------------------------------------------------

## Step 2: Choose Purpose and Find Sources

**Topic:** ______________________  **Audience:** ______________________

**A question players could investigate through their choices:**

------------------------------------------------------------------------

Start with one Wikipedia article. Add more only as needed.

| File name (article title) | URL | What it grounds |
|---------------------------|-----|-----------------|
| | | |
| | | |

## Step 3: Create and Populate Your Collection

Workspace → Knowledge → **Create** (keep access **Private**) → Add Content → **New directory** "Wikipedia" → Add Content → **Add text content**. Paste several paragraphs or complete sections with the link, then **Save**. Wait for processing and open each file to check.

**Collection name:** ______________________

**Secondary source** (explanation or analysis that helps interpret your topic):

File: __________________  Source: __________________

**Heuristic source** (questions or rules of thumb that guide player decisions):

File: __________________  Source: __________________

## Step 4: Write instructions.txt

At the collection root, Add Content → Add text content, title **instructions**. Use your filenames to say which material grounds scenes, which helps interpret them, and which guides player choices.

**Draft:**

------------------------------------------------------------------------

------------------------------------------------------------------------

## Step 5: Revise the System Prompt

Workspace → Models → ⋯ → **Edit** your copy. Under **Knowledge**, replace STEM Wikipedia Experiments with your collection. Revise **Purpose** and **Audience**. Replace the source and retrieval directions above the numbered steps with:

```text
Offer four adventure options immediately. After a player chooses, retrieve instructions.txt from the attached Knowledge collection and use its directions to find relevant source passages. Use article passages for details, secondary sources for interpretation, and heuristic sources for questions or decision rules during play.
```

Remove instructions that refer to sources you replaced. Keep the numbered game steps, Constraints, and Format. **Save & Update**.

## Step 6: Test

New Chat → select your copy → ask for four adventure options about your topic → choose one.

**Check citations.** In the same chat ask:

```text
Which passage supports this scene? Quote it and cite your source.
```

Select the citation beside the response. Does its source passage support the response?

------------------------------------------------------------------------

**Compare.** Send the same opening request to the original [STEM Adventure Games](https://chat.ailab.gc.cuny.edu/?model=stem-adventure-games) in another tab.

| | Original | My copy |
|---|---|---|
| Opening options offered | | |
| Details drawn from sources | | |
| Citations shown | | |

**Does your copy use new sources as instructed?**

------------------------------------------------------------------------

## Step 7: Revise and Retest

**One problem I observed:**

------------------------------------------------------------------------

**What I changed (source file, instructions.txt, or system prompt):**

------------------------------------------------------------------------

**Did the change resolve it?** ☐ Yes ☐ Partly ☐ No

## Step 8: Share

In your copy's editor, open **Access** and grant intended users or groups **Read** access. Give the same users Read access to the Knowledge collection.

## Parting Questions

- How else could you see yourself using knowledge collections in the future?
- What are the limitations of this approach?

## Resources

- [Sandbox Knowledge documentation](https://ailab.gc.cuny.edu/sandbox-docs/knowledge-bases/) and [Open WebUI Knowledge](https://docs.openwebui.com/features/workspace/knowledge/)
- [Sandbox Roles & Permissions](https://ailab.gc.cuny.edu/sandbox-docs/roles-permissions/)
- [Full workshop copy](https://cuny-ai-lab.github.io/sandbox-series/knowledge/workshop-copy.html)
- [Monthly usage](https://tools.ailab.gc.cuny.edu/model-access)
