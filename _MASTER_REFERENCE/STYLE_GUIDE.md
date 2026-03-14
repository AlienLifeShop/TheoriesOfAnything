# Style Guide — Document Formatting Standards

> **Last Updated:** Jun 14, 2025
> **Purpose:** Quick reference for creating and formatting documents in the knowledge base

---

## DOCUMENT TEMPLATE

Every content document MUST follow this structure:

```markdown
# [ID] — [Full Title]

> **Source Count:** [N] | **Weighted Score:** [N] | **Source Confidence:** [N/5] | **Primary Tier:** [N] or [N–N] | **Last Updated:** [Month Day, Year]
> **Keywords:** comma, separated, relevant, terms
> **Category Tags:** section-tag, sub-category, topic-tag (max 6)
> **Cross-References:** [DocID — Short Name](relative/path.md) · [DocID](relative/path.md)

---

## QUICK SUMMARY

[Single paragraph — 3-6 sentences. What the topic IS, key evidence, tier assessment.]

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Archaeological Record)

### 1.1 [Claim Title]
- Evidence
- Source citations

---

## 2. CREDIBLE CLAIMS (Tier 2 — Academic / Debated but Supported)

### 2.1 [Claim Title]

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Possible but Unverified)

### 3.1 [Claim Title]

---

## 4. DUBIOUS CLAIMS (Tier 4 — No Credible Source / Contradicted by Evidence)

### 4.1 [Claim Title]

---

## Counter-Arguments & Criticisms

[Strongest REAL, PUBLISHED counter-arguments to the document's major claims.
Each must cite a specific scholar or publication.

If the topic is settled consensus with no real dispute, use:
"No significant counter-arguments exist in the scholarly literature for the core claims in this document. [Topic Name] represents established [field] consensus with no active scholarly dispute over the fundamental claims presented here."

NEVER invent weak objections.]

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
- Source confidence: `[N/5]` in the document header only, based on weighted bibliography scoring (peer-reviewed journal = 3 pts, academic press/primary text = 2 pts, popular/other = 1 pt). Thresholds: < 14 = [1/5], 14–21 = [2/5], 22–29 = [3/5], 30–41 = [4/5], 42+ = [5/5]. Do NOT place `[N/5 sources]` tags on individual claim headers — the rating applies to the document as a whole, not per-claim.
- Tier inline: `(Tier N)` or `(Tier N–N)`
- Key findings: `[KEY FINDING]` 
- Debunked: `**[DEBUNKED]** Claim — Explanation`
- Review needed: `<!-- REVIEW: note -->`

### Tables
Use markdown pipe tables for comparisons, catalogs, and timelines.

### Blockquotes
Use `>` for paraphrased primary-text quotes.

### Links
Use relative paths: `[A_1_01](../A_Foundations/A1_Mesopotamian_Near_Eastern/A_1_01_Sumerian_Texts_and_Tablets.md)`

### Evidence Specificity
Every claim must include specific, verifiable details:
- **Specific dates:** "in 1953" not "in the mid-20th century"
- **Named scholars in bold:** "**Robert Schoch** proposed" not "some researchers suggest"
- **Measurements with units:** "2.3 million blocks averaging 2.5 tonnes each" not "many large blocks"
- **Institutional attribution:** "a 2019 study by the Max Planck Institute" not "studies show"
- **Artifact/tablet IDs:** "tablet CBS 10673" not "a Sumerian tablet"

### Bibliography Rules
- Numbered list, academic citation format
- Minimum 5 entries per document
- **Source Count** in header MUST match actual bibliography entry count
- Never fabricate ISBNs, DOIs, authors, or publications

### Counter-Arguments
- Include a `## Counter-Arguments & Criticisms` section in every document
- Only include REAL, PUBLISHED counter-arguments attributed to specific scholars
- If no real counter-arguments exist (settled consensus), use the honest "no dispute" note template
- Never invent weak objections to fill space

---

## FILE NAMING

```
[Section]_[Group]_[Seq]_Short_Descriptive_Name.md
```

- **Section**: A–ZH (uppercase, one or two letters)
- **Group**: Subfolder group number (1–5)
- **Seq**: Two-digit sequence within group, zero-padded (01, 02, …)
- **Name**: Underscores between words, Title_Case
- No spaces, max ~50 characters for name portion
- Sequential within each subfolder group, no gaps

### Good Examples
```
A_1_01_Sumerian_Texts_and_Tablets.md       ✓
P_1_01_Meaning_of_Life_Frameworks.md       ✓
Q_1_03_Dark_Matter_Dark_Energy.md          ✓
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
[Section]_[Group]_[Seq]_[descriptive_name].[ext]
```

Example: `A_1_01_eridu_genesis_tablet.jpg`, `Q_1_01_cosmic_web_simulation.png`

---

*See ORGANIZATION_RULES.md for complete rules. See METHODOLOGY.md for research methodology and FACT_CHECKING.md for tier and quality standards.*
