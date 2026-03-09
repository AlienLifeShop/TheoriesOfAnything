# Methodology, Fact-Checking, and Transparency — Theories of Everything

> **Created:** Mar 8, 2026 | **Last Updated:** Mar 8, 2026
> **Purpose:** Public-facing document explaining how this knowledge base is built, how claims are evaluated, what fact-checking systems are in place, and what readers should know about its reliability and limitations.

---

## 1. WHAT THIS PROJECT IS

**Theories of Anything** is a multi-disciplinary research knowledge base containing **1,071 documents** across **32 sections** (A–ZF) with **~239,000 lines** of research. It investigates the origin and meaning of life, the nature of reality and consciousness, ancient wisdom, cross-cultural patterns, modern science, and the future of humanity.

The project does not advocate a single theory. It maps ALL perspectives — mainstream, alternative, and skeptical — and rates every claim on a standardized reliability scale so readers can evaluate evidence on its merits.

---

## 2. THE FACT-CHECKING SYSTEM

### 2.1 Four-Tier Reliability Rating

Every claim in every document is assigned a reliability tier:

| Tier | Label | Standard | What It Means |
|------|-------|----------|---------------|
| **1** | **VERIFIED** | Peer-reviewed research, primary archaeological evidence, scientific consensus | This claim is well-established. Multiple independent lines of evidence support it. |
| **2** | **CREDIBLE** | Academic work, published research, debated but with scholarly support | This claim has quality evidence behind it but remains debated among experts. |
| **3** | **SPECULATIVE** | Possible but unverified; popular-author level, intriguing but lacking primary evidence | This claim is interesting but not proven. Treat with caution. |
| **4** | **DUBIOUS** | No credible source; contradicted by available evidence; conspiracy-only | This claim has no reliable support and may be debunked. Included for completeness, not endorsement. |

**Key rules:**
- The **claim** is rated, not the topic — a single document can contain Tier 1 through Tier 4 claims side by side
- A Tier 2 claim with [5/5] source confidence is treated as stronger than Tier 2 with [2/5]
- Claims that have been debunked receive a `[DEBUNKED]` tag — they are **never deleted**, only contextualized
- Tiers can change when new evidence emerges — changes are dated
- When uncertain, we rate **lower** (more skeptically) rather than higher

### 2.2 Source Confidence Rating ([N/5] Weighted System)

The project rates every document's evidential strength using a **weighted bibliography scoring system**. Each bibliography entry is automatically classified by source type and assigned a point value:

| Source Type | Points | Detection Method |
|-------------|--------|-----------------|
| **Peer-reviewed journal article** | **3 points** | Journal name, volume/page numbers, DOI with journal context |
| **Academic press book / primary text** | **2 points** | University press, established academic publisher, translated primary texts |
| **Popular book / website / other** | **1 point** | Commercial publishers, websites, popular-audience works |

The weighted score (not the raw count) determines the [N/5] rating:

| Score | Label | Weighted Score | Interpretation |
|-------|-------|---------------|----------------|
| **[5/5]** | **Exceptional** | 42+ points | Heavily sourced with high-quality evidence |
| **[4/5]** | **Strong** | 30–41 points | Strong academic foundation |
| **[3/5]** | **Moderate** | 22–29 points | Corpus-average sourcing — standard confidence |
| **[2/5]** | **Limited** | 14–21 points | Below-average — verify key claims independently |
| **[1/5]** | **Minimal** | < 14 points | Thinly or weakly sourced — treat with significant caution |

**Why weighted scoring:**
- **Quality matters** — A document citing 8 peer-reviewed *Nature* articles (24 points) scores higher than one citing 15 popular-author books (15 points). Credit goes where it's due.
- **Verifiable** — Anyone can check the bibliography entries and their types. The `update_source_ratings_weighted.py` script classifies entries automatically and produces a full breakdown.
- **Balanced** — The system produces a bell-curve distribution centered on [3/5], with roughly equal numbers above and below the median.
- **Improvable** — Adding a peer-reviewed journal article to a bibliography adds 3 points. Adding a popular book adds 1. The incentive structure rewards finding better evidence.

**Important:** The weighted score measures *quantity weighted by quality* of bibliography entries. The **Tier system** (Section 2.1) evaluates the *content quality* of claims themselves. Together they give a complete picture: a [4/5] document with mostly Tier 3–4 claims is well-sourced but speculative. A [2/5] document with all Tier 1 claims is thinly sourced but verified.

### 2.3 Source Type Hierarchy

Evidence is weighted by source quality, in this priority order:

```
1. Primary texts      — Original tablets, manuscripts, codices, inscriptions
2. Archaeological     — Artifacts, sites, stratigraphy, laboratory analysis
3. Peer-reviewed      — Journal articles, academic monographs
4. Academic books     — Published by credentialed scholars
5. Popular authors    — Hancock, Temple, Narby — useful but lower weight
6. Testimony          — Whistleblowers, witnesses — assessed case-by-case
7. Internet claims    — Forum posts, social media — lowest weight
```

### 2.4 Bias Detection Checklist

Every source and claim is evaluated against these criteria:

- Does the source acknowledge counter-evidence?
- Is the methodology transparent and reproducible?
- Does it use emotional manipulation or fear-based language?
- Does it cite primary sources with specific references?
- Does the author have financial incentives (book sales, speaking fees, clicks)?
- Does it distinguish between "unproven" and "disproven"?
- Have the key claims survived peer review?
- Is the claim falsifiable (can it in principle be proven wrong)?
- Does it pass Occam's Razor (is a simpler explanation available)?
- Does the author apply the same evidentiary standards to their own claims as to others'?

**Red flags** that lower confidence:
- Financial incentive to sensationalize
- No primary source citation ("ancient texts say..." without specifying which)
- Emotional manipulation language ("THEY don't want you to know")
- Single-source claims presented as fact
- Citations that don't check out when verified
- Retracted publications

---

## 3. INTERPRETIVE FRAMEWORK

Ancient and contested claims are analyzed through three lenses:

| Lens | Approach | Typical Tier Range |
|------|----------|--------------------|
| **Mythic** | The tradition as mythology, archetype, or cultural psychology (Jung, Campbell) | Tier 1–2 |
| **Literal** | The tradition as describing real events, entities, or technologies | Tier 2–4 |
| **Symbolic** | The tradition as encoding knowledge in symbolic or allegorical form | Tier 1–3 |

Every analysis states which lens is being applied. Most Tier 1–2 claims use the Mythic or Symbolic lens. Literal interpretations are typically Tier 3–4 unless directly supported by physical evidence.

---

## 4. CROSS-CULTURAL PATTERN EVALUATION

When a pattern appears across multiple independent cultures, significance is assessed:

| Pattern Frequency | Assessment | Action |
|-------------------|-----------|--------|
| 2 cultures | Could be coincidence or cultural diffusion | Not significant alone |
| 3–4 cultures | Possibly significant — check for historical contact | Investigate diffusion routes |
| 5–7 cultures | Likely significant — exceeds coincidence threshold | Strong pattern — document fully |
| 8+ independent cultures | Almost certainly meaningful | Major finding — cross-validate all evidence |

Alternative explanations are always tested:
1. **Diffusion** — Did cultures learn it from each other?
2. **Common observation** — Would any culture independently notice this? (e.g., snakes exist everywhere)
3. **Cognitive bias** — Does the human brain naturally generate this pattern? (e.g., Snake Detection Theory)
4. **Shared ancestry** — Does this trace to a common ancestral culture or language family?
5. **Real phenomenon** — Is there a physical, astronomical, or geological basis? (e.g., precession → the number 72 in myths)

---

## 5. DOCUMENT STRUCTURE

Every document in the knowledge base follows an identical template:

| Section | Purpose |
|---------|---------|
| **Header Block** | Source confidence rating [N/5], primary tier, last updated date, keywords, category tags, cross-references |
| **Quick Summary** | 3–6 sentence overview of the topic and its evidential status |
| **Tier 1 — Verified** | Peer-reviewed, archaeologically confirmed claims |
| **Tier 2 — Credible** | Academic, debated but supported claims |
| **Tier 3 — Speculative** | Possible but unverified claims |
| **Tier 4 — Dubious** | No credible source or contradicted by evidence |
| **Counter-Arguments** | The strongest objections and alternative explanations for major claims |
| **Images** | Table of associated images with descriptions, sources, and licenses |
| **Bibliography** | Numbered, academic-format citations of all sources used |
| **Cross-Reference Index** | Links to related documents across the knowledge base with connection descriptions |

This structure ensures that every topic — whether ancient Sumerian tablets, quantum physics, consciousness research, or mythology — is evaluated using the exact same framework.

---

## 6. NON-NEGOTIABLE RULES

These rules are enforced across the entire knowledge base without exception:

1. **NEVER fabricate sources** — Only cite real, verifiable publications with real authors, titles, publishers, and dates
2. **NEVER delete data** — Move, tag, or contextualize claims, but never erase them. Debunked claims get `[DEBUNKED]` tags and remain visible
3. **ALWAYS present counter-arguments** — Every major claim requires its strongest opposition documented alongside it
4. **ALWAYS apply tier ratings** — No unrated claims in any finalized document
5. **ALWAYS use source confidence** — Specify [N/5] based on weighted bibliography score (journals ×3, academic ×2, other ×1)
6. **ALWAYS include primary sources** — Secondary analysis alone is insufficient
7. **ALWAYS flag uncertainty** — Say "UNCERTAIN" or "UNKNOWN" explicitly when warranted
8. **ALWAYS date claims** — Include publication year for all cited sources
9. **ALWAYS note corrections** — If a claim is debunked or updated, mark the change with a date
10. **NEVER present belief as fact** — Even popular or mainstream claims are rated at their actual tier level

---

## 7. QUALITY METRICS AND SCORING

The project uses automated quality scoring tools to measure document and corpus-level quality:

### 7.1 Quality Scorecard

Each document is scored across eight weighted dimensions:
- **Structural Compliance** (15 pts) — Does it have all required sections (header, all 4 tiers, counter-arguments, bibliography, cross-references)?
- **Source Attribution** (15 pts) — Are claims linked to specific bibliography entries?
- **Evidence Depth** (15 pts) — Quality and depth of evidential support
- **Counter-Argument Rigor** (15 pts) — Are counter-arguments substantive, not token?
- **Bibliography Quality** (15 pts) — Number and quality of cited sources
- **Cross-Referencing** (10 pts) — Number of connections to other documents
- **Factual Traceability** (10 pts) — Can claims be traced to verifiable sources?
- **Content Completeness** (5 pts) — Is the document thorough on its topic?

**Current corpus quality score:** 77.18/100 (B) — measured across all 1,071 documents

### 7.2 Factuality Scoring

A separate factuality scan measures evidential rigor:

| Dimension | What It Measures | Current Score |
|-----------|-----------------|---------------|
| **Tier Weight** (25 pts) | Are most claims appropriately rated at Tier 1–2? | 65% |
| **Source Confidence** (20 pts) | Bibliography count and quality-based scoring | 63% |
| **Bibliography Density** (15 pts) | Are enough sources cited per document? | 71% |
| **Verifiable Sources** (10 pts) | Can cited sources be independently verified (DOI/ISBN presence)? | 53% |
| **Vague Sourcing** (10 pts) | Absence of vague attribution ("some researchers say...") | 92% |
| **Counter-Argument Rigor** (10 pts) | Are counter-arguments substantive, not token? | 70% |
| **Evidence Specificity** (10 pts) | Are claims backed by specific data, dates, and names? | 64% |

**Current factuality score:** 67.6/100 (C+)

These scores are tracked over time and used to prioritize improvement efforts. The gap between structural quality (B) and factuality (C+) reflects that it is easier to have the right format than to have perfect evidence — an honest assessment that drives ongoing improvement.

---

## 8. AUTOMATION AND TOOLING

The knowledge base is supported by purpose-built scripts:

| Tool | Function |
|------|----------|
| **run_pipeline.py** | Master pipeline — rebuilds indexes, runs audits, checks citations |
| **quality_scorecard.py** | Scores every document across eight quality dimensions (structure, attribution, evidence, counter-arguments, bibliography, cross-referencing, traceability, completeness) |
| **factuality_scan.py** | Measures evidential rigor across seven dimensions |
| **update_source_ratings_weighted.py** | Classifies bibliography entries by source type (journal/academic/other), calculates weighted scores, and assigns [N/5] source confidence ratings |
| **build_search_guide.py** | Generates AI-optimized routing document for rapid topic lookup |
| **formatting_scan.py** | Detects formatting violations across the corpus |
| **crossref_batch_verify.py** | Validates that cross-references point to real documents |
| **isbn_enrichment.py** | Adds ISBNs and DOIs to bibliography entries |
| **tier_classifier.py** | Identifies misclassified tier ratings |
| **scan_coverage.py** | Maps keyword coverage gaps across sections |

These tools run regularly to catch errors, formatting drift, and quality degradation before they accumulate.

---

## 9. WHAT THIS PROJECT IS NOT

**This is not:**
- A definitive authority on any topic
- An endorsement of any particular worldview, religion, or conspiracy theory
- A substitute for reading primary sources
- Free from errors — AI-assisted research may contain mistakes, hallucinated citations, or incomplete context

**This is:**
- A research compilation that connects ideas across disciplines
- A framework for evaluating claims on their merits
- A tool for finding connections that no single discipline can see alone
- Transparent about its own weaknesses and limitations

---

## 10. HOW TO EVALUATE WHAT YOU READ HERE

When reading any document in this knowledge base:

1. **Check the tier rating** — Tier 1 claims have peer-reviewed evidence. Tier 4 claims are explicitly flagged as dubious.
2. **Check the source confidence** — [5/5] means 42+ weighted points from quality-classified bibliography entries (exceptional). [1/5] means fewer than 14 weighted points (minimal). Higher-quality sources (journals, academic press) earn more points.
3. **Read the counter-arguments** — Every document includes the strongest objections. If the counter-arguments are convincing, so be it.
4. **Follow the bibliography** — Every claim should have a cited source. Look up the original papers, books, or archaeological reports yourself.
5. **Notice the interpretive lens** — Is the claim being evaluated as literal history, symbolic encoding, or cultural mythology? The lens changes the tier.
6. **Cross-check dates** — Science advances. A claim from 2005 may have been updated or overturned by 2025. Check when sources were published.
7. **Apply your own judgment** — This project raises questions and presents evidence. The conclusions are yours to draw.

---

## 11. CORPUS STATISTICS (as of Mar 8, 2026)

| Metric | Value |
|--------|-------|
| Total documents | 1,071 |
| Total sections | 32 (A–ZF) |
| Total lines of research | ~239,000 |
| Unique indexed keywords | 17,185 |
| Keyword-document links | 22,995 |
| Unique images | 627+ |
| Quality score | 77.18/100 (B) |
| Factuality score | 67.6/100 (C+) |
| Thematic threads mapped | 20+ |
| Cross-domain connections | 200+ |
| Source confidence system | Weighted bibliography scoring [N/5] (journals ×3, academic ×2, other ×1; median ≈ 28 pts) |
| Documents at [5/5] (42+ weighted pts) | ~179 (16.7%) |
| Documents at [3/5]+ (22+ weighted pts) | ~831 (77.6%) |
| Interpretive lenses applied | 3 (Mythic, Literal, Symbolic) |

---

## 12. CONTACT AND CONTRIBUTION

This project is built for the good of humanity. All research is intended to be freely accessible. If you find errors, have corrections, or want to contribute:

- Verify claims against their cited sources and report discrepancies
- Suggest new sources or counter-arguments
- Propose topics for new documents following the established template
- Point out hallucinated or fabricated citations so they can be corrected
- 
---

## DISCLAIMER

This knowledge base was researched and compiled using **multiple AI sources and search engines**, including but not limited to: **Claude (Anthropic), GPT (OpenAI), Gemini (Google), Perplexity, and conventional academic search engines** (Google Scholar, JSTOR, PubMed).

**The [N/5] source confidence rating** on each document uses a **weighted scoring system** where peer-reviewed journal articles count for 3 points, academic press books for 2 points, and other sources for 1 point. This rewards quality, not just quantity — a document citing *Nature* articles scores higher than one citing only popular-author books. Ratings are assigned automatically by `update_source_ratings_weighted.py` and can be verified by checking any document's bibliography.

**AI-assisted research may contain errors**, including hallucinated citations, incomplete context, or outdated information. This project exists to connect dots and raise questions, not to provide final answers.

**Always verify claims against the primary sources cited in each document's bibliography.**

---

*This document is part of the _MASTER_REFERENCE system. See PROJECT_MISSION.md for the full mission statement, RESEARCH_METHODOLOGY.md for detailed quality standards, and STYLE_GUIDE.md for formatting rules.*
