# S_1_09 — Quantum Cryptography and Post-Quantum Security

> **Source Count:** 0 | **Weighted Score:** 0 | **Source Confidence:** [1/5] | **Primary Tier:** 1–2 | **Last Updated:** March 10, 2026
> **Keywords:** quantum cryptography, quantum key distribution, QKD, post-quantum cryptography, RSA, Shor's algorithm, lattice-based cryptography, BB84, quantum internet, NIST PQC, cryptographic agility, harvest now decrypt later
> **Category Tags:** future technology, cryptography, quantum, security, computing
> **Cross-References:** [S_1_04 — Quantum Computing](S_1_04_Quantum_Computing_Information.md) · [ZA_2_01 — Quantum Mechanics](../../ZA_Physics_Quantum/ZA2_Gravity_Spacetime_Cosmology/ZA_2_01_Time_Physics_Philosophy.md) · [V_1_01 — Information Theory](../../V_Mathematics_Information/V1_History_Cultural/V_1_01_History_of_Zero.md) · [S_1_06 — Internet](S_1_06_Internet_Digital_Civilization.md)

---

## QUICK SUMMARY

**Quantum cryptography** and **post-quantum cryptography** address the existential threat that quantum computers pose to current encryption. **The threat**: large-scale quantum computers running **Shor's algorithm** (Peter Shor, 1994) can efficiently factor large integers and compute discrete logarithms — breaking the mathematical foundations of **RSA**, **Diffie-Hellman**, and **Elliptic Curve Cryptography (ECC)**, which secure virtually all current internet communications (HTTPS, TLS, VPNs, digital signatures, banking). A sufficiently powerful quantum computer (estimated at ~4,000+ error-corrected logical qubits for 2048-bit RSA) would break these systems in hours rather than the billions of years required classically. **Current quantum computing status**: as of 2024, the largest quantum processors (~1,100+ physical qubits, IBM "Condor") are far from the millions of physical qubits needed to implement error-corrected Shor's algorithm on cryptographically relevant key sizes; estimates for timeline range from 10 to 30+ years, but the "harvest now, decrypt later" threat — adversaries collecting encrypted communications today to decrypt when quantum computers are available — makes the transition urgent. **Quantum Key Distribution (QKD)**: the **BB84 protocol** (Bennett & Brassard, 1984) uses quantum mechanics (the no-cloning theorem, measurement disturbance) to guarantee secure key exchange — any eavesdropping attempt physically perturbs the quantum states and is detectable; QKD has been commercially deployed (ID Quantique, Toshiba) and demonstrated over satellite links (China's Micius satellite, 2017, key distribution over 1,200 km); however, QKD requires dedicated physical infrastructure (optical fiber or line-of-sight), is expensive, and cannot protect stored data or authenticate users. **Post-quantum cryptography (PQC)**: NIST finalized its first PQC standards in August 2024 — **CRYSTALS-Kyber** (lattice-based key encapsulation) and **CRYSTALS-Dilithium**, **FALCON**, and **SPHINCS+** (digital signature schemes) — designed to be secure against both classical and quantum computers while running on existing hardware; migration to PQC across global infrastructure is a massive, multi-year undertaking requiring cryptographic agility.

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Scholarly Consensus)

### 1.1 Shor's Algorithm Threat
- Shor's algorithm is mathematically proven to efficiently break RSA, DH, and ECC on a sufficiently large quantum computer — this is not a theoretical speculation but a mathematical certainty; the only uncertainty is *when* quantum computers powerful enough to execute it will exist; the threat is universally acknowledged by cryptographic and national security communities (NSA, NIST, GCHQ)

### 1.2 NIST PQC Standards
- NIST's PQC standardization process (begun 2016, finalized 2024) produced algorithms based on mathematical problems believed to be resistant to both classical and quantum attack — primarily lattice-based problems (Learning With Errors) and hash-based signatures; these algorithms have undergone extensive public cryptanalysis over 8+ years; migration to PQC is recommended by NIST, NSA, and CISA for all federal and critical infrastructure systems

---

## 2. CREDIBLE CLAIMS (Tier 2 — Academic / Debated but Supported)

### 2.1 QKD Practicality
- QKD is information-theoretically secure (proven by physics, not mathematical assumptions) — but practical QKD systems have implementation vulnerabilities (side-channel attacks on detectors, Trojan horse attacks on sources) that weaken their theoretical guarantees; furthermore, QKD addresses only key distribution (not authentication, data-at-rest encryption, or digital signatures) and requires expensive dedicated infrastructure; many cryptographers argue that PQC on existing networks provides better security-per-dollar for most applications (Bernstein & Lange, 2017)

### 2.2 Harvest Now, Decrypt Later
- Intelligence agencies and adversaries are plausibly collecting encrypted communications now in anticipation of future quantum decryption capability — this is widely assumed in the security community and has driven urgency in PQC migration; the actual scope of such collection is classified, but the strategic logic is sound for long-lived secrets (diplomatic cables, military plans, trade secrets with multi-decade relevance)

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Possible but Unverified)

### 3.1 Quantum Internet
- A global quantum internet — connecting quantum computers and enabling distributed quantum computing, unconditionally secure communication, and quantum sensor networks — is a long-term research goal; quantum repeaters (needed to extend QKD beyond ~100 km fiber distance) have been demonstrated in laboratories but not deployed at scale; China's 2,000 km Beijing-Shanghai quantum backbone (2017, using trusted relay nodes — not end-to-end quantum) is the most ambitious implementation; a true quantum internet likely requires quantum memory and entanglement distribution technologies that remain immature

---

## 4. DUBIOUS CLAIMS (Tier 4 — No Credible Source / Contradicted by Evidence)

### 4.1 Quantum Computers Already Breaking Encryption
- **[DEBUNKED]** Claims that quantum computers have already broken or can currently break RSA/ECC encryption are false — the largest numbers factored by quantum computers (as of 2024) are tiny (tens of bits vs. the 2048+ bits used in practice); current quantum processors lack the scale and error correction needed by orders of magnitude; while the future threat is real, current quantum computers pose zero threat to deployed cryptographic systems

### Counter-Arguments
- The timeline for cryptographically relevant quantum computers is highly uncertain — pessimistic estimates suggest 30+ years or never (if error correction scaling proves impractical); overly urgent migration may impose unnecessary costs and risks (PQC algorithms have larger key sizes and computational overhead, and may themselves prove vulnerable to future cryptanalysis)
- PQC algorithms, while extensively vetted, are based on mathematical hardness assumptions that could be broken by new classical or quantum algorithms — lattice-based cryptography has not been studied for as long as RSA; NIST's process is rigorous but not a guarantee of permanent security
- QKD advocates argue that information-theoretic security (guaranteed by physics) is fundamentally superior to computational security (guaranteed by mathematical assumptions that could be overturned); QKD critics argue this theoretical advantage is undermined by practical implementation challenges

---

## IMAGES

| # | Description | Filename | Source | License |
|---|-------------|----------|--------|---------|
*No images assigned yet.*

---

## BIBLIOGRAPHY

- **Shor, P.W. "Algorithms for Quantum Computation: Discrete Logarithms and Factoring." In *Proc**. 35th Annual Symposium on Foundations of Computer Science* (1994): 124–134. DOI: 10.1109/sfcs.1994.365700
- **Bennett, C**. H. & Brassard, G. "Quantum Cryptography." In *Proc. IEEE International Conference on Computers, Systems and Signal Processing* (1984): 175–179.
- **NIST**. *Post-Quantum Cryptography: FIPS 203, 204, 205.* National Institute of Standards and Technology (2024).
- **Bernstein, D**. J. & Lange, T. "Post-Quantum Cryptography." *Nature* 549 (2017): 188–194. DOI: 10.1038/nature23461.
- **Liao, S.-K. et al**. "Satellite-to-Ground Quantum Key Distribution." *Nature* 549 (2017): 43–47.
- **Mosca, M**. "Cybersecurity in an Era with Quantum Computers." *IEEE Security & Privacy* 16 (2018): 50–57. DOI: 10.1109/msp.2018.3761723
- **Alagic, G. et al**. *Status Report on the Third Round of the NIST Post-Quantum Cryptography Standardization Process.* NIST (2022). DOI: 10.30837/rt.2022.3.210.05
- **Gisin, N. et al**. "Quantum Cryptography." *Reviews of Modern Physics* 74 (2002): 145–195. DOI: 10.1103/revmodphys.74.145
- **Pirandola, S. et al**. "Advances in Quantum Cryptography." *Advances in Optics and Photonics* 12 (2020): 1012–1236.
- **NSA**. *Announcing Suite B Cryptography Replacement.* NSA Cybersecurity Advisory (2022).
- **Wehner, S. et al**. "Quantum Internet: A Vision for the Road Ahead." *Science* 362 (2018): eaam9288.

---

## CROSS-REFERENCE INDEX

| Related Doc | Connection |
|-------------|-----------|
| [S_1_04 — Quantum Computing](S_1_04_Quantum_Computing_Information.md) | Quantum threat |
| [ZA_2_01 — Quantum Mechanics](../../ZA_Physics_Quantum/ZA2_Gravity_Spacetime_Cosmology/ZA_2_01_Time_Physics_Philosophy.md) | Physics foundations |
| [V_1_01 — Information Theory](../../V_Mathematics_Information/V1_History_Cultural/V_1_01_History_of_Zero.md) | Cryptographic math |
| [S_1_06 — Internet](S_1_06_Internet_Digital_Civilization.md) | Network security |

---

*Last Updated: March 10, 2026*

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
