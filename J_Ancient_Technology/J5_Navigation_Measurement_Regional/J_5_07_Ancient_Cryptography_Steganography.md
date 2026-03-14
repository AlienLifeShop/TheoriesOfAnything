# J_5_07 — Ancient Cryptography and Steganography

> **Source Count:** 12 | **Weighted Score:** 23 | **Source Confidence:** [3/5] | **Primary Tier:** 1–2 | **Last Updated:** March 9, 2026
> **Keywords:** cryptography, cipher, steganography, scytale, Caesar cipher, substitution cipher, Polybius square, atbash, hidden writing, secret communication, code, enigma, ancient cipher, invisible ink, tattoo message, wax tablet
> **Category Tags:** ancient technology, communication, military, secret societies
> **Cross-References:** [J_5_04 — Ancient Communication Systems](J_5_04_Ancient_Communication_Systems.md) · [N_1_01 — Secret Societies Overview](../../N_Secret_Societies/N1_Ancient_Mystery_Schools/N_1_01_Mystery_Schools.md) · [V_1_01 — Mathematics Information Overview](../../V_Mathematics_Information/V1_History_Cultural/V_1_01_History_of_Zero.md) · [ZD_1_01 — Information Computation Overview](../../ZD_Information_Computation/ZD1_Foundations_Theory/ZD_1_01_Algorithms_Computation_Limits.md)

---

## QUICK SUMMARY

The concealment of information — through **cryptography** (transforming a message so it cannot be read without the key) and **steganography** (hiding the very existence of a message) — has ancient origins driven by military, diplomatic, and commercial necessity. The earliest known use of cryptographic techniques dates to c. **1900 BCE** in Egypt (tomb of Khnumhotep II at Beni Hasan), where unusual hieroglyphic substitutions were used — though these may have been more stylistic than secrecy-driven. The first clearly military-purpose cipher device was the **Spartan scytale** (c. 7th–5th century BCE): a strip of leather wound around a cylindrical staff of specific diameter, on which a message was written; the strip, when unwound, appeared as meaningless letters — only a staff of matching diameter could restore the text. This constitutes a **transposition cipher** (rearranging letter order without substitution). The **atbash cipher** (Hebrew, used in the Book of Jeremiah, c. 600 BCE) is a **substitution cipher** mapping each letter to its reverse-alphabet equivalent (א→ת, ב→ש, etc.); the word *Sheshach* in Jeremiah 25:26 and 51:41 is widely accepted as an atbash cipher for *Babel* (Babylon). **Julius Caesar** (1st c. BCE) used a simple substitution cipher — each letter shifted by a fixed number of positions (typically 3: A→D, B→E...) — described by Suetonius (*Lives of the Caesars*, "Julius," 56). The **Polybius square** (2nd c. BCE): a 5×5 grid encoding each letter as a pair of coordinates, enabling transmission by torch signals (a distant visual cipher); described in Polybius *Histories* X.45. Ancient steganographic methods included: shaving a slave's head, tattooing a message on the scalp, and waiting for hair to regrow (Herodotus 5.35); writing in **invisible ink** (lemon juice, milk, or urine, readable when heated — described by Pliny the Elder); and hiding messages inside wax tablets (scraping text onto the wooden backing beneath the wax layer — Herodotus 7.239, Demaratus warning of Xerxes' invasion plan).

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Scholarly Consensus)

### 1.1 Egyptian Non-Standard Hieroglyphs
- The tomb inscription of **Khnumhotep II** at Beni Hasan (c. 1900 BCE, 12th Dynasty) contains unusual hieroglyphic substitutions — replacing common signs with rare or invented ones; this is often cited as the **earliest known cryptographic-like practice** (Kahn, 1967)
- However, scholars debate whether the intent was secrecy or aesthetic distinction (making the inscription more prestigious or challenging to read) — true secrecy-motivated cryptography is not clearly attested in Egyptian sources
- **Sacred hieroglyphs**: by the Late Period, temple inscriptions used increasingly obscure sign forms (*cryptographic hieroglyphs*), readable only by specialized priests — though this may reflect theological exclusivity rather than military secrecy

### 1.2 Caesar Cipher
- **Suetonius** (*De Vita Caesarum*, "Divus Julius" 56): "If he had anything confidential to say, he wrote it in cipher, that is, by so changing the order of the letters of the alphabet, that not a word could be made out"
- The shift of 3 (A→D) is the conventional attribution; a generalized shift cipher (any fixed offset) is now called a "Caesar cipher" in modern cryptography
- As a **monoalphabetic substitution cipher**, it is trivially breakable by frequency analysis — but frequency analysis was not formally described until **al-Kindi** (c. 850 CE, *A Manuscript on Deciphering Cryptographic Messages*), making the Caesar cipher effective in its era

### 1.3 Al-Kindi and the Birth of Cryptanalysis
- **Al-Kindi** (Abu Yusuf Ya'qub ibn Ishaq al-Kindi, c. 801–873 CE): wrote *Risalah fi Istikhraj al-Mu'amma* (A Manuscript on Deciphering Cryptographic Messages), the oldest known treatise on **cryptanalysis**
- Introduced **frequency analysis**: the observation that in any language, certain letters appear with characteristic frequencies (e.g., *alif* is the most common letter in Arabic); by counting letter frequencies in a ciphertext and matching them to known frequency distributions, any simple substitution cipher can be broken
- This discovery rendered all monoalphabetic substitution ciphers insecure and drove the development of more complex ciphers (polyalphabetic substitution, homophonic ciphers)

---

## 2. CREDIBLE CLAIMS (Tier 2 — Academic / Debated but Supported)

### 2.1 The Scytale
- Described by Plutarch (*Lysander* 19) and others: a leather strip wound helically around a rod of specific diameter; letters written across the strip while wound produce a transposition cipher when unwound
- Scholars (Kelly, 1998) have questioned whether the scytale was a cipher device or simply a means of authentication (the matching diameter proving the message's origin) — the cryptographic interpretation remains the mainstream view but is debated

### 2.2 Polybius Square
- **Polybius** (*Histories* X.45–47, 2nd c. BCE): describes a system of encoding letters in a 5×5 grid, each letter represented by two numbers (row and column); designed for long-distance visual signaling using two sets of torches — one set for the row number, one for the column
- This is the earliest known **fractionation cipher** (breaking a letter into two components), a concept foundational to modern cryptography; the Polybius square is the ancestor of the ADFGVX cipher used in World War I

### 2.3 Hebrew Atbash and Other Biblical Ciphers
- **Atbash**: a simple substitution where the first letter of the alphabet maps to the last, the second to the second-to-last, etc. (in Hebrew: א↔ת, ב↔ש, ג↔ר...)
- Jeremiah 25:26 and 51:41: the word **ששך** (*Sheshach*) appears where **בבל** (*Babel*/Babylon) is expected; applying atbash: ב→ש, ב→ש, ל→כ — confirming *Babel* as the plaintext
- Other biblical wordplay (e.g., the **albam** cipher, shifting 11 positions) appears in medieval Jewish literature but may not derive from ancient practice

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Possible but Unverified)

### 3.1 Steganographic Practices in Antiquity
- **Herodotus 5.35**: Histiaeus sent a secret message to Aristagoras by tattooing it on a slave's shaved head, then waiting for the hair to grow back; Aristagoras shaved the slave's head to read the message — orchestrating the Ionian Revolt (499 BCE)
- **Herodotus 7.239**: Demaratus warned Sparta of Xerxes' planned invasion by scraping a message onto the wooden backing of a wax tablet, then covering it with wax — appearing as a blank tablet; Queen Gorgo discovered the hidden text
- These stories are attested only by Herodotus and may contain legendary embellishment, but the techniques described are physically plausible

### 3.2 Invisible Ink
- **Pliny the Elder** (*Natural History* 26.8): describes writing with plant juices that become visible when heated; Ovid (*Ars Amatoria* 3.627) recommends writing with fresh milk, revealed by sprinkling soot
- **Philo of Byzantium** (3rd c. BCE): reportedly described sympathetic inks made from nutgall extract — appearing invisible until washed with copper sulfate solution (revealing dark text); if authentic, this represents early chemical knowledge applied to steganography

---

## 4. DUBIOUS CLAIMS (Tier 4 — No Credible Source / Contradicted by Evidence)

### 4.1 Unbreakable Ancient Ciphers
- **[DEBUNKED]** Claims that ancient civilizations possessed encryption systems that remain unbreakable today are unsupported; all documented ancient ciphers (substitution, transposition) are trivially breakable by modern — and even medieval — cryptanalytic techniques

### Counter-Arguments
- Ancient cryptographic techniques were innovative for their time and sufficient for their purposes; their simplicity does not diminish the intellectual achievement of their inventors

---

## IMAGES

| # | Description | Filename | Source | License |
|---|-------------|----------|--------|---------|
*No images assigned yet.*

---

## BIBLIOGRAPHY

1. Kahn, D. *The Codebreakers: The Story of Secret Writing.* Macmillan (1967). DOI: 10.1086/ahr/74.2.537
2. Singh, S. *The Code Book: The Science of Secrecy from Ancient Egypt to Quantum Cryptography.* Anchor (2000). DOI: 10.1145/966789.966797
3. Al-Kindi. *A Manuscript on Deciphering Cryptographic Messages.* Ed. and trans. in Al-Kadi, I.A., "The Origins of Cryptology." *Cryptologia* 16.2 (1992): 97–126. DOI: 10.1080/0161-119291866801
4. Herodotus. *The Histories.* Trans. R. Waterfield. Oxford World's Classics (1998). DOI: 10.1093/actrade/9780199535668.book.1
5. Suetonius. *The Twelve Caesars.* Trans. R. Graves. Penguin Classics (2007).
6. Polybius. *The Histories.* Trans. R. Waterfield. Oxford World's Classics (2010).
7. Kelly, T. "The Myth of the Skytale." *Cryptologia* 22.3 (1998): 244–260. DOI: 10.1080/0161-119891886902
8. Bauer, C.P. *Secret History: The Story of Cryptology.* CRC Press (2013).
9. Pliny the Elder. *Natural History.* Trans. H. Rackham. Loeb Classical Library (1938–1963). ISBN: 9781594200823
10. Mollin, R.A. *An Introduction to Cryptography.* 2nd ed. CRC Press (2007).
11. Stern, M.A. "Atbash Cipher in the Hebrew Bible." *Semitica* 46 (2001): 139–152.
12. Mrayati, M. et al. (eds). *Arabic Origins of Cryptology.* 6 vols. King Faisal Center for Research and Islamic Studies (2003–2007).

---

## CROSS-REFERENCE INDEX

| Related Doc | Connection |
|-------------|-----------|
| [J_5_04 — Ancient Communication](J_5_04_Ancient_Communication_Systems.md) | Communication methods |
| [N_1_01 — Secret Societies](../../N_Secret_Societies/N1_Ancient_Mystery_Schools/N_1_01_Mystery_Schools.md) | Secrecy traditions |
| [V_1_01 — Mathematics](../../V_Mathematics_Information/V1_History_Cultural/V_1_01_History_of_Zero.md) | Mathematical foundations |
| [ZD_1_01 — Information Computation](../../ZD_Information_Computation/ZD1_Foundations_Theory/ZD_1_01_Algorithms_Computation_Limits.md) | Information theory |

---

*Last Updated: March 9, 2026*

---

<table border="1" cellpadding="12" cellspacing="0" style="border-collapse: collapse; border: 2px solid #888; margin-top: 2em; background: #fafafa;">
<tr><td>

### ⚠️ AI-Assisted Research Disclaimer

This document was generated and structured with the assistance of AI tools.
While every effort is made to ensure accuracy, AI-assisted content may
contain errors, misattributions, or unintended inaccuracies. **Always
verify claims, dates, and sources independently** before citing or relying
on any information presented here.

- **Sources may contain errors.** Bibliography entries and cross-references
  are checked by automated systems, but mistakes can occur. If something
  looks wrong, it may be.
- **Speculative and unverified claims are clearly labeled.** This project
  uses a four-tier evidence system:
  - **Tier 1 — Verified:** Peer-reviewed, established scientific consensus.
  - **Tier 2 — Credible:** Academically supported, debated but grounded.
  - **Tier 3 — Speculative:** Plausible but unverified by mainstream science.
  - **Tier 4 — Dubious:** No credible support or contradicted by evidence.
- **This project maps multiple perspectives — not a single truth.** Mainstream,
  alternative, and skeptical viewpoints are presented side by side for
  critical comparison, *not* endorsement. Inclusion does not imply agreement.
- **We are actively improving.** Source verification, factuality scoring,
  and bibliography enrichment are ongoing. Each revision adds stronger
  citations, corrects identified errors, and expands coverage.

📖 For full details on our verification methodology, scoring systems, and
quality metrics, see: [Fact-Checking & Verification Systems](../../_MASTER_REFERENCE/FACT_CHECKING.md)

*Think Openly. Check the sources. Draw your own conclusions.*

</td></tr>
</table>
