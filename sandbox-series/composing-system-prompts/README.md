# Composing System Prompts (Fall 2026)

_Session 1 of the CUNY AI Lab Sandbox Workshop Series: configure model behavior with system prompts._

Participants learn how user prompts and system prompts differ, compare how two models interpret an ambiguous sentence, add a short in-chat system prompt and regenerate their responses, then clone a shared custom model, revise one instruction, and compare the copy against the original. The session closes with each participant drafting their own instructions and saving a configuration to develop before the next workshop.

**Workshop Date:** Thursday, September 17, 2026
**Time:** 2:30–4:00 p.m. (90 minutes)
**Location:** New Media Lab, Room 7388.01, CUNY Graduate Center
**Format:** Hands-on workshop (Session 1 of 3)
**Facilitator:** Zach Muhlbauer (CUNY AI Lab)
**Required access:** Individual Sandbox access and sign-in; Workspace Models access for cloning and creation

_This session was originally conducted as part of the [Sandbox Workshop Series](../) at the CUNY Graduate Center. It revises the Spring 2026 workshop [Composing System Prompts](../../system-prompting/)._

## About the CUNY AI Lab

The **CUNY AI Lab** is a faculty and staff-led incubator for experimentation with AI by CUNY researchers across disciplines, strengthening CUNY's position at the leading edge of technological innovation. Located at the CUNY Graduate Center and led by experienced scholars and technologists who have built widely used open publishing platforms, the Lab fosters momentum for AI experimentation while foregrounding ethical practices and values that reinforce CUNY's mission of accessible, equitable, and transformative education.

This workshop is part of the CUNY AI Lab's commitment to developing critical AI literacy among faculty, staff, and students across the university system.

## Overview

Two comparison prompts open the session. The first, a Winograd schema sentence about a nurse and a doctor, shows how models resolve an ambiguous pronoun. The second asks whether to walk or drive to a car wash 50 meters away, and shows how an unstated purpose shapes a recommendation. Participants then paste three sentences of instructions into the Sandbox's in-chat System Prompt field and regenerate both responses to see what changes. The second half moves to Workspace: participants try a shared example (STEM Adventure Games for teaching, Compare Wikipedia Edits for research), read its system prompt, clone it, revise one instruction, and run the original and the copy side by side. They finish by drafting instructions using Purpose, Procedure, Constraints, and Format and saving a model of their own.

## Learning Objectives

- Distinguish system prompts (setup instructions for a model) from user prompts (questions or tasks entered in chat) and from custom models (a base model plus instructions and documents)
- Compare two models on the same input and describe the assumptions each response makes
- Add in-chat system prompt instructions and regenerate responses without changing the question or settings
- Clone a shared custom model in Workspace, revise one instruction, and compare the copy with the original
- Draft a system prompt using Purpose, Procedure, Constraints, and Format, and save it as a model configuration

## Workshop Structure

1. **Introductions** - Name, pronouns, role at CUNY, and what brings you to the workshop
2. **Sandbox Access** - Request access with CUNY Login; sign in with two-factor authentication if prompted
3. **System Prompts, User Prompts, Custom Models** - Working definitions from the Sandbox documentation
4. **Chat Features** - Upload files, integrations (tools and skills), and message actions
5. **Select and Compare Models** - Find the model selector; use Compare to run two models at once
6. **Who Was Late?** - The nurse-and-doctor sentence and the Winograd Schema Challenge
7. **Going to the Car Wash** - Compare outputs; what does this person want to accomplish?
8. **Add System Prompt** - Paste short instructions into Controls, then Regenerate each response
9. **Debrief** - What changed? Did either model ask about purpose or explain its assumptions?
10. **Try Examples** - STEM Adventure Games (teaching) or Compare Wikipedia Edits (research); review Base Model and System Prompt
11. **Clone Models** - Rename the copy, revise one instruction, Save & Create, repeat the original request
12. **Compare Configurations** - Original and copy side by side; what did you change, and did it work?
13. **Draft System Prompts** - Purpose, Procedure, Constraints, Format
14. **Create Models** - Workspace → Models → Create; name, base model, draft prompt, Save & Create
15. **Workshop Resources** - Keep your draft and choose source documents for the next session

## Interactive Tools

- **[CUNY AI Lab Sandbox](https://chat.ailab.gc.cuny.edu/)** - Self-hosted chat platform with open-weight models
- **[Access application](https://ailab.gc.cuny.edu/request-access/)** - Individual access with CUNY Login
- **[Model Registry](https://ailab.gc.cuny.edu/models/)** - Models used in the session included Gemma 4 26B, Mistral Large 3, and DeepSeek V4 Flash
- **[STEM Adventure Games](https://chat.ailab.gc.cuny.edu/?model=stem-adventure-games)** - Teaching example
- **[Compare Wikipedia Edits](https://chat.ailab.gc.cuny.edu/?model=compare-wikipedia-revisions)** - Research example
- **[Model Access](https://tools.ailab.gc.cuny.edu/model-access)** - Monthly usage

## Technical Details

### Slide Deck

- **[Live Slides](https://cuny-ai-lab.github.io/sandbox-series/basics/)** - Interactive slideshow
- **[Full workshop copy](https://cuny-ai-lab.github.io/sandbox-series/basics/workshop-copy.html)** - Complete text and alt text
- **[Presenter lesson plan](https://cuny-ai-lab.github.io/sandbox-series/WORKSHOP.html)** - Timed plan and access requirements
- **[GitHub Repository](https://github.com/CUNY-AI-Lab/sandbox-series)** - Source code and materials

### Related Sessions

- **[Curating Knowledge Collections](../curating-knowledge-collections/)** - Session 2, October 1, 2026
- **[Configuring Skills and Tools](../configuring-skills-tools/)** - Session 3, October 15, 2026

## Research & Citations

- Levesque, H., Davis, E., and Morgenstern, L. (2012). "The Winograd Schema Challenge." _Principles of Knowledge Representation and Reasoning_.
- CUNY AI Lab. [Sandbox documentation](https://ailab.gc.cuny.edu/sandbox-docs/): Basic Concepts, Custom Models, Getting Started.
- Open WebUI. [Models](https://docs.openwebui.com/features/workspace/models/).

## License

All materials are licensed under a **Creative Commons Attribution-ShareAlike (CC-BY-SA) 4.0 International Public License** unless otherwise noted.
