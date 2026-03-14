# Research Methodology & Transparency — Theories of Everything

> **Created:** Mar 14, 2026 | **Last Updated:** Mar 14, 2026
> **Purpose:** Public-facing document explaining how this knowledge base is built, what research methodology is used, and what readers should know about its approach, structure, and limitations.

---

## QUICK REFERENCE

### What This Project Is

| Aspect | Detail |
|--------|--------|
| **Type** | Multi-disciplinary research knowledge base |
| **Scale** | 2,432 documents, 34 sections (A–ZH), ~391,000 lines |
| **Topics** | Origins of life, consciousness, ancient wisdom, cross-cultural patterns, modern science, future of humanity |
| **Approach** | Maps ALL perspectives — mainstream, alternative, skeptical — with standardized reliability ratings |
| **Position** | Does not advocate a single theory |

### Document Template

| Section | Purpose |
|---------|---------|
| Header Block | [N/5] rating, primary tier, date, keywords, tags, cross-refs |
| Quick Summary | 3–6 sentence overview with evidential status |
| Tier 1 — Verified | Peer-reviewed, archaeologically confirmed claims |
| Tier 2 — Credible | Academic, debated but supported |
| Tier 3 — Speculative | Possible but unverified |
| Tier 4 — Dubious | No credible source or contradicted |
| Counter-Arguments | Strongest objections and alternative explanations |
| Images | Table with descriptions, sources, licenses |
| Bibliography | Numbered, academic-format citations |
| Cross-Reference Index | Links to related docs with connection descriptions |

### Interpretive Lenses

| Lens | Approach | Typical Tier Range |
|------|----------|--------------------|
| **Mythic** | Tradition as mythology, archetype, cultural psychology (Jung, Campbell) | Tier 1–2 |
| **Literal** | Tradition as describing real events, entities, or technologies | Tier 2–4 |
| **Symbolic** | Tradition as encoding knowledge in symbolic/allegorical form | Tier 1–3 |

### Automation & Tooling

| Tool | Function |
|------|----------|
| `pipeline.py` | Master pipeline — 6-step quality chain + infrastructure |
| `quality_scorecard.py` | 8-dimension quality scoring per document |
| `factuality_scan.py` | 7-dimension factuality measurement |
| `update_source_ratings_weighted.py` | Classifies bib by source type, assigns [N/5] |
| `build_search_guide.py` | Generates AI-optimized topic routing |
| `formatting_scan.py` | Detects formatting violations corpus-wide |
| `crossref_batch_verify.py` | Validates cross-references point to real docs |
| `isbn_enrichment.py` | Adds ISBNs/DOIs to bib entries |
| `tier_classifier.py` | Identifies misclassified tier ratings |
| `scan_coverage.py` | Maps keyword coverage gaps |
| `source_verifier.py` | 7-API entity/source verification |
| `cross_verifier.py` | Cross-references cached verification data |
| `claim_extractor.py` | Extracts atomic claims from docs |
| `validate_quick.py` | 4-layer validation across full corpus |
| `generate_disclaimer.py` | Generates AI disclaimer footer for documents |

### Corpus Statistics (as of Mar 14, 2026)

| Metric | Value |
|--------|-------|
| Total documents | 2,437 |
| Total sections | 34 (A–ZH) |
| Total lines | ~395,376 |
| Unique indexed keywords | 30,637 |
| Keyword-document links | 46,734+ |
| Unique images | 627+ |
| Quality score | 85.8/100 (A-) |
| Factuality score | 72.4/100 (B-) |
| Thematic threads | 20+ |
| Cross-domain connections | 200+ |
| Interpretive lenses | 3 (Mythic, Literal, Symbolic) |
| Source confidence system | Weighted [N/5] (journals ×3, academic ×2, other ×1) |
| Docs at [5/5] (42+ pts) | 375 (15.4%) |
| Docs at [3/5]+ (22+ pts) | 2,099 (86.3%) |

---

## 1. RESEARCH APPROACH

### 1.1 Multi-Perspective Mapping

This project does not select a single theory and defend it. Instead, it systematically maps:
- **Mainstream scientific consensus** — what the evidence currently supports
- **Alternative hypotheses** — what challenging theories propose, with their evidence
- **Skeptical objections** — what critics say about each claim
- **Historical context** — how understanding has evolved over time

Every topic receives the same structured analysis regardless of whether the content is conventional or controversial. The framework treats evidence quality, not popularity or familiarity, as the measure of reliability.

### 1.2 Cross-Cultural Pattern Evaluation

When a pattern appears across multiple independent cultures, significance is assessed:

| Pattern Frequency | Assessment | Action |
|-------------------|-----------|--------|
| 2 cultures | Could be coincidence or diffusion | Not significant alone |
| 3–4 cultures | Possibly significant — check for contact | Investigate diffusion routes |
| 5–7 cultures | Likely significant — exceeds coincidence | Strong pattern — document fully |
| 8+ independent cultures | Almost certainly meaningful | Major finding — cross-validate |

Alternative explanations are always tested:
1. **Diffusion** — Did cultures learn it from each other?
2. **Common observation** — Would any culture independently notice this? (e.g., snakes exist everywhere)
3. **Cognitive bias** — Does the human brain naturally generate this pattern?
4. **Shared ancestry** — Common ancestral culture or language family?
5. **Real phenomenon** — Physical, astronomical, or geological basis? (e.g., precession → 72 in myths)

### 1.3 Source Type Hierarchy

Evidence is weighted by source quality in this priority order:

| Priority | Source Type | Examples |
|:--------:|------------|---------|
| 1 | Primary texts | Original tablets, manuscripts, codices, inscriptions |
| 2 | Archaeological | Artifacts, sites, stratigraphy, lab analysis |
| 3 | Peer-reviewed | Journal articles, academic monographs |
| 4 | Academic books | Published by credentialed scholars |
| 5 | Popular authors | Hancock, Temple, Narby — useful but lower weight |
| 6 | Testimony | Whistleblowers, witnesses — case-by-case |
| 7 | Internet claims | Forum posts, social media — lowest weight |

---

## 2. DOCUMENT STRUCTURE

Every document in the knowledge base follows an identical template. This ensures that every topic — from ancient Sumerian tablets to quantum physics to consciousness research — is evaluated using the exact same framework.

### 2.1 Header Block

Contains machine-readable metadata:
- **Source confidence** — [N/5] weighted bibliography score
- **Primary tier** — the dominant reliability level of the document's claims
- **Last updated** — date of most recent revision
- **Keywords** — searchable terms for the topic
- **Category tags** — section classification
- **Cross-references** — links to related documents

### 2.2 Content Sections

Each document presents claims organized by evidence strength:
- **Quick Summary** (3–6 sentences) captures the topic and its evidential status
- **Tier 1–4 sections** separate claims by reliability level
- **Counter-Arguments & Criticisms** presents the strongest REAL, PUBLISHED objections. If no real counter-arguments exist for a settled-consensus topic, an honest "no dispute" note is used instead.
- Claims within tiers include specific references to bibliography entries
- Evidence must be specific: exact dates, named scholars in **bold**, measurements with units, institutional attribution, artifact/tablet IDs

### 2.3 Bibliography & Cross-References

- **Bibliography** uses numbered, academic-format citations (minimum 5 entries per document)
- **Source Count** in the header must match the actual number of bibliography entries
- Every significant claim traces to a specific bibliography entry
- **Cross-Reference Index** links to related documents with explanations of how they connect
- Cross-references are bidirectional — if Doc A references Doc B, Doc B should reference Doc A

---

## 3. NON-NEGOTIABLE RULES

These rules are enforced across the entire knowledge base without exception:

| # | Rule | Rationale |
|:-:|------|-----------|
| 1 | **NEVER fabricate sources** | Only cite real, verifiable publications with real authors, titles, publishers, dates |
| 2 | **NEVER delete data** | Move, tag, or contextualize. Debunked claims get `[DEBUNKED]` tags and remain visible |
| 3 | **ALWAYS present real counter-arguments** | If no verifiable CA exists, use an honest "no dispute" note rather than inventing weak objections |
| 4 | **ALWAYS apply tier ratings** | No unrated claims in finalized documents |
| 5 | **ALWAYS use source confidence** | [N/5] based on weighted bibliography score |
| 6 | **ALWAYS include primary sources** | Secondary analysis alone is insufficient |
| 7 | **ALWAYS flag uncertainty** | "UNCERTAIN" or "UNKNOWN" explicitly when warranted |
| 8 | **ALWAYS date claims** | Publication year for all cited sources |
| 9 | **ALWAYS note corrections** | Mark debunked/updated claims with a date |
| 10 | **NEVER present belief as fact** | Even popular claims are rated at their actual tier level |

---

## 4. PIPELINE ARCHITECTURE

### 4.1 Quality Pipeline (6 Steps)

```
Q1 (DOI Enrichment)
 ├→ Q2 (Weighted Ratings)
 └→ Q3 (Crossref Verify) ──→ Q4 (Quality Scorecard)
                           └→ Q5 (Factuality Scan)
                                └→ Q6 (Claim Verify)
```

| Step | Script | Function | Depends On |
|:----:|--------|----------|:----------:|
| Q1 | `targeted_doi_enrichment.py` | Add DOIs to bib entries via CrossRef API | — |
| Q2 | `update_source_ratings_weighted.py` | Classify bibs, assign [N/5] ratings | Q1 |
| Q3 | `crossref_batch_verify.py` | Verify DOIs against CrossRef database | Q1 |
| Q4 | `quality_scorecard.py` | Score 8 quality dimensions | Q3 |
| Q5 | `factuality_scan.py` | Score 7 factuality dimensions | Q3 |
| Q6 | `claim_extractor.py` + `cross_verifier.py` | Extract and verify claims | Q5 |

### 4.2 Infrastructure Pipeline (6+3 Steps)

| Step | Script | Function |
|:----:|--------|----------|
| I1 | `processors/index_generator.py` | Regenerate MASTER_INDEX.md |
| I2 | `processors/index_generator.py` | Regenerate KEYWORD_INDEX.md |
| I3 | `build_search_guide.py` | Regenerate AI_SEARCH_GUIDE.md |
| I6 | `formatting_scan.py` | Check formatting compliance |
| I8 | `regenerate_summaries.py` | Regenerate summaries |
| I9 | `corpus_stats.py` | Update corpus statistics |

### 4.3 Running the Pipeline

```bash
# Full pipeline (infrastructure + quality)
python _scripts/pipeline.py --full

# Quality only
python _scripts/pipeline.py --quality

# Infrastructure only
python _scripts/pipeline.py --infrastructure

# Single step
python _scripts/pipeline.py --step Q3

# Check status
python _scripts/pipeline.py --status
```

---

## 5. WHAT THIS PROJECT IS NOT

**This is not:**
- A definitive authority on any topic
- An endorsement of any worldview, religion, or conspiracy theory
- A substitute for reading primary sources
- Free from errors — AI-assisted research may contain mistakes, hallucinated citations, or incomplete context

**This is:**
- A research compilation connecting ideas across disciplines
- A framework for evaluating claims on their merits
- A tool for finding connections no single discipline can see alone
- Transparent about its own weaknesses and limitations

---

## 6. CONTACT AND CONTRIBUTION

This project is built for the good of humanity. All research is intended to be freely accessible.

- Verify claims against cited sources and report discrepancies
- Suggest new sources or counter-arguments
- Propose topics following the established template — use the canonical prompt at `_scripts/prompts/research_pull_prompt.md` for creating new documents
- Point out hallucinated or fabricated citations
- Discord: https://discord.gg/7VbWTA8t

Share your Prompts and responses or Expanded Topics to help the project grow!

---

## DISCLAIMER

This knowledge base was researched and compiled using **multiple AI sources and search engines**: **Claude (Anthropic), GPT (OpenAI), Gemini (Google), Perplexity**, and academic search engines (Google Scholar, JSTOR, PubMed). The [N/5] source confidence rating uses a weighted scoring system (journals ×3, academic ×2, other ×1). AI-assisted research may contain errors including hallucinated citations, incomplete context, or outdated information. **Always verify claims against the primary sources cited in each document's bibliography.**

---

*This document is part of the _MASTER_REFERENCE system. See FACT_CHECKING.md for verification systems and scoring, SYSTEM_REVIEW.md for system health, and PROJECT_MISSION.md for the mission statement.*
