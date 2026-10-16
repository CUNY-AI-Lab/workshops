# The Afterlives of the September 11 Digital Archive - Slide Reference

**Panel discussion · Elebash Recital Hall, CUNY Graduate Center · September 10, 2026**
**Deck:** Stefano Morello (ASHP/CML; CUNY AI Lab) · **Panel:** Stephen Brier, Tom Scheinfeldt, Greg "Fritz" Umbach, Stefano Morello
**Live:** [cuny-ai-lab.github.io/sept11da-slides](https://cuny-ai-lab.github.io/sept11da-slides/) · **Source:** [CUNY-AI-Lab/sept11da-slides](https://github.com/CUNY-AI-Lab/sept11da-slides)

## Movement 1: Credits and Stewardship

- **Title:** The Afterlives of the September 11 Digital Archive; 911digitalarchive.org.
- **Credits (partial), 2002 to tonight:** a timeline of collection (ASHP/CML and CHNM together, 2001) and stewardship (CHNM, then RRCHNM: preservation, the Omeka migration, hosting, fundraising). The spoken note: the people who kept the archive running are not on the stage; stewardship over this timescale has been "whoever happened to still be there," and the archive cannot tell you who maintained it. RRCHNM has an active plan (Title II accessibility compliance; flattening the site for long-term sustainability).

## Movement 2: The Record

- **"Final challenging tasks" (Brier & Brown, 2011):** migration to open-source infrastructure (done, funded by Save America's Treasures and NEH); long-term preservation (done); metadata enhancement (not done); redesign of the public interface (partly, in 2011).
- **The turn (spoken, no slide):** the four tasks are still the right list; what none could anticipate is that a machine can now read the archive: handwriting, voicemails, photographs. That moves the cost of reading from unaffordable to an afternoon of GPU time in the New Media Lab, and makes the two open tasks, metadata and interface, tractable along with accessibility (alt text, transcripts, captions). Machine reading makes compliance tractable; compliance makes discoverability fundable.

## Movement 3: Method and Result

- **Data:** 70,359 items returned by the API; 67,609 files, 150.7 GB; 66,830 distinct by SHA-256 (779 duplicates).
- **Processing:** every model open-weights and run locally on New Media Lab hardware. GLM-OCR for handwriting, image transcription, and alt text; Whisper for voicemails, interviews, and recordings; PDF remediation with the CUNY AI Lab's PDF accessibility tool. Privacy, reproducibility, cost.
- **Output:** 41,225 handwritten card pages transcribed ("How did you witness history on September 11, 2001?"); 199 hours of audio; 31,600 photographs, flyers, drawings, and screenshots described (83 GB of imagery, now searchable); 17 million characters read from the FDNY Incident Action Plans; 123 Flash pieces recovered.

## Movement 4: Recovery, Review, and Remediation

- **Tiers:** 0 file recovery · 1 personally identifiable information · 2 transcription and description quality · 3 metadata · 4 new opportunities for interpretation.
- **Tier 1, PII:** a review queue of flagged items by urgency, including reachable minors and spoken contact details.
- **Tier 2, Quality review (Is the machine right?):** sampling across the 41,225 card pages, 31,600 images, and 199 hours of audio; a QC dashboard by pipeline (vision, zip-image, PDF, handwritten text recognition, speech recognition).
- **Tier 3, Metadata enhancement:** Dublin Core as stored, 18 fields across 70,359 items; Subject empty on every item; 24 usable dates; no tags. Now that every item has text, writing or inferring metadata for discoverability and accessibility becomes far easier.

## Movement 5: Tier 4 and the Offer

- **New opportunities for interpretation:** text analysis, mapping contributions (hometowns), absence, languages, and more; index counts of hometowns, characters, site captures, and members.
- **Lenses** that an index makes answerable, with the rule that every visual walks back to the artifact; a marked placeholder lens for Iraq / FDNY material.
- **The offer:** this work is offered to RRCHNM's active preservation and accessibility plan, not instead of it.
