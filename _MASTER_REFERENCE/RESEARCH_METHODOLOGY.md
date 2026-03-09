# Research Methodology — Standards & Quality Framework

> **Created:** Feb 27, 2026 | **Last Updated:** Mar 8, 2026
> **Purpose:** Complete reference for the reliability system, source evaluation, bias detection, and quality standards used across the entire knowledge base.

---

## 1. THE FOUR-TIER RATING SYSTEM

| Tier | Label | Criteria | Example Claims |
|---|---|---|---|
| **1 — VERIFIED** | Peer-reviewed, primary texts, archaeological evidence with mainstream consensus | Sumerian tablets exist, DNA structure, Göbekli Tepe dating, quantum entanglement verified |
| **2 — CREDIBLE** | Academic work, published research, debated but with scholarly support | Sphinx water erosion (Schoch), Orch-OR consciousness (Penrose/Hameroff), Younger Dryas impact |
| **3 — SPECULATIVE** | Possible but unverified; intriguing, popular-author level, lacking primary evidence | Atlantis as historical place, DNA/shamanism connection (Narby), Taurid celestial serpent mythology |
| **4 — DUBIOUS** | No credible source; contradicted by evidence; conspiracy-only | Shapeshifting reptilian leaders, Rh-negative as alien blood, literal Nibiru planet |

### Rating Rules
- Rate the **CLAIM**, not the topic — one document can span all four tiers
- A Tier 2 claim with [5/5] source confidence is stronger than Tier 2 with [2/5]
- Debunked claims stay with **[DEBUNKED]** tag — NEVER deleted
- Tiers can change with new evidence — always note date of change
- When in doubt, rate LOWER (more skeptical) rather than higher

---

## 2. SOURCE CONFIDENCE SYSTEM (WEIGHTED)

Every document receives a source confidence rating based on a **weighted bibliography scoring system** where higher-quality sources count for more:

| Source Type | Points | Examples |
|-------------|--------|---------|
| **Peer-reviewed journal** | **3 pts** | *Nature*, *Science*, *PNAS*, academic journals with volume/page |
| **Academic press book / primary text** | **2 pts** | University press, Routledge, Springer, translated primary texts |
| **Popular book / website / other** | **1 pt** | Commercial publishers, websites, popular-audience works |

The weighted score determines the [N/5] rating:

| Rating | Label | Weighted Score | Interpretation |
|---|---|---|---|
| **[5/5]** | Exceptional | 42+ points | Heavily sourced with high-quality evidence |
| **[4/5]** | Strong | 30–41 points | Strong academic foundation |
| **[3/5]** | Moderate | 22–29 points | Corpus-average sourcing — standard confidence |
| **[2/5]** | Limited | 14–21 points | Below-average — verify key claims independently |
| **[1/5]** | Minimal | < 14 points | Thinly or weakly sourced — treat with significant caution |

Ratings are assigned automatically by `update_source_ratings_weighted.py`. The weighted median is 28 points (corresponding to [3/5]).

**Note:** The weighted score measures *quantity weighted by quality*. The Tier system (Section 1) evaluates claim content; this system evaluates source strength. Together they give a complete picture.

---

## 3. SOURCE TYPE HIERARCHY

When evaluating evidence, weight sources in this order:

```
1. Primary texts (original tablets, manuscripts, codices)
2. Archaeological evidence (artifacts, sites, stratigraphy)
3. Peer-reviewed academic analysis (journals, monographs)
4. Academic books by credentialed scholars
5. Popular-author interpretations (Hancock, Temple, Narby)
6. Whistleblower/testimony (Grusch, Fravor — assessed case-by-case)
7. Internet claims and forum posts
```

### Red Flags in Sources
- Financial incentive to sensationalize (book sales, clicks, speaking fees)
- No primary source citation (just "ancient texts say...")
- Emotional manipulation language ("THEY don't want you to know")
- Single-source claims presented as fact
- Citations that don't check out
- Publications that have been retracted

---

## 4. INTERPRETIVE LENSES

When analyzing claims about non-human beings, supernatural events, or ancient accounts, apply three lenses:

| Lens | Approach | Typical Tier |
|---|---|---|
| **Mythic** | The tradition as mythology, archetype, cultural psychology (Jung, Campbell) | 1-2 |
| **Literal** | The tradition as describing real events, entities, or technologies | 2-4 |
| **Symbolic** | The tradition as encoding knowledge in symbolic/allegorical form | 1-3 |

**Rule:** Always state which lens is being applied. Most Tier 1-2 claims use the Mythic or Symbolic lens. Literal interpretations are typically Tier 3-4 unless directly supported by physical evidence.

---

## 5. BIAS DETECTION CHECKLIST

Apply to every source and every claim:

- [ ] Does the source acknowledge counter-evidence?
- [ ] Is the methodology transparent and reproducible?
- [ ] Does it use emotional manipulation or fear?
- [ ] Does it cite primary sources with specific references?
- [ ] Does the author have financial incentives?
- [ ] Does it distinguish between "unproven" and "disproven"?
- [ ] Have key claims survived peer review?
- [ ] Is the claim falsifiable? (Can it in principle be proven wrong?)
- [ ] Does it pass Occam's Razor? (Is a simpler explanation available?)
- [ ] Does the author apply the same standards to their own claims as to their opponents'?

---

## 6. CROSS-CULTURAL PATTERN EVALUATION

When a pattern appears across multiple independent cultures:

| Pattern Frequency | Significance | Example |
|---|---|---|
| 2 cultures | Could be coincidence or diffusion | Not significant alone |
| 3-4 cultures | Possibly significant — check for contact | Warrants investigation |
| 5-7 cultures | Likely significant — exceeds coincidence | Strong pattern |
| 8+ independent cultures | Almost certainly meaningful | Knowledge-giver archetype (13/13) |

### Alternative Explanations to Test
1. **Diffusion** — Did cultures A learn it from culture B?
2. **Common observation** — Is this something any culture would notice? (e.g., serpents are everywhere)
3. **Cognitive bias** — Does the human brain naturally generate this pattern? (Snake Detection Theory)
4. **Shared ancestry** — Does this trace to a common ancestral culture?
5. **Real phenomenon** — Is there a physical/astronomical/geological basis? (e.g., precession → number 72)

---

## 7. NON-NEGOTIABLE RULES

1. **NEVER delete data** — Move, tag, or contextualize, but never erase
2. **NEVER fabricate sources** — Cite only real, verifiable publications
3. **ALWAYS present counter-arguments** — Every major claim needs its strongest opposition
4. **ALWAYS apply tier ratings** — No unrated claims in final documents
5. **ALWAYS use source confidence** — Specify [N/5] based on weighted bibliography score (journals ×3, academic ×2, other ×1)
6. **ALWAYS include primary sources** — Secondary analysis is insufficient alone
7. **ALWAYS flag uncertainty** — Say "UNCERTAIN" or "UNKNOWN" explicitly when warranted
8. **ALWAYS date claims** — Include publication year for all sources
9. **ALWAYS note corrections** — If a claim is debunked, mark it; never just remove it
10. **NEVER present belief as fact** — Even popular claims are marked with their actual tier

---

## 8. DOCUMENT QUALITY CHECKLIST

| Element | Required | Status Check |
|---|---|---|
| Header block (Source Confidence [N/5], Primary Tier, Last Updated, Keywords, Cross-References) | YES | |
| QUICK SUMMARY (single paragraph, 3-6 sentences) | YES | |
| Tier 1 section (or note "No claims at this tier level") | YES | |
| Tier 2 section | YES | |
| Tier 3 section | YES | |
| Tier 4 section | YES | |
| Source confidence tags [N/5] on individual claims | YES | |
| Counter-arguments for major claims | YES | |
| IMAGES table | YES | |
| BIBLIOGRAPHY (numbered, academic format) | YES | |
| CROSS-REFERENCE INDEX table | YES | |
| Footer with consolidation date | YES | |

---

*This methodology applies equally to ancient Sumerian tablets, quantum physics papers, consciousness research, and philosophical arguments. The standard is consistency: every claim is evaluated by the same framework, regardless of whether it's mainstream or alternative.*
