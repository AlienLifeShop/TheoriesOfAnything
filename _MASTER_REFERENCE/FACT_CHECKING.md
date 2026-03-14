# Fact-Checking & Verification Systems — Theories of Everything

> **Created:** Mar 14, 2026 | **Last Updated:** Mar 14, 2026
> **Purpose:** Complete reference for all fact-checking systems, verification APIs, scoring metrics, and data quality tools used in this knowledge base.

---

## QUICK REFERENCE

### Current Scores

| Metric | Score | Grade | Trend |
|--------|:-----:|:-----:|:-----:|
| **Quality Scorecard** | 85.8/100 | A- | ↑ from 84.6 → 85.6 → 85.8 (xref + header fixes) |
| **Factuality Score** | 72.4/100 | B- | ↑ from 62.9 (C) after scanner + evidence fixes |
| **Validation Errors** | 0 | ✅ | Stable |
| **Validation Warnings** | 0 | ✅ | ↓ from 1,340 → 472 → 0 (CAs + bib format fixed) |

### Quality Dimensions (8 dimensions, 100 pts total)

| Dimension | Weight | Score | Status |
|-----------|:------:|:-----:|:------:|
| Structural Compliance | 15 pts | 100% | ✅ Strong |
| Source Attribution | 15 pts | 80% | ✅ Good |
| Evidence Depth | 15 pts | 85% | ✅ Good |
| Counter-Argument Rigor | 15 pts | 63% | ⚠️ ↑ from 51% (Phase 2 CAs) |
| Bibliography Quality | 15 pts | 94% | ✅ Strong |
| Cross-Referencing | 10 pts | 93% | ✅ Strong |
| Factual Traceability | 10 pts | 82% | ✅ Good |
| Content Completeness | 5 pts | 99% | ✅ Strong |

### Factuality Dimensions (7 dimensions, 100 pts total)

| Dimension | Weight | Score | Status |
|-----------|:------:|:-----:|:------:|
| Tier Weight | 25 pts | 66% | ⚠️ Moderate |
| Bib Breadth | 20 pts | 54% | ⚠️ Low — recalibrated after format fix |
| Bibliography Density | 15 pts | 64% | ⚠️ Moderate |
| Verifiable Sources | 10 pts | 50% | ⚠️ Low |
| Vague Sourcing | 10 pts | 98% | ✅ Excellent |
| Counter-Argument Rigor | 10 pts | 58% | ⚠️ ↑ from 53% (Phase 2 CAs) |
| Evidence Specificity | 10 pts | 53% | ⚠️ Low |

### Source Confidence Distribution

| Rating | Docs | % | Weighted Score Range |
|:------:|:----:|:---:|:--------------------:|
| [5/5] | 375 | 15.4% | 42+ points |
| [4/5] | 858 | 35.3% | 30–41 points |
| [3/5] | 866 | 35.6% | 22–29 points |
| [2/5] | 317 | 13.0% | 14–21 points |
| [1/5] | 16 | 0.7% | < 14 points |

### External Verification APIs

| API | Purpose | Scripts | Rate Limit |
|-----|---------|---------|:----------:|
| **CrossRef** | DOI validation, bib search, retraction detection | crossref_batch_verify, targeted_doi_enrichment, citation_checker | 1.0–1.1s/req |
| **Open Library** | ISBN validation, book metadata | isbn_enrichment, validate_isbns, source_verifier | 0.5–2.0s/req |
| **Wikipedia** | Entity existence, article summaries | source_verifier | 0.5s/req |
| **Wikidata** | Entity lookup (QID, label, description) | source_verifier | 0.3s/req |
| **Semantic Scholar** | Paper search, citation counts | source_verifier | 1.0s/req |
| **OpenAlex** | Author/institution lookup | source_verifier | 0.3s/req |
| **PubMed (NCBI)** | Biomedical literature search | source_verifier | 0.5s/req |
| **DOI Handle** | DOI validity check | source_verifier, citation_checker | implicit |

---

## 1. FOUR-TIER RELIABILITY RATING

Every claim in every document is assigned a reliability tier:

| Tier | Label | Standard | What It Means |
|------|-------|----------|---------------|
| **1** | **VERIFIED** | Peer-reviewed research, primary archaeological evidence, scientific consensus | Well-established. Multiple independent lines of evidence support it. |
| **2** | **CREDIBLE** | Academic work, published research, debated but with scholarly support | Quality evidence behind it but remains debated among experts. |
| **3** | **SPECULATIVE** | Possible but unverified; popular-author level, intriguing but lacking primary evidence | Interesting but not proven. Treat with caution. |
| **4** | **DUBIOUS** | No credible source; contradicted by available evidence; conspiracy-only | No reliable support — may be debunked. Included for completeness, not endorsement. |

**Key rules:**
- The **claim** is rated, not the topic — a single document can contain Tier 1 through Tier 4 claims side by side
- A Tier 2 claim with [5/5] source confidence is stronger than Tier 2 with [2/5]
- Debunked claims receive a `[DEBUNKED]` tag — **never deleted**, only contextualized
- Tiers can change when new evidence emerges — changes are dated
- When uncertain, rate **lower** (more skeptically) rather than higher

---

## 2. SOURCE CONFIDENCE RATING ([N/5] Weighted System)

### Weighted Scoring

| Source Type | Points | Detection Method |
|-------------|:------:|-----------------|
| **Peer-reviewed journal article** | **3** | Journal name, volume/page numbers, DOI with journal context |
| **Academic press book / primary text** | **2** | University press, established academic publisher, translated primary texts |
| **Popular book / website / other** | **1** | Commercial publishers, websites, popular-audience works |

### Rating Thresholds

| Score | Label | Weighted Points | Interpretation |
|:-----:|-------|:---------------:|----------------|
| **[5/5]** | Exceptional | 42+ | Heavily sourced with high-quality evidence |
| **[4/5]** | Strong | 30–41 | Strong academic foundation |
| **[3/5]** | Moderate | 22–29 | Corpus-average sourcing — standard confidence |
| **[2/5]** | Limited | 14–21 | Below-average — verify key claims independently |
| **[1/5]** | Minimal | < 14 | Thinly or weakly sourced — treat with significant caution |

### Source Type Hierarchy

```
1. Primary texts      — Original tablets, manuscripts, codices, inscriptions
2. Archaeological     — Artifacts, sites, stratigraphy, laboratory analysis
3. Peer-reviewed      — Journal articles, academic monographs
4. Academic books     — Published by credentialed scholars
5. Popular authors    — Hancock, Temple, Narby — useful but lower weight
6. Testimony          — Whistleblowers, witnesses — assessed case-by-case
7. Internet claims    — Forum posts, social media — lowest weight
```

---

## 3. BIAS DETECTION CHECKLIST

Every source and claim is evaluated against:

| Check | Red Flag If... |
|-------|---------------|
| Acknowledges counter-evidence? | Ignores all opposing data |
| Methodology transparent? | Hidden or unreproducible methods |
| Uses emotional language? | "THEY don't want you to know" |
| Cites primary sources? | "Ancient texts say..." (no specifics) |
| Author financial incentives? | Book sales, speaking fees driving claims |
| Distinguishes unproven vs. disproven? | Conflates the two |
| Survived peer review? | Never submitted or failed |
| Claim falsifiable? | No possible way to test or disprove |
| Passes Occam's Razor? | Simpler explanation available |
| Same standards to own claims? | Double standard in evidence demands |

**Additional red flags:** Financial incentive to sensationalize, single-source claims as fact, citations that don't check out, retracted publications.

---

## 4. EXTERNAL VERIFICATION APIS (Detailed)

### 4.1 CrossRef API

| Property | Detail |
|----------|--------|
| **Base URL** | `https://api.crossref.org/works` |
| **Endpoints** | `/works/{DOI}` (direct lookup), `/works?query.bibliographic=...` (search) |
| **Used by** | `crossref_batch_verify.py`, `targeted_doi_enrichment.py`, `processors/citation_checker.py` |
| **Data returned** | DOI validation, bibliographic metadata, title/year match, retraction signals |
| **User-Agent** | `TheoriesOfAnythingCrossref/1.0` |
| **Rate limit** | 1.0–1.1s sleep per request |
| **Cache** | `data/crossref_results.json`, `data/doi_crossref_cache.json` |

### 4.2 Open Library API

| Property | Detail |
|----------|--------|
| **Base URLs** | `https://openlibrary.org/search.json` (title), `https://openlibrary.org/isbn/{isbn}.json` (ISBN) |
| **Used by** | `isbn_enrichment.py`, `validate_isbns.py`, `source_verifier.py` |
| **Data returned** | ISBN-to-book validation, title/publisher/date metadata |
| **Rate limit** | 0.5s (isbn_enrichment), exponential backoff (validate_isbns) |
| **Cache** | `data/isbn_cache.json`, `data/verification_cache.json` → `open_library` key |

### 4.3 Wikipedia REST API

| Property | Detail |
|----------|--------|
| **Base URL** | `https://en.wikipedia.org/api/rest_v1/page/summary/{title}` |
| **Used by** | `source_verifier.py` |
| **Data returned** | Article existence, title, description, text extract |
| **Rate limit** | 0.5s/request |
| **Cache** | `data/verification_cache.json` → `wikipedia` key |

### 4.4 Wikidata API

| Property | Detail |
|----------|--------|
| **Base URL** | `https://www.wikidata.org/w/api.php?action=wbsearchentities` |
| **Used by** | `source_verifier.py` |
| **Data returned** | Entity QID, label, description |
| **Rate limit** | 0.3s/request |
| **Cache** | `data/verification_cache.json` → `wikidata` key |

### 4.5 Semantic Scholar API

| Property | Detail |
|----------|--------|
| **Base URL** | `https://api.semanticscholar.org/graph/v1/paper/search` |
| **Used by** | `source_verifier.py` |
| **Data returned** | paperId, title match, year, citation count, venue |
| **Fields** | `title,year,citationCount,venue` |
| **Rate limit** | 1.0s/request (official: 100 req/5min) |
| **Cache** | `data/verification_cache.json` → `semantic_scholar` key |

### 4.6 OpenAlex API

| Property | Detail |
|----------|--------|
| **Base URLs** | `https://api.openalex.org/authors?search=...`, `https://api.openalex.org/institutions?search=...` |
| **Used by** | `source_verifier.py` |
| **Data returned** | Author display_name, works_count, cited_by_count; institution lookup |
| **Rate limit** | 0.3s/request |
| **Cache** | `data/verification_cache.json` → `openalex` key |

### 4.7 PubMed / NCBI E-Utilities

| Property | Detail |
|----------|--------|
| **Base URL** | `https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esearch.fcgi` |
| **Used by** | `source_verifier.py` |
| **Data returned** | Paper search results, PubMed IDs, result counts |
| **Parameters** | `db=pubmed&term=...&retmax=3&retmode=json` |
| **Rate limit** | 0.5s/request |
| **Cache** | `data/verification_cache.json` → `pubmed` key |

### 4.8 DOI Handle Resolution

| Property | Detail |
|----------|--------|
| **Base URLs** | `https://doi.org/api/handles/{DOI}` (handle), `https://doi.org/{DOI}` (HTTP HEAD) |
| **Used by** | `source_verifier.py`, `processors/citation_checker.py` |
| **Data returned** | Validity flag (responseCode == 1 = valid) |
| **Cache** | `data/verification_cache.json` → `doi` key |

---

## 5. IMAGE & COLLECTION APIs

Used by `downloaders/image_downloader.py` via `utils/rate_limiter.py`:

| Source | Base URL | Type | API Key | Rate |
|--------|----------|:----:|:-------:|:----:|
| Metropolitan Museum | `collectionapi.metmuseum.org/public/collection/v1` | API | No | 80/min |
| British Museum | `www.britishmuseum.org/api` | API | No | 30/min |
| Wikimedia Commons | `commons.wikimedia.org/w/api.php` | API | No | 200/min |
| Smithsonian | `api.si.edu/openaccess/api/v1.0` | API | **Yes** | 60/min |
| CORE | `api.core.ac.uk/v3` | API | **Yes** | 60/min |
| arXiv | `export.arxiv.org/api` | API | No | 20/min |
| PubMed Central | `eutils.ncbi.nlm.nih.gov/entrez/eutils` | API | No | 10/min |
| Pleiades | `pleiades.stoa.org` | API | No | 30/min |
| ORACC | `oracc.museum.upenn.edu` | API | No | 20/min |
| CDLI | `cdli.ucla.edu` | API | No | 30/min |
| Louvre | `collections.louvre.fr` | Scrape | No | 20/min |
| ETCSL | `etcsl.orinst.ox.ac.uk` | Scrape | No | 20/min |
| Sacred-Texts | `www.sacred-texts.com` | Scrape | No | 15/min |
| Perseus | `www.perseus.tufts.edu` | Scrape | No | 20/min |
| UNESCO | `whc.unesco.org` | Scrape | No | 10/min |
| Google Scholar | `scholar.google.com` | Scrape | No | 5/min |
| Penn Museum | `www.penn.museum` | Scrape | No | 15/min |
| World History Encyclopedia | `www.worldhistory.org` | Scrape | No | 15/min |

---

## 6. CACHING INFRASTRUCTURE

| Cache File | Fed By | Consumed By |
|------------|--------|-------------|
| `data/crossref_results.json` | crossref_batch_verify, citation_checker | factuality_scan, quality_scorecard, cross_verifier |
| `data/doi_crossref_cache.json` | targeted_doi_enrichment | targeted_doi_enrichment (dedup) |
| `data/isbn_cache.json` | isbn_enrichment | isbn_enrichment (cache-only mode) |
| `data/verification_cache.json` | source_verifier (7 sub-caches) | cross_verifier, claim_scorer |
| `data/isbn_validation.json` | validate_isbns | — |

**verification_cache.json sub-keys:** `wikipedia`, `doi`, `wikidata`, `semantic_scholar`, `openalex`, `open_library`, `pubmed`

---

## 7. SCORING SCRIPTS (Offline — No API Calls)

| Script | Function | Input | Output |
|--------|----------|-------|--------|
| `quality_scorecard.py` | Scores 8 quality dimensions per doc | All 2,432 docs + crossref_results.json | `data/quality_scorecard_report.md`, `data/quality_scorecard.json` |
| `factuality_scan.py` | Scores 7 factuality dimensions per doc | All 2,432 docs + crossref_results.json | `data/factuality_scores.json`, `data/_factuality_out.txt` |
| `claim_extractor.py` | Extracts atomic claims from docs | All 2,432 docs | `data/extracted_claims.json` |
| `claim_scorer.py` | Scores extracted claims on 4 dimensions (source support, tier, verification, specificity) | extracted_claims.json + verification_cache.json | `data/scored_claims.json`, `data/claim_scores_report.md` |
| `claim_linker.py` | Links claims to bibliography entries via 4 methods (bracket_ref, source_line, inline_cite, bold_scholar) | extracted_claims.json + doc bibliographies | `data/linked_claims.json`, `data/claim_links_report.md` |
| `update_source_ratings_weighted.py` | Classifies bib entries, assigns [N/5] ratings | Doc bibliographies | In-place doc updates |
| `cross_verifier.py` | Cross-references cached data for verification report | verification_cache.json, crossref_results.json | `data/source_verification_report.md` |

---

## 8. VALIDATION PIPELINE

The `validate_quick.py` script runs 4 layers of checks across all 2,432 docs:

| Layer | What It Checks |
|-------|---------------|
| **doc_validator** | Required sections present, header format, tier structure |
| **format_compliance** | Markdown formatting, naming convention, image table format |
| **extra_checks** | Cross-reference validity, bibliography numbering, keyword consistency |
| **factuality_gate** | Minimum factuality threshold met, no critical scoring failures |

**Current status:** 0 errors, 0 warnings

---

## 9. NON-NEGOTIABLE RULES

These rules are enforced across the entire knowledge base without exception:

1. **NEVER fabricate sources** — Only cite real, verifiable publications with real authors, titles, publishers, and dates
2. **NEVER delete data** — Move, tag, or contextualize. Debunked claims get `[DEBUNKED]` tags and remain visible
3. **ALWAYS present counter-arguments IF REAL ONES EXIST** — If no verifiable, sourced counter-argument exists, use an honest "no dispute" note rather than inventing weak objections
4. **ALWAYS apply tier ratings** — No unrated claims in any finalized document
5. **ALWAYS use source confidence** — Specify [N/5] based on weighted bibliography score
6. **ALWAYS include primary sources** — Secondary analysis alone is insufficient
7. **ALWAYS flag uncertainty** — Say "UNCERTAIN" or "UNKNOWN" explicitly when warranted
8. **ALWAYS date claims** — Include publication year for all cited sources
9. **ALWAYS note corrections** — Mark debunked/updated claims with a date
10. **NEVER present belief as fact** — Even popular or mainstream claims are rated at their actual tier level
11. **ALWAYS use evidence specificity** — Exact dates, named scholars in **bold**, measurements with units, institutional attribution, artifact/tablet IDs
12. **ALWAYS ensure Source Count matches** — The header Source Count must equal the actual number of bibliography entries (minimum 5)
13. **USE THE CANONICAL PROMPT** — For new document creation, always use `_scripts/prompts/research_pull_prompt.md`

---

## 10. HOW TO EVALUATE WHAT YOU READ HERE

1. **Check the tier rating** — Tier 1 = peer-reviewed evidence. Tier 4 = explicitly dubious.
2. **Check source confidence** — [5/5] = 42+ weighted points (exceptional). [1/5] = < 14 points (minimal).
3. **Read the counter-arguments** — Every document includes the strongest objections.
4. **Follow the bibliography** — Look up the original papers, books, or reports yourself.
5. **Notice the interpretive lens** — Mythic, Literal, or Symbolic? The lens changes the tier.
6. **Cross-check dates** — A claim from 2005 may be overturned by 2025.
7. **Apply your own judgment** — This project presents evidence. The conclusions are yours.

---

## DISCLAIMER

This knowledge base was researched and compiled using **multiple AI sources and search engines**: **Claude (Anthropic), GPT (OpenAI), Gemini (Google), Perplexity**, and academic search engines (Google Scholar, JSTOR, PubMed). The [N/5] source confidence rating uses a weighted scoring system (journals ×3, academic ×2, other ×1). AI-assisted research may contain errors including hallucinated citations, incomplete context, or outdated information. **Always verify claims against the primary sources cited in each document's bibliography.**

---

*This document is part of the _MASTER_REFERENCE system. See METHODOLOGY.md for research methodology, SYSTEM_REVIEW.md for system health, and PROJECT_MISSION.md for the mission statement.*
