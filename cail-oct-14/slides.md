# CUNY AI Lab, October 14, 2026 - Slide Reference

**Presenters:** Luke Waltzer, Matthew K. Gold, Stefano Morello, Stephen Zweibel, and Zach Muhlbauer
**Live:** [cuny-ai-lab.github.io/cail-oct-14](https://cuny-ai-lab.github.io/cail-oct-14/) (slide URLs use numbers: `#/3` opens slide 3)
**Source:** [CUNY-AI-Lab/cail-oct-14](https://github.com/CUNY-AI-Lab/cail-oct-14)

Luke and Matt open with context, without slides (about 5 to 7 minutes). The four slide sections run about 25 minutes, leaving about 35 minutes for discussion.

| # | Presenter | Title | Source |
|---|-----------|-------|--------|
| 1 | all | CUNY AI Lab | ACH 2026 title slide |
| 2 | all | Origins | Logos of the four units |
| 3 | Stefano | Infrastructure Decisions | Section opener |
| 4 | Stefano | Guiding Principles | The four principles on ailab.gc.cuny.edu, each beside a practice |
| 5 | Stefano | Bottom Up Approach to AI Infrastructure | Diagram redrawn from the ACH "CALI to CAIL" chart |
| 6 | Stefano | Infrastructure | Hosting diagram |
| 7 | Stefano | The Local Pipeline | Local transcription, diarization, image description, and OCR |
| 8 | Stefano | Sustaining and Sharing the Work | Retreat outline and position paper |
| 9 | Steve | The CAIL Gateway, Access and Agent Tools | Section opener |
| 10 | Steve | The CAIL Gateway | Gateway overview deck, merged |
| 11 | Steve | Applying for Access | Live request-access page; admin queue with sample data |
| 12 | Steve | Class Overview for Instructors | My classes page with sample data |
| 13 | Steve | Administration | Admin People and class views with sample data |
| 14 | Steve | Agent Studio and Site Studio | Agent Studio workspace screenshot; Site Studio mock-up |
| 15 | Steve | CAIL Pi | Fall 2026 workshops |
| 16 | Zach | Apps and Outreach | Section opener |
| 17 | Zach | The CAIL Sandbox | ACH 2026 |
| 18 | Zach | Comparing Open-Weight Models | ACH 2026 |
| 19 | Zach | Configurations for Courses | ACH 2026 |
| 20 | Zach | AmigAI in Spanish Courses | ACH 2026 |
| 21 | Zach | Tools Portal | New screenshot and bullets |
| 22 | Zach | Teaching Tools | Screenshot showing Stem Splitter and Systems Mapping |
| 23 | Zach | Demo | Embedded Vimeo video |
| 24 | all | Discussion | ACH 2026 |

## Opening (all)

### 1. CUNY AI Lab

Luke Waltzer, Matthew K. Gold, Stefano Morello, Stephen Zweibel and Zach Muhlbauer. CUNY Graduate Center, October 14, 2026.

### 2. Origins

Teaching and Learning Center · GC Digital Initiatives · Mina Rees Library · American Social History Project. Four Graduate Center units that each took up AI in their own way and came together as the CUNY AI Lab.

## Infrastructure Decisions (Stefano Morello)

### 4. Guiding Principles

- **Privacy by Design:** we only work with Zero Data Retention providers, and with locally hosted models. Cloud models run only on zero-retention hosts; material that shouldn't be sent out goes to the GPU server in the New Media Lab.
- **Transparency:** we favor open-weight models and make their licenses, abilities, and limits legible in our Model Registry. Published weights let the Lab get the same model from more than one provider; a closed model is offered only for a specific reason.
- **Environmental Accountability:** we show the estimated carbon footprint under every query.
- **Criticality:** we try to build tools that open up how AI works and keep users' judgment at the center.

### 5. Bottom Up Approach to AI Infrastructure

For CUNY, by CUNY. A shared approach across centers, rooted in digital humanities, critical ed tech, and open knowledge. Tools built in conversation with faculty and staff. Since 2022: Teaching and Learning Center, GC Digital Initiatives, Mina Rees Library, ASHP / New Media Lab → Critical AI Literacy Institute (2025) → CUNY AI Lab (Fall 2025). The Lab responds to people who come to it for help and support, not to wish lists; the point is continuity and accountability, not scale. The TLC strand: Teach@CUNY AI Toolkit (2023), TLC workshops (2023 to 2024), communities of practice (2024 to 2025), then CALI (2025).

### 6. Infrastructure

One way in, the places the cloud tools run, and the model calls that cross them. People sign in with CUNY Login and apply, on their own or for a class; the front door then checks login, access, and allowance on every visit. Cloudflare Workers host PDF Accessibility, Agent Studio, Site Studio, Media Tools, and the Model Gateway itself. The Sandbox runs on an always-on container on AWS. With a Lab key, API access works from any code or app; CAIL Pi is one thing it serves. Solid lines go through the Gateway or are run by the Lab; dashed lines go straight to a provider.

### 7. The Local Pipeline

The answer for material that shouldn't leave the Graduate Center, such as identifiable research data. Everything is local: model weights are downloaded once, and no file leaves the machine while a job runs. Lab staff run jobs on the New Media Lab's own hardware: a Dell Pro Max workstation (NVIDIA RTX 5000 Ada, 32 GB of GPU memory) and Mac Studios. Installed: faster-whisper (served by Speaches) and pyannote speaker-diarization 3.1 for transcription and speaker labels; Qwen3-VL 8B and DeepSeek-OCR for image description and OCR. It became a standing service on September 25, 2026, when a principal investigator asked for an IRB-approvable way to transcribe focus-group audio.

### 8. Sustaining and Sharing the Work

**Within CUNY:** access is open to everyone at the GC, and across CUNY mostly through classes; building a community of practice to scale, including fellows who support classes and projects, and workshops. Spring 2026: Fellows Cohort 1; Vibe Coding workshops. Fall 2026: Fellows Cohort 2; Vibe Coding, Sandbox Series, coworking sessions. Class access opens when the instructor brings a critical approach to AI and can support their own students, or when the Lab can support the course itself.

**Beyond CUNY:** we publish most of our code so other universities can adapt and adopt it; we look for partners who understand CUNY's procurement and find creative ways to work within it. Commons In A Box is the CUNY precedent for packaging academic software that other institutions can run and change.

## The CAIL Gateway, Access and Agent Tools (Stephen Zweibel)

### 10. The CAIL Gateway

We connect the Lab's tools to it; we choose which models to offer; we run it on Cloudflare Workers. Lab tools (Sandbox, Studios, Media Tools), personal API keys (researchers' own code), and approved applications (other CUNY projects) → CAIL Gateway (credential, allowance, and model checks) → model providers (zero retention, open weights). Researchers can call every model from their own code with one key, and a model can move to another provider without anyone changing their tools. Providers are deliberately unnamed on the slide.

### 11. Applying for Access

People apply on their own or for a whole class. Everyone signs in with CUNY Login first. Each application is reviewed and given an allowance ($5 or $20 a month). Instructors share one link, and students join with it. One application covers the Sandbox, API keys, the Studios, and Media Tools. Students at other campuses get in through a class. Administration screens show sample data.

### 12. Class Overview for Instructors

Instructors see who has joined their class and which students are nearing their allowance (20% or less left, counting everything they do in the Lab; instructors never see amounts). They can replace or close the class link and withdraw a student. Sample data.

### 13. Administration

Administrators see every person's access, allowance, and end date; each class with its teachers and students; and approve, renew, and withdraw access in one place. Allowances: standard $5, plus $20, administrator $50, each per 30 days. The same work can be done from Claude or Codex through an MCP server (about 60 actions: reviewing requests and class applications, rosters and class links, allowance resets, diagnostics), with CUNY Login and a check on every action that the person is still an administrator. Sample data.

### 14. Agent Studio and Site Studio

People hand the agent a whole task. Researchers keep sources, files, and drafts in one Agent Studio workspace; faculty and students build and preview academic websites in Site Studio. Same sign-in and allowance as the other tools. The Agent Studio screenshot is a real workspace from the current app; Site Studio is still the mock-up from the ACH deck.

### 15. CAIL Pi

Pi is an open-source coding agent for the terminal. Participants set it up with the Lab's models in one command; each person uses their own Lab key and allowance. The Lab teaches with it in the fall's vibe-coding workshops. Agent Studio and Site Studio offer agent help in the browser for people for whom the terminal is a barrier. Closing: the Gateway can connect to any provider that meets these rules, including a public one; Empire AI is the obvious candidate in New York.

## Apps and Outreach (Zach Muhlbauer)

### 17. The CAIL Sandbox

The Lab's chat and classroom AI environment, built on Open WebUI: curated open-weight models and configurable tools behind CUNY sign-in. Models on the left, chat in the center, system prompt and parameters on the right.

### 18. Comparing Open-Weight Models

Send one prompt to two curated models and read the responses side by side, with token counts and response times. A public Model Registry explains capabilities, licensing, and recommended use.

### 19. Configurations for Courses

Course-specific configurations: a base model, system prompt, documents, and tools. Reusable project templates adapted across sections and semesters. A configuration becomes a designed object students can interrogate.

### 20. AmigAI in Spanish Courses

One configuration template, adapted across Spanish sections: SPAN 101 conversation, SPA 204 discourse analysis, SPAN 207 heritage critique (and SPA 4010 as a writing coach). At ACH in June 2026, the AmigAI sections were the busiest workload, 36.6% of all messages.

### 21. Tools Portal

[ailab.gc.cuny.edu/tools](https://ailab.gc.cuny.edu/tools): transcription, image description, and OCR; PDF accessibility checks; a free, public AI Use Disclosure tool.

### 22. Teaching Tools

Stem Splitter and Systems Mapping follow the media processing examples.

### 23. Demo

Embedded Vimeo demo video.

### 24. Discussion
