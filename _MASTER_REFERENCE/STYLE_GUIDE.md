# Style Guide — Document Formatting Standards

> **Last Updated:** Mar 8, 2026
> **Purpose:** Quick reference for creating and formatting documents in the knowledge base

---

## DOCUMENT TEMPLATE

Every content document MUST follow this structure:

```markdown
# [ID] — [Full Title]

> **Source Count:** [N] | **Weighted Score:** [N] | **Source Confidence:** [N/5] | **Primary Tier:** [N] or [N–N] | **Last Updated:** [Month Day, Year]
> **Keywords:** comma, separated, relevant, terms
> **Cross-References:** [DocID — Short Name](relative/path.md) · [DocID](relative/path.md)

---

## QUICK SUMMARY

[Single paragraph — 3-6 sentences. What the topic IS, key evidence, tier assessment.]

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Archaeological Record)

### 1.1 [Claim Title] [N/5 sources]
- Evidence
- Source citations

---

## 2. CREDIBLE CLAIMS (Tier 2 — Academic / Debated but Supported)

### 2.1 [Claim Title] [N/5 sources]

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Possible but Unverified)

### 3.1 [Claim Title] [N/5 sources]

---

## 4. DUBIOUS CLAIMS (Tier 4 — No Credible Source / Contradicted by Evidence)

### 4.1 [Claim Title] [N/5 sources]

---

## IMAGES

| # | Description | Filename | Source | License |
|---|-------------|----------|--------|---------|

---

## BIBLIOGRAPHY

1. Author. *Title*. Publisher, Year.

---

## CROSS-REFERENCE INDEX

| Related Doc | Connection |
|-------------|-----------|
| [XX#](path) | Brief description |

---

*Consolidated from [sources]. Last Updated: [date]*
```

---

## FORMATTING RULES

### Headers
- `#` — Document title only (one per document)
- `##` — Main sections (Tier sections, IMAGES, BIBLIOGRAPHY, etc.)
- `###` — Individual claims or subsections

### Tags & Labels
- Source confidence: `[N/5]` based on weighted bibliography scoring (peer-reviewed journal = 3 pts, academic press/primary text = 2 pts, popular/other = 1 pt). Thresholds: < 14 = [1/5], 14–21 = [2/5], 22–29 = [3/5], 30–41 = [4/5], 42+ = [5/5]
- Tier inline: `(Tier N)` or `(Tier N–N)`
- Key findings: `[KEY FINDING]` 
- Debunked: `**[DEBUNKED]** Claim — Explanation`
- Review needed: `<!-- REVIEW: note -->`

### Tables
Use markdown pipe tables for comparisons, catalogs, and timelines.

### Blockquotes
Use `>` for paraphrased primary-text quotes.

### Links
Use relative paths: `[A01](../A_Foundations/A01_Sumerian_Texts_and_Tablets.md)`

---

## FILE NAMING

```
[SectionLetter][TwoDigitNumber]_Short_Descriptive_Name.md
```

- Section letter: A–ZF (uppercase)
- Number: Two-digit, zero-padded (01, 02, 03)
- Name: Underscores between words, Title_Case
- No spaces, max ~50 characters for name portion
- Sequential within section, no gaps

### Good Examples
```
A01_Sumerian_Texts_and_Tablets.md       ✓
P01_Meaning_of_Life_Frameworks.md       ✓
Q03_Dark_Matter_Dark_Energy.md          ✓
```

### Bad Examples
```
a1_sumerian.md                          ✗ (lowercase, single digit)
A - Sumerian Texts.md                   ✗ (spaces)
meaning_of_life.md                      ✗ (no section letter or number)
```

---

## IMAGE NAMING

```
[SectionLetter][DocNumber]_[descriptive_name].[ext]
```

Example: `A01_eridu_genesis_tablet.jpg`, `Q01_cosmic_web_simulation.png`

---

*See ORGANIZATION_RULES.md for complete rules. See RESEARCH_METHODOLOGY.md for tier and quality standards.*
