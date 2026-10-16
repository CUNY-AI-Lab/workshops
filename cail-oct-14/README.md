# CUNY AI Lab: Infrastructure, Access, and Outreach

_An October 14, 2026 session presenting how the CUNY AI Lab operates: its guiding principles, where its tools run, the CAIL Gateway and access system, and the Sandbox and tools in use across CUNY._

This 24-slide session was prepared for a visit by colleagues from CUNY Central and guests. Luke Waltzer and Matthew K. Gold opened with context, without slides. Stefano Morello presented the Lab's infrastructure decisions, Stephen Zweibel the CAIL Gateway, access, and agent tools, and Zach Muhlbauer the Sandbox, course configurations, and outreach, followed by an open discussion. The format was informal, with questions invited throughout.

**Date:** Tuesday, October 14, 2026, about 4:15 to 5:20 p.m.
**Location:** CUNY Graduate Center
**Format:** Presentation (about 25 minutes of slides across four sections) and discussion (about 35 minutes)
**Presenters:** Luke Waltzer, Matthew K. Gold, Stefano Morello, Stephen Zweibel, and Zach Muhlbauer (CUNY AI Lab)

_The deck remixes slides from the Lab's ACH 2026 presentation and internal planning documents (a September 2026 retreat outline, a July 2026 position paper on AI infrastructure for CUNY, and an August 2026 Gateway overview)._

## About the CUNY AI Lab

The **CUNY AI Lab** is a faculty and staff-led incubator for experimentation with AI by CUNY researchers across disciplines, strengthening CUNY's position at the leading edge of technological innovation. Located at the CUNY Graduate Center and led by experienced scholars and technologists who have built widely used open publishing platforms, the Lab fosters momentum for AI experimentation while foregrounding ethical practices and values that reinforce CUNY's mission of accessible, equitable, and transformative education.

The Lab grew out of four Graduate Center units that each took up AI in their own way: the Teaching and Learning Center, GC Digital Initiatives, the Mina Rees Library, and the American Social History Project / Center for Media and Learning with its New Media Lab. The Critical AI Literacy Institute (2025) brought that work under one banner; the CUNY AI Lab launched in Fall 2025.

## Overview

The session makes the case for a bottom-up, "for CUNY, by CUNY" approach to AI infrastructure. Stefano Morello's section carries the commitments: the four guiding principles on the Lab's website (privacy by design, transparency, environmental accountability, criticality), each paired with a current practice; the origins chart from the centers through CALI to CAIL; a hosting diagram showing one way in and where the cloud tools run; a fully local pipeline for material that should not leave the Graduate Center; and how the Lab sustains and shares the work within and beyond CUNY. Stephen Zweibel's section shows where those commitments become working rules: the CAIL Gateway through which the Lab's tools, personal API keys, and approved applications reach model providers; the application and class-access system; administration screens and an MCP server for administrators; Agent Studio and Site Studio; and CAIL Pi, a terminal coding agent used in the fall vibe-coding workshops. Zach Muhlbauer's section covers the Sandbox, side-by-side model comparison, course configurations, the AmigAI Spanish template, the Tools portal, teaching tools, and a demo video.

## Key Points

- **Guiding principles in practice:** only zero-data-retention providers and locally hosted models; open-weight models with licenses, abilities, and limits legible in the Model Registry; an estimated carbon footprint shown under every query; tools that open up how AI works and keep users' judgment at the center
- **Bottom-up operations:** the Lab responds to people who come to it for help and support, carrying forward how the centers have always worked with faculty, students, and staff
- **Where the tools run:** CUNY Login and an application as the one way in; Cloudflare Workers for the Studios, Media Tools, PDF Accessibility, and the Model Gateway; an always-on container for the Sandbox; API access with a Lab key from any code or app
- **The local pipeline:** transcription and speaker labels (faster-whisper, pyannote), image description and OCR on the New Media Lab's own GPU workstation and Mac Studios, with nothing leaving the machine while a job runs; a standing service since late September 2026
- **The CAIL Gateway:** one key for every model; models can move to another provider without anyone changing their tools; credential, allowance, and model checks on every request
- **Access and allowances:** individual or class applications, reviewed with a monthly allowance; instructors share one class link and can see who has joined, who is nearing their allowance, and withdraw students; administrators manage people and classes in one place, including from Claude or Codex through an MCP server
- **Agent tools:** Agent Studio (sources, files, and drafts in one workspace) and Site Studio (academic websites built and previewed in the browser); CAIL Pi for the terminal
- **Sustaining and sharing:** access open across the Graduate Center and, elsewhere in CUNY, mostly through classes; graduate student fellows (a Spring 2026 cohort and a 2026–27 cohort) and workshop series (Vibe Coding in Spring and Fall 2026, the Sandbox Series, and coworking sessions); most code published for other universities to adapt and adopt

## Technical Details

### Built With

- Reveal.js 5.1.0 with the notes plugin; speaker notes for every slide (press `S`)
- A light theme (Newsreader headings, IBM Plex Sans text) with a presenter accent per section
- Inline SVG diagrams for hosting and the local pipeline; a carbon-footprint overlay; an embedded demo video
- Administration screens shown with sample data only

### Slide Deck

- **[Live Slides](https://cuny-ai-lab.github.io/cail-oct-14/)** - Interactive slideshow with speaker notes
- **[GitHub Repository](https://github.com/CUNY-AI-Lab/cail-oct-14)** - Source code and slide manifest
- **[Slide-by-slide reference](./slides.md)** - Contents and spoken notes for all 24 slides

### Related

- **[CUNY AI Lab](https://ailab.gc.cuny.edu/)** - Guiding principles, [Model Registry](https://ailab.gc.cuny.edu/models/), [Tools](https://ailab.gc.cuny.edu/tools), and [access application](https://ailab.gc.cuny.edu/request-access/)
- **[Sandbox Workshop Series (Fall 2026)](../sandbox-series/)** and **[Critical AI Literacy Institute at Brooklyn College](../cali-brooklyn/)**

## License

All materials are licensed under a **Creative Commons Attribution-ShareAlike (CC-BY-SA) 4.0 International Public License** unless otherwise noted.
