# AI Agent Prompts — Complete Collection

> **Purpose:** Ready-to-copy prompt templates for pulling research from any AI agent (Claude, GPT, Gemini, Grok, etc.)
> **Last Updated:** Mar 14, 2026
> **Usage:** Copy the relevant prompt, replace [BRACKETS] with your topic, paste into any AI agent

---

## TABLE OF CONTENTS

1. [Project Onboarding Prompt](#1-project-onboarding-prompt) — Give any AI agent full project context
2. [Full Research Pull](#2-full-research-pull) — Deep research on a new topic from scratch
3. [Quick Expansion Pull](#3-quick-expansion-pull) — Add new info to an existing document
4. [Cross-Connection Analysis](#4-cross-connection-analysis) — Find connections between topics
5. [Counter-Argument & Bias Check](#5-counter-argument--bias-check) — Stress-test claims
6. [Section Sweep](#6-section-sweep) — Audit an entire section for gaps
7. [Image Source Pull](#7-image-source-pull) — Find real, downloadable reference images
8. [Primary Source Analysis](#8-primary-source-analysis) — Deep dive into ancient texts
9. [Scientific Literature Review](#9-scientific-literature-review) — Peer-reviewed papers on a topic
10. [Philosophical Analysis](#10-philosophical-analysis) — Meaning, ethics, existential questions
11. [Timeline Construction](#11-timeline-construction) — Build comprehensive chronologies
12. [Synthesis & Pattern Detection](#12-synthesis--pattern-detection) — Find hidden connections across domains
13. [Source Verification Audit](#13-source-verification-audit) — Fact-check claims and validate sources
14. [Master Doc Section Evidence Refresh](#14-master-doc-section-evidence-refresh) — Scan one master-doc section at a time for new evidence, contradictions, and stale stats

---

## 1. PROJECT ONBOARDING PROMPT

```
You are contributing to a multi-disciplinary research knowledge base called "Theories of Everything."

PROJECT SCOPE: Understanding the fundamental nature of existence — the origin and meaning of life, the nature of reality and consciousness, ancient wisdom, suppressed knowledge, and possible futures.

SCALE: 2,437 documents across 34 sections (A–ZH), ~395,376+ lines, 30,637+ indexed keywords, 627+ images.

QUALITY METRICS: Quality 85.8/100 (A-), Factuality 72.4/100 (B-). 0 errors, 0 warnings. 40 active scripts, 7-source external verification pipeline, 25,686 claims extracted.

SECTIONS (34 total, A–ZH):
A-Foundations (ancient texts), B-Beings & Entities, C-Global Traditions, D-Sites & Artifacts, 
E-Cataclysms & Chronology, F-Lost Connections, G-Modern Frameworks, H-Suppression & Thesis,
I-UAP Disclosure, J-Ancient Technology, K-Consciousness, L-Genetics & Origins, 
M-Forbidden Archaeology, N-Secret Societies, O-Earth Anomalies,
P-Philosophy & Meaning, Q-Cosmology & Physics, R-Biology & Evolution, S-Future & Technology,
T-Psychology & Social, U-Art, Music & Culture, V-Mathematics & Information,
W-World Civilizations, X-Medicine & Healing, Y-Altered States & Psychedelics,
Z-Molecular Biology & Genomics, ZA-Physics & Quantum Mechanics, ZB-Ecology & Organismal Biology,
ZC-Social Science & Anthropology, ZD-Information & Computation, ZE-Ethics & Applied Philosophy,
ZF-Oceanography, ZG-Linguistics & Communication, ZH-Archaeoastronomy

FILE NAMING: [Section]_[Group]_[Seq]_Name.md (e.g., A_1_01_Sumerian_Texts.md)
Each doc ID encodes section, subfolder group, and position within that group.

RELIABILITY SYSTEM — 4 Tiers:
- Tier 1 VERIFIED: Peer-reviewed, archaeological record, primary texts
- Tier 2 CREDIBLE: Academic, debated but supported
- Tier 3 SPECULATIVE: Possible but unverified
- Tier 4 DUBIOUS: No credible source / contradicted by evidence

SOURCE CONFIDENCE: [N/5] rates a document's weighted bibliography score. Each source is classified: peer-reviewed journal = 3 pts, academic press/primary text = 2 pts, popular/other = 1 pt. Thresholds: [1/5] = <14 pts, [2/5] = 14-21, [3/5] = 22-29 (median), [4/5] = 30-41, [5/5] = 42+.

RULES:
- NEVER fabricate sources — only cite real publications with real authors, titles, publishers, dates
- NEVER fabricate ISBNs, DOIs, scholar names, artifact numbers, or quotes
- Present ALL sides — mainstream, alternative, skeptical
- Rate every claim with a Tier (1-4)
- Flag debunked claims with [DEBUNKED] tag
- Distinguish between "unproven" and "disproven"
- Include counter-arguments for every major claim — ONLY if real, published ones exist. If no real counter-argument exists (settled consensus), say so honestly rather than inventing weak objections
- Use evidence specificity: exact dates, named scholars in **bold**, measurements with units, institutional attribution, artifact/tablet IDs
- Minimum 5 bibliography entries per document; Source Count header must match actual bib count
- Use the CANONICAL PROMPT at `_scripts/prompts/research_pull_prompt.md` for all new document creation — it contains the complete, current document template and all formatting rules
- VS Code Copilot users: `.github/copilot-instructions.md` is auto-loaded every session with all formatting rules — follow it exactly
- CRITICAL FORMAT RULES: Blockquote headers (NEVER tables), Chicago bibliography (NEVER APA), ALL-CAPS section headings (except Counter-Arguments & Criticisms), 2-column cross-reference tables, verify filenames before linking

ORIGINAL THESIS (still active): 78.9% of ancient serpent traditions were originally positive (knowledge-givers), later demonized over ~2,500 years.

EXPANDED MISSION: Build the most comprehensive, interconnected knowledge base about the nature of existence — ancient wisdom, modern science, consciousness, origins, meaning, and the future of humanity.
```

---

## 2. FULL RESEARCH PULL

> **CANONICAL PROMPT:** `_scripts/prompts/research_pull_prompt.md` — Use the "Universal Research Pull" section.
> This is the ONLY prompt that should be used to create new documents. It contains the complete, up-to-date document template, formatting rules, evidence specificity requirements, counter-argument guidance, weighted scoring instructions, and all non-negotiable rules.

**Quick summary of what the canonical prompt includes:**
- Full document template (header → Quick Summary → Tiers 1–4 → Counter-Arguments & Criticisms → Images → Bibliography → Cross-Reference Index)
- Source Confidence computation formula (journals ×3, academic ×2, other ×1; thresholds for [1/5] through [5/5])
- Evidence specificity rules (exact dates, named scholars in **bold**, measurements with units, institutional attribution, artifact IDs)
- Counter-argument rules (only real, published CAs — honest "no dispute" note for settled consensus)
- Non-negotiable rules (no fabrication, minimum 5 bib entries, Source Count must match actual bib count)
- Image source priority list
- NEW SOURCES FOUND table for candidate sources needing external verification

**To use:** Open `_scripts/prompts/research_pull_prompt.md`, copy the prompt, replace `[TOPIC]` and `[SECTION_ID]`, paste into any AI agent.

---

## 3. QUICK EXPANSION PULL

> **CANONICAL PROMPT:** `_scripts/prompts/research_pull_prompt.md` — Use the "Quick-Pull Variant" section.
> Contains updated evidence specificity rules, counter-argument guidance, and source verification requirements.

**To use:** Open `_scripts/prompts/research_pull_prompt.md`, copy the Quick-Pull variant, replace `[TOPIC]` and `[DOC_ID]`, paste into any AI agent.

---

## 4. CROSS-CONNECTION ANALYSIS

```
CONNECTION ANALYSIS — [TOPIC A] ↔ [TOPIC B]

I have research documents on both [TOPIC A] and [TOPIC B]. 
Find ALL connections between them that I may have missed:

1. Direct textual/evidential links
2. Symbolic or thematic parallels
3. Shared personnel or researchers
4. Chronological overlaps
5. Causal or correlation relationships
6. Counter-connections (where they seem linked but aren't)
7. Connections that pass through a THIRD topic

For each connection:
- Rate strength: STRONG / MODERATE / SPECULATIVE / SUPERFICIAL
- Cite the specific evidence
- Note if the connection has been previously identified in mainstream scholarship
- Suggest how this connection changes understanding of either topic

Also identify: what BROADER PATTERN does this connection reveal about the nature of reality, knowledge, or human experience?
```

---

## 5. COUNTER-ARGUMENT & BIAS CHECK

```
BIAS CHECK — [TOPIC] — [DOC_ID]

Review the following claims about [TOPIC] and provide:

1. **Strongest counter-arguments** for each claim listed
2. **Steel-man the skeptical position** — make the BEST possible case against the claims
3. **Identify confirmation bias** — where has cherry-picking occurred?
4. **Source quality audit** — are the cited sources reliable? Any retracted?
5. **Missing context** — what important information is omitted?
6. **Alternative explanations** that are simpler (Occam's Razor test)
7. **Updated information** — has new evidence changed the picture since original writing?
8. **Logical fallacies** present in the argumentation

Be ruthless. The goal is to make the research STRONGER by exposing weaknesses.
Do NOT soften criticism to be polite.
```

---

## 6. SECTION SWEEP

```
SECTION SWEEP — [SECTION NAME] — All Documents [DOC_IDS]

Perform a comprehensive audit of this section:

1. **Gap Analysis:** What important topics are MISSING from this section?
2. **Cross-Reference Check:** What connections to other sections are missing?
3. **Tier Review:** Are any claims rated too high or too low?
4. **Redundancy Check:** Is any content duplicated across documents?
5. **Currency Check:** What major developments (2024-2026) are not reflected?
6. **Structural Audit:** Do all documents follow the standard template?
7. **Image Needs:** What key images are missing?
8. **Bibliography Completeness:** What sources should be added?
9. **Counter-Argument Coverage:** Where are counter-arguments weak or missing?
10. **Connection to Expanded Mission:** How does this section relate to questions of meaning, consciousness, or the nature of reality?
```

---

## 7. IMAGE SOURCE PULL

```
IMAGE PULL — [TOPIC]

I need reference images for [TOPIC]. For each image provide:
| # | Description | Source Site | Direct URL or Search Path | Original Filename | License | Tier |

Rules:
- Only REAL images from museums, archives, or Wikimedia Commons
- Include the ORIGINAL FILENAME as it appears on the source site
- Specify exact search path (e.g., "Met > Search > 'cylinder seal enki' > Object 327009")
- Note Tier: T1 = museum photo of artifact, T2 = published reproduction, T3 = modern interpretation

Priority sources:
1. The Met Open Access (metmuseum.org) — Public Domain
2. British Museum (britishmuseum.org)
3. Wikimedia Commons — CC/PD
4. Louvre Collections (collections.louvre.fr)
5. Smithsonian Open Access
6. CDLI (cuneiform tablets)
7. UNESCO World Heritage
```

---

## 8. PRIMARY SOURCE ANALYSIS

```
PRIMARY SOURCE ANALYSIS — [TEXT/ARTIFACT NAME]

Analyze [TEXT/ARTIFACT] as a primary source:

1. **Original language and dating** — When was it created? In what language?
2. **Provenance** — Where was it found? By whom? Current location?
3. **Translation history** — Who translated it? Are there competing translations?
4. **Key passages relevant to:** [SPECIFIC TOPIC]
5. **Academic consensus** — What do mainstream scholars say about it?
6. **Alternative interpretations** — What do independent researchers claim?
7. **Textual parallels** — What other texts contain similar passages?
8. **Reliability assessment** — How confident can we be in the text's authenticity and translation?
9. **What questions does it answer?** About origins, consciousness, reality, meaning?
10. **What questions does it raise?** What mysteries remain?

Cite specific passages with line/verse numbers where available.
```

---

## 9. SCIENTIFIC LITERATURE REVIEW

```
LITERATURE REVIEW — [SCIENTIFIC TOPIC]

Provide a comprehensive review of peer-reviewed literature on [TOPIC]:

1. **Foundational papers** — The seminal works that established the field
2. **Current state** — What is the consensus as of 2025-2026?
3. **Active debates** — What are researchers currently arguing about?
4. **Recent breakthroughs** — Papers from 2023-2026 that changed understanding
5. **Methodological issues** — What are the limitations of current research?
6. **Replication status** — Have key findings been replicated?
7. **Interdisciplinary connections** — How does this connect to other scientific fields?
8. **Philosophical implications** — What does this research say about reality, consciousness, or existence?
9. **Unanswered questions** — What are the biggest open problems?

Format: Author (Year), Journal, Key Finding, Citation Count if available.
Only cite REAL papers. Say "I cannot verify" if unsure about a citation.
```

---

## 10. PHILOSOPHICAL ANALYSIS

```
PHILOSOPHICAL ANALYSIS — [QUESTION/CONCEPT]

Analyze [CONCEPT] from multiple philosophical traditions:

1. **Western Philosophy** — Ancient Greek through contemporary analytic/continental
2. **Eastern Philosophy** — Hindu, Buddhist, Taoist, Confucian perspectives
3. **Indigenous Philosophies** — Aboriginal, Native American, African, Pacific traditions
4. **Ancient Near Eastern** — Sumerian, Egyptian, Babylonian, Hebrew wisdom traditions
5. **Modern Scientific Philosophy** — What does current science contribute to this question?
6. **Points of convergence** — Where do multiple traditions agree?
7. **Points of divergence** — Where do they fundamentally disagree?
8. **Practical implications** — How does this analysis affect how we should live?
9. **Connection to the "meaning of life" question** — What does this tell us about purpose?
10. **Unresolvable tensions** — What paradoxes or contradictions remain?

Rate each philosophical position: STRONG (well-argued, widely held), MODERATE (defensible, minority), WEAK (logically problematic), UNKNOWN (insufficient evidence).
```

---

## 11. TIMELINE CONSTRUCTION

```
TIMELINE — [TOPIC] — [DATE RANGE]

Construct a comprehensive timeline for [TOPIC] covering [DATE RANGE]:

1. List ALL significant events with:
   - Exact date (or best estimate with uncertainty noted)
   - What happened
   - Who was involved
   - Primary source for the date
   - Tier rating for the dating certainty
   
2. Include:
   - Mainstream accepted events
   - Alternative/disputed events (marked as Tier 2-4)
   - Cross-cultural contemporary events
   - Geological/astronomical context events
   
3. Format as a table:
| Date | Event | Evidence | Tier | Source | Cross-Reference |

4. Note any dating controversies or calibration issues
5. Identify gaps where events SHOULD exist but evidence is missing
```

---

## 12. SYNTHESIS & PATTERN DETECTION

```
SYNTHESIS — [LIST OF TOPICS]

I have research on the following topics: [LIST TOPICS WITH DOC IDS]

Perform a synthesis analysis to detect patterns:

1. **Common elements** — What appears in 3+ of these topics?
2. **Hidden connections** — What connections are NOT obvious at first glance?
3. **Contradictions** — Where do these topics conflict with each other?
4. **Emergent patterns** — What larger pattern emerges when you see all topics together?
5. **Predictions** — Based on these patterns, what ELSE should be true? (testable predictions)
6. **Alternative explanations** — What else could explain these patterns? (coincidence, cognitive bias, shared source, etc.)
7. **Implications for reality** — What does this pattern suggest about the nature of existence?
8. **Research gaps** — What additional research would confirm or refute the pattern?

Be specific. Cite evidence from each topic. Rate each pattern's strength.
```

---

## 13. SOURCE VERIFICATION AUDIT

> **Full prompt with 6 variants available at:** `_scripts/prompts/source_verification_prompt.md`

```
SOURCE VERIFICATION AUDIT — [DOC_ID] — [TOPIC]

You are a FACT-CHECKER, not a research assistant. Your job is to VERIFY, not expand.

I'm going to paste a research document below. For EVERY claim in this document:

1. **VERIFY THE CLAIM** — TRUE / PARTIALLY TRUE / UNVERIFIABLE / FALSE / FABRICATED SOURCE
2. **VERIFY EACH CITATION** — Does this publication actually exist? Is the author real?
3. **CHECK THE TIER RATING** — Should it be higher or lower?
4. **CHECK SOURCE CONFIDENCE** — Does the weighted bibliography score match the [N/5] rating? (journals ×3, academic ×2, other ×1)
5. **FLAG RED FLAGS** — AI-fabricated sources, vague attributions, wrong dates, fake quotes

FORMAT:
### Claim [N.N]: [Title]
- **Status:** [TRUE / PARTIALLY TRUE / UNVERIFIABLE / FALSE / FABRICATED]
- **Tier Check:** [Current] → [Suggested] — [Reason]
- **Citation Verified:** YES / NO / PARTIALLY
- **Issues:** [List]

### BIBLIOGRAPHY VERIFICATION
| # | Author | Title Exists? | Year | Verdict |
|---|--------|--------------|------|---------|

### OVERALL ASSESSMENT
- Confirmed accurate: [N] | Needs correction: [N] | Fabricated sources: [N]

Be RUTHLESS. The goal is accuracy, not politeness.

=== DOCUMENT TO VERIFY BEGINS BELOW ===
[PASTE FULL DOCUMENT]
```

---

*These prompts are tools. Adapt them freely. The goal is always: maximum information, maximum accuracy, maximum honesty, minimum bias.*

---

## 14. MASTER DOC SECTION EVIDENCE REFRESH

```
MASTER DOC SECTION EVIDENCE REFRESH — [FILE NAME] — [SECTION HEADING]

TASK: Audit exactly ONE section of ONE master-reference document at a time.
Do not scan the whole project at once.

INPUTS I WILL PROVIDE:
- File name: [FILE NAME]
- Section heading: [SECTION HEADING]
- Section text pasted below
- Optional: related internal stats or linked docs

YOUR JOB:
1. Separate claims into two buckets:
   - EXTERNAL CLAIMS: statements about history, science, archaeology, genetics, religion, technology, and similar topics
   - INTERNAL PROJECT CLAIMS: corpus counts, section totals, thread counts, document totals, map totals, workflow claims
2. For EXTERNAL CLAIMS, use current authoritative sources where possible:
   - peer-reviewed papers
   - university or museum pages
   - UNESCO, NOAA, NASA, NIH, Smithsonian, Britannica, major archives, official databases
3. For INTERNAL PROJECT CLAIMS, do NOT pretend to externally verify them.
   Instead, mark them as needing an internal consistency check against the corpus.
4. For each claim, classify it as one of:
   - STRENGTHENED
   - MIXED / CONTESTED
   - WEAKENED
   - DISPROVEN
   - INTERNAL-ONLY
   - NEEDS DIRECT CITATION
5. Prioritize new information from 2024-2026 when relevant, but include older foundational sources if they are still the best evidence.
6. Never invent a source. If a claim is plausible but you cannot verify the exact number or wording, say so directly.

REQUIRED OUTPUT FORMAT:

## Section Scanned
- File: [FILE NAME]
- Heading: [SECTION HEADING]

## Claim Review Table
| Claim | Type (External/Internal) | Verdict | What changed or was confirmed | Recommended rewrite |
|---|---|---|---|---|

## Best Sources
- [Source 1: author or organization, title, year, why it matters]
- [Source 2: author or organization, title, year, why it matters]
- [Source 3: author or organization, title, year, why it matters]

## Action Summary
- Which lines are safe to keep as-is
- Which lines should be softened
- Which exact numbers need re-checking
- Which items are actually internal stats and should be validated against project files instead of web sources

RULES:
- Be skeptical
- Distinguish "not proven" from "disproven"
- Do not upgrade speculative claims without source-level support
- If an exact number is not clearly sourced, recommend replacing it with tighter wording
- Keep the output compact and section-scoped

SECTION TEXT:
[PASTE SECTION HERE]
```
