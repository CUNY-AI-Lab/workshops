# The Afterlives of the September 11 Digital Archive

_Stefano Morello's segment of a CUNY Graduate Center panel marking the 25th anniversary of September 11: what the Lab learned by running every item in the September 11 Digital Archive through open-weight models on New Media Lab hardware, and an offer to integrate that work into the archive's active preservation plan._

**Event:** The Afterlives of the September 11 Digital Archive, panel discussion
**Date:** Thursday, September 10, 2026, 6:00–8:00 p.m.
**Location:** Elebash Recital Hall, CUNY Graduate Center
**Format:** Panel discussion; this deck accompanies one presenter's segment
**Panel:** Stephen Brier, Tom Scheinfeldt, Greg "Fritz" Umbach, and Stefano Morello
**Deck:** Stefano Morello (Director, American Social History Project / Center for Media and Learning; CUNY AI Lab)

_The September 11 Digital Archive was built in 2001 by the American Social History Project (ASHP) and the Center for History and New Media (CHNM, now RRCHNM). This presentation was delivered as part of the Graduate Center's public events program._

## About the CUNY AI Lab

The **CUNY AI Lab** is a faculty and staff-led incubator for experimentation with AI by CUNY researchers across disciplines, strengthening CUNY's position at the leading edge of technological innovation. Located at the CUNY Graduate Center and led by experienced scholars and technologists who have built widely used open publishing platforms, the Lab fosters momentum for AI experimentation while foregrounding ethical practices and values that reinforce CUNY's mission of accessible, equitable, and transformative education.

This presentation is an example of the Lab's local pipeline: open-weight models run on the New Media Lab's own hardware for material that should not leave the Graduate Center.

## Overview

The deck moves in five movements. **Credits and stewardship** names who kept the archive alive between 2002 and tonight, the two eras of collection (ASHP and CHNM together) and stewardship (CHNM, then RRCHNM), and the fact that the archive cannot say so itself. **The record** scores the four "final challenging tasks" that Brier and Brown set out around the 2011 Omeka migration: migration to open-source infrastructure (done), long-term preservation (done), metadata enhancement (not done), and redesign of the public interface (partly). **Method and result** reports what was pulled from the archive's API, which models read it (GLM-OCR for handwriting, image transcription, and alt text; Whisper for voicemails, interviews, and recordings; the Lab's PDF accessibility tool for scanned documents), what came back, and the fact that every model was open-weights and ran locally. **The review tiers** cover file recovery, personally identifiable information, transcription and description quality, and metadata, and argue that searchability is a condition of plurality rather than a postscript to preservation. **Tier 4 and the offer** names new opportunities for interpretation (text analysis, mapping contributions, absence, languages) and frames the work as an offer to RRCHNM's active plan, not a rival to it.

## Key Figures

| What | Figure |
|------|--------|
| Items returned by the API | 70,359 |
| Files (150.7 GB); distinct file content by SHA-256 | 67,609; 66,830 |
| Handwritten card pages transcribed | 41,225 |
| Hours of audio transcribed locally | 199 |
| Photographs, flyers, drawings, and screenshots described | 31,600 |
| Characters read out of the FDNY Incident Action Plans | 17 million |
| Flash pieces recovered | 123 |

## Technical Details

### Built With

- Single-page HTML deck on the CUNY AI Lab slide framework (keyboard, swipe, scrubber, fragments, overview, lightbox), the same engine as the GCDI Orientation deck
- An archival aesthetic: paper-white slides, ink text, a deep archival blue accent, and a rust second accent reserved for work not yet done
- A title background, "Index Sweep," of one mark per sampled item

### Slide Deck

- **[Live Slides](https://cuny-ai-lab.github.io/sept11da-slides/)** - Interactive slideshow
- **[GitHub Repository](https://github.com/CUNY-AI-Lab/sept11da-slides)** - Source, speaker notes, and figure sources
- **[Slide-by-slide reference](./slides.md)**

### Related

- **[Event page](https://www.gc.cuny.edu/events/afterlives-september-11-digital-archive-panel-discussion)** - The Graduate Center
- **[September 11 Digital Archive](https://911digitalarchive.org)**
- **[CUNY AI Lab: Infrastructure, Access, and Outreach](../cail-oct-14/)** - The local pipeline described in the October 14, 2026 session

## License

All materials are licensed under a **Creative Commons Attribution-ShareAlike (CC-BY-SA) 4.0 International Public License** unless otherwise noted.
