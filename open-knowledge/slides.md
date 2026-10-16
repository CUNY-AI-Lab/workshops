# AI & Open Educational Resources - Slide Reference

**Presenters:** Stefano Morello, Zach Muhlbauer, and Stephen Zweibel (CUNY AI Lab)
**Audience:** Open Knowledge Fellowship participants · **Date:** June 2026
**Live:** [cuny-ai-lab.github.io/open-knowledge](https://cuny-ai-lab.github.io/open-knowledge/) · **Source:** [CUNY-AI-Lab/open-knowledge](https://github.com/CUNY-AI-Lab/open-knowledge) (includes the spoken transcript this reference follows)

## 1–2. Opening

**AI & Open Educational Resources.** What kind of world are we building as we use AI? For OER the question starts with provenance: AI makes it easier to adapt and remix course materials, but it can also erase the trail of reuse and revision that open education depends on. David Wiley's 5Rs; Creative Commons' CC Signals as an AI-era way to express reuse preferences.

**Whether You Use AI Is Your Call.** Langdon Winner's question; AI is already part of teaching and learning; the Graduate Center's draft guidance leaves decisions about AI use to you.

**Roadmap.** I. AI Basics · II. What It Can Do Now · III. Problematics · IV. Your OER Work · V. Discussion.

## Part I: AI Basics (3–6)

- **Large Language Models Predict Tokens:** inference builds the output one token at a time; tokenize the prompt, fill the context window, run a forward pass, score possible next tokens, choose one, repeat.
- **How Large Language Models Are Trained:** guess a hidden next token, check, shift the weights, at huge scale; later tuning with examples and human rankings.
- **Unpacking The Pile:** EleutherAI's documented 825 GiB English corpus from 22 sources (Wikipedia, Project Gutenberg, Stack Exchange, GitHub, arXiv, PubMed Central, FreeLaw, Books3); Books3's roughly 196,000 books copied from a private piracy site.

## Part II: What It Can Do Now (7–10)

- **Rewarded for Guessing:** Kalai and coauthors on why hallucinations persist; rare facts answered from nearby patterns; benchmarks that reward lucky guesses and give no credit for uncertainty.
- **Grounding the Answer:** a grounded system searches a live source before answering; tools let the model search the web or a catalog, read a file, or run code and read the result.
- **Working in a Loop:** agentic systems revise each tool call from the last result; a weak search triggers a better query; an error triggers a patch; bad OCR triggers tighter instructions.

## Part III: Problematics (11–18)

- **What Happens to "Open":** open licensing asks for credit and a return to the commons; model builders can train while dropping both; if open work is scraped without return, some people stop sharing and the commons shrinks.
- **Chat Answers Take the Audience:** when an AI answer replaces the click-through, readers who are also maintainers stop arriving; referral traffic to open sites has fallen while automated traffic climbs.
- **Academic Publishers Are Selling Scholarly Writing to AI Companies:** deals by Taylor & Francis and Wiley made without asking or paying authors; the writing sold is the closed, paywalled kind authors sign over.
- **A License Alone Will Not Stop Model Training:** 2025 rulings treating training as fair use; a large settlement for pirating books, not for training; restrictive licenses mostly burden ordinary reusers; collective responses (CC preference signals, Wikimedia charging scrapers) have more force.
- **When Open Knowledge Becomes Weights:** the 5Rs (retain, revise, remix, reuse, redistribute) asked of model weights: can people download and run them, inspect training data and code, reuse under the license, run them without costly hardware?
- **Public AI:** closed models owned and run by one company versus open models run outside any single company and governed in public.
- **The CUNY AI Lab:** a faculty- and staff-led group that builds and runs AI infrastructure for teaching and research across CUNY; public and non-commercial; open models; no training on your data.

## Part IV: Your OER Work (19–29)

- **Where It Helps with OER Work:** alt text and captions people then check; scanned pages and old PDFs into editable, publishable text; rough drafts and translations a subject expert revises.
- **Judging Appropriate Use:** Is a person accountable for the result? Is AI assistance disclosed? Has the output been checked against a reliable source? Is the model grounded in sources you trust?
- **From Idea to Artifact:** subject experts can build the resource they imagine without writing every line; digitizing archives, interactive resources, a lower barrier for people without a coding background.
- **Manifold Companion:** a document-processing platform for CUNY's Manifold instance; AI handles OCR and structure; humans review and export.
- **Lalli, Il Venditore di Sogni:** digitized manuscripts of an Italian-American writer published as an open, searchable archive with OCR and translation side by side.
- **Italian American Open Syllabus:** a curated, peer-reviewed collection of open essays and reading lists; AI converted Word contributions into clean HTML; the editing and scholarship stayed human.
- **Impariamo l'Italiano:** interactive Italian-learning games built with AI assistance by a fellow with no coding background; a later multilingual version, LanGames.
- **Cloze Reader:** a small reading-practice tool that turns passages into fill-in-the-blank exercises.
- **ThinkWith:** built by a first-year writing instructor after CUNY AI Lab workshops; a student pastes a source passage, a cultural artifact, and a connecting paragraph, and the model gives feedback that sends them back to revise; the judge is still a model, so the teacher still judges the result.
- **Informed Refusal and Informed Adoption:** both legitimate; use AI where it helps with someone accountable, and say why; decline where it does not fit, and say why.

## Part V: Discussion (30–35)

Five discussion questions (see README) and a references slide: Kalai et al. on hallucinations; Stanford HAI's AI Index; the Open Source Initiative; OLMo; Wiley on the 5Rs; UNESCO on open education; the Authors Guild and The Bookseller on publisher deals; Open Future and Internet Policy Review on public AI and the commons; Langdon Winner; Creative Commons on AI training and signals; Verhulst on openness; Wikimedia on crawler load and paid API access.
