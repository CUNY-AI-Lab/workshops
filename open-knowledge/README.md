# AI & Open Educational Resources

_A CUNY AI Lab session for the Graduate Center's Open Knowledge Fellowship: how language models work, what they can do now, what AI extraction does to open knowledge, and where AI belongs in OER work._

The session opens with Langdon Winner's question, what kind of world are we building as we use AI, and leaves the decision about AI use to each participant. Part I explains inference and training and unpacks a documented training corpus, The Pile. Part II covers why models are rewarded for guessing, how grounding and tools work, and what an agentic loop is. Part III turns to the problematics for open knowledge: what happens to "Open," chat answers that take the audience from open sites, publishers licensing scholarly writing to AI companies, why a license alone will not stop training, what it means when open knowledge becomes model weights, and public AI. Part IV asks where AI helps with OER work, how to judge appropriate use, and shows projects the presenters and fellows built. Five discussion questions close the session.

**Date:** June 2026 (Summer 2026)
**Audience:** Open Knowledge Fellowship participants, CUNY Graduate Center
**Format:** Presentation with discussion (35 slides)
**Presenters:** Stefano Morello, Zach Muhlbauer, and Stephen Zweibel (CUNY AI Lab)

_This session was originally conducted for the Open Knowledge Fellowship at the CUNY Graduate Center. An earlier 32-slide iteration of the deck survives in the Lab's `critical-ai-encounters` repository._

## About the CUNY AI Lab

The **CUNY AI Lab** is a faculty and staff-led incubator for experimentation with AI by CUNY researchers across disciplines, strengthening CUNY's position at the leading edge of technological innovation. Located at the CUNY Graduate Center and led by experienced scholars and technologists who have built widely used open publishing platforms, the Lab fosters momentum for AI experimentation while foregrounding ethical practices and values that reinforce CUNY's mission of accessible, equitable, and transformative education.

This session is part of the CUNY AI Lab's commitment to developing critical AI literacy among faculty, staff, and students across the university system.

## Key Points

- **Inference and training:** a model generates one token at a time from the context window; training repeats a hidden-next-token guess at scale, then tunes with examples and human rankings
- **Training data:** The Pile (EleutherAI) documents its 22 sources openly, including the contested Books3 set of about 196,000 books from a piracy site; most commercial corpora are hidden
- **Rewarded for guessing:** hallucinations persist because training and evaluation reward confident guesses over acknowledged uncertainty (Kalai et al.)
- **Grounding and loops:** tools let a model search, read a file, or run code and read the result; agentic systems revise each tool call from the last result
- **What happens to "Open":** model builders can train on open work while dropping credit and returning nothing; referral traffic to open sites has fallen; some publishers have sold scholarly writing to AI companies without asking or paying authors
- **Licenses and weights:** courts in 2025 treated training as fair use; restrictive licenses mostly affect ordinary reusers; collective responses (Creative Commons preference signals, Wikimedia charging scrapers) have more force; Wiley's 5Rs applied to model weights
- **Public AI:** open models that can be run outside a single company and governed in public; the CUNY AI Lab runs on such models as a public, non-commercial service that does not train on user data
- **Where AI helps with OER:** alt text and captions people then check; OCR of scanned pages into editable text; rough drafts and translations a subject expert revises; always with a person accountable, disclosure, a check against a reliable source, and grounding in trusted sources
- **Projects:** Manifold Companion (OCR and structure for CUNY's Manifold instance); the Franco Lalli manuscript archive; the Italian American Open Syllabus; Impariamo l'Italiano and LanGames; Cloze Reader; ThinkWith, built by a first-year writing instructor after CUNY AI Lab workshops
- **Informed refusal and informed adoption:** both are legitimate; the point is to have reasons and say them

## Discussion Questions

1. Where in your teaching would a grounded, course-specific assistant help, and where would it get in the way?
2. What would informed refusal look like in your field? What would you want to tell a student about it?
3. If you released an OER, how would you want AI to be allowed to use it, or not?
4. What is one resource you have wanted to build but could not? Could anything here lower that barrier?
5. Which of today's worries still feels unresolved to you?

## Technical Details

### Built With

- Single-page HTML deck using the knowledge-collections deck engine with a warm ivory theme (no dark slides), lazy-loaded live site embeds in browser frames, screenshot sliders with captions, and a lightbox
- Accessibility: hash routing, overview on Escape, focus management, ARIA announcements, reduced motion

### Slide Deck

- **[Live Slides](https://cuny-ai-lab.github.io/open-knowledge/)** - Interactive slideshow
- **[GitHub Repository](https://github.com/CUNY-AI-Lab/open-knowledge)** - Source code and the spoken transcript
- **[Slide-by-slide reference](./slides.md)**
- **[Earlier iteration](https://github.com/CUNY-AI-Lab/critical-ai-encounters)** - 32-slide version with a five-part roadmap (Who We Are; What Is AI?; What "Agentic" Means; AI & OER in Practice; Discussion)

### Related

- **[Manifold Companion](https://github.com/CUNY-AI-Lab/manifold-companion)**
- **[Teach@CUNY AI Toolkit](../tcuny-ai-toolkit/)**

## License

All materials are licensed under a **Creative Commons Attribution-ShareAlike (CC-BY-SA) 4.0 International Public License** unless otherwise noted.
