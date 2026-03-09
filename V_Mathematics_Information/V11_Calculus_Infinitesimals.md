# V11 — Calculus & Infinitesimals: Newton, Leibniz & the Kerala School

> **Document ID:** V11
> **Section:** V_Mathematics_Information
> **Keywords:** calculus, Newton, Leibniz, Kerala school, Madhava, infinitesimal, derivative, integral, fluxion, limit, fundamental theorem, priority dispute, non-standard analysis, Robinson
> **Category Tags:** mathematics, information
> **Cross-References:** [V03](V03_Infinity_Paradoxes_Mathematical_Philosophy.md) · [V04](V04_Ethnomathematics_Indigenous_Systems.md) · [ZA08](../ZA_Physics_Quantum/ZA08_General_Special_Relativity.md) · P03
> **Reliability Tier:** Tier 1 (primary texts, manuscripts, and mathematical proofs survive)
> **Last Updated:** Mar 07, 2026 | **Source Count:** 20 | **Weighted Score:** 41 | **Source Confidence:** [4/5] | **Confidence:** High

---

## QUICK SUMMARY

Calculus — the mathematics of continuous change — is arguably the most powerful intellectual tool ever created, enabling the scientific revolution, modern physics, engineering, economics, and computation.
**Isaac Newton** (1642–1727) and **Gottfried Wilhelm Leibniz** (1646–1716) independently developed calculus in the 1660s–1680s — Newton as "method of fluxions" for physics, Leibniz as a general symbolic system with superior notation ($\frac{dy}{dx}$, $\int$) that the world still uses.
The **Kerala school** of mathematics in southern India — beginning with **Madhava of Sangamagrama** (c. 1340–1425) — discovered infinite series expansions for trigonometric functions (equivalent to Taylor/Maclaurin series) **250 years before Newton and Leibniz**, representing one of the most significant priority questions in the history of mathematics.
The **priority dispute** between Newton and Leibniz (1699–1716) became the bitterest scientific controversy of its era, splitting European mathematics into British (Newtonian) and Continental (Leibnizian) camps for a century — to Britain's detriment, as Leibniz's notation proved far more productive.
The logical foundations of calculus remained problematic until the 19th century — **Cauchy, Weierstrass, and Dedekind** replaced Newton's intuitive "fluxions" and Leibniz's "infinitesimals" with the rigorous **epsilon-delta definition of limits**. In 1960, **Abraham Robinson** rehabilitated infinitesimals through **non-standard analysis**, proving that Leibniz's original infinitesimal reasoning could be made logically rigorous after all.

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Archaeological Record)

### 1.1 Precursors to calculus

Calculus did not emerge from nothing:
- **Archimedes** (c. 287–212 BCE): *Method of Exhaustion* — approximated areas and volumes by inscribing/circumscribing polygons with increasing numbers of sides. His calculation of the area under a parabola and the volume of a sphere are proto-integral calculus.
- **The Archimedes Palimpsest** (discovered 1906, fully imaged 2008): revealed Archimedes' *Method of Mechanical Theorems* — showing he used "indivisibles" (infinitely thin slices) to discover results before proving them rigorously by exhaustion.
- **Cavalieri** (1598–1647): *Geometria Indivisibilibus* (1635) — systematized the method of indivisibles in Europe.
- **Fermat** (1630s): found tangent lines to curves (proto-differentiation) and areas under power curves (proto-integration) using methods equivalent to the power rule.

### 1.2 Newton's method of fluxions

**Isaac Newton** developed calculus primarily for physics:
- **1665–1666** ("annus mirabilis"): Newton developed his "method of fluxions" during the plague years at Woolsthorpe — independently of Leibniz.
- **Fluxions**: Newton treated quantities as flowing (*fluent*) and their rates of change as fluxions (denoted by dots: $\dot{x}$). He obtained the **fundamental theorem of calculus** (FTC) — differentiation and integration are inverse operations.
- **Publication delay**: Newton did not publish his calculus until *Principia Mathematica* (1687, using geometric proofs) and *De Analysi* (written 1669, circulated privately, published 1711). His notation ($\dot{x}$, $\ddot{x}$) was less effective than Leibniz's.
- Newton applied calculus to orbital mechanics — *Principia* derived Kepler's laws from the inverse-square law of gravity, demonstrating calculus's power.

### 1.3 Leibniz's calculus notation and system

**Gottfried Wilhelm Leibniz** developed calculus as a general symbolic method:
- **1675–1684**: Leibniz independently developed differential and integral calculus, publishing in *Acta Eruditorum* (1684: differential calculus; 1686: integral calculus) — before Newton published.
- **Notation**: $\frac{dy}{dx}$ for derivatives, $\int y \, dx$ for integrals, $d$ for differentials — all still standard notation. This notation is far more suggestive and productive than Newton's dots.
- Leibniz treated differentials $dx$ and $dy$ as "infinitely small" quantities whose ratio gives the derivative — conceptually powerful but logically problematic until Robinson (1960).
- Continental mathematicians (Bernoulli brothers, Euler, Lagrange) developed Leibniz's framework into the calculus that shaped 18th- and 19th-century mathematics and physics.

### 1.4 The Kerala school — Madhava's series (14th–16th century)

The Kerala school of astronomy and mathematics:
- **Madhava of Sangamagrama** (c. 1340–1425, Kerala, India): discovered infinite series for $\pi$, sine, cosine, and arctangent — results attributed to him in later Kerala texts (Nilakantha's *Tantrasamgraha*, 1501; Jyeshthadeva's *Yuktibhāṣā*, c. 1530).
- **Madhava-Leibniz series**: $\frac{\pi}{4} = 1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \cdots$ — discovered by Madhava c. 1400, independently by Leibniz in 1674 and Gregory in 1671.
- **Madhava-Newton power series**: series expansions equivalent to Taylor series for sine and cosine — discovered ~250 years before Newton.
- The *Yuktibhāṣā* contains **proofs** of these results using a method equivalent to integration — not merely stated results but rigorous derivations.
- The Kerala school represents the most significant pre-European development of calculus-like mathematics.

### 1.5 The Newton-Leibniz priority dispute

The bitterest scientific controversy:
- **1699**: Fatio de Duillier accused Leibniz of plagiarizing Newton.
- **1711–1713**: the dispute escalated — the Royal Society of London (of which Newton was President) investigated and found in Newton's favor (*Commercium Epistolicum*, 1712/1713) — but Newton himself secretly authored most of the report.
- **Modern consensus**: independent invention — Newton developed calculus first (1665–1666) but Leibniz published first (1684) — and there is no credible evidence that Leibniz saw Newton's unpublished manuscripts.
- **Consequences**: British mathematicians loyally used Newton's inferior notation for over a century, isolating themselves from Continental developments. The "analytical revolution" (Babbage, Herschel, Peacock at Cambridge, c. 1815) finally adopted Leibniz's notation in Britain.

### 1.6 Rigorization — limits, epsilon-delta, and non-standard analysis

The logical foundations of calculus:
- **Berkeley's criticism** (1734): *The Analyst* — Bishop Berkeley attacked fluxions as logically incoherent: infinitesimals that are sometimes zero and sometimes not are "ghosts of departed quantities."
- **Cauchy** (1820s): introduced the concept of the limit as the foundation of calculus — derivatives and integrals defined as limits of sequences and sums.
- **Weierstrass** (1860s): formalized the **epsilon-delta definition** — for every $\varepsilon > 0$, there exists $\delta > 0$ such that... — eliminating all reference to infinitesimals. This remains the standard rigorous foundation.
- **Abraham Robinson** (1918–1974), *Non-Standard Analysis* (1960/1966): using model theory (mathematical logic), Robinson proved that a rigorous number system containing actual infinitesimals is consistent — vindicating Leibniz's intuition 300 years later.

---

## 2. CREDIBLE BUT DEBATED CLAIMS (Tier 2 — Academic / Debated)

### 2.1 Whether Kerala results were transmitted to Europe

The key question:
- **Joseph (1991, 2011)**: argued that Jesuit missionaries in Kerala (16th–17th century) may have transmitted Kerala mathematical results to Europe — providing a possible channel for Indian infinite series reaching European mathematicians.
- **Counter-argument**: no documentary evidence of such transmission has been found — Leibniz and Newton developed their calculus from clearly documented European antecedents (Archimedes, Cavalieri, Fermat, Barrow).
- **Current consensus**: independent invention is the most parsimonious explanation, but the possibility of transmission (via Jesuit intermediaries) cannot be definitively ruled out.

### 2.2 Which is the "better" foundation — limits or infinitesimals?

- **Epsilon-delta** (Weierstrass): standard, logically unimpeachable, but pedagogically challenging — beginners struggle with the quantifier logic.
- **Non-standard analysis** (Robinson): closer to the intuitive reasoning of Newton and Leibniz — infinitesimals are genuine mathematical objects. Logically equivalent in power to standard analysis.
- **Smooth infinitesimal analysis** (Bell, 1998): an alternative approach using category theory — infinitesimals are nilsquare ($\varepsilon^2 = 0$ but $\varepsilon \neq 0$).
- No "winner" — each approach has advantages and adherents.

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Possible but Unverified)

### 3.1 Lost calculus-like methods in Islamic mathematics

Ibn al-Haytham (c. 965–1040) computed the volume of a paraboloid using a method equivalent to integration. Whether a broader calculus-like program existed in Islamic mathematics but was lost is speculative — the surviving texts show impressive individual results but not a systematic calculus.

---

## 4. DUBIOUS OR FRINGE CLAIMS (Tier 4 — No Credible Source / Contradicted by Evidence)

### 4.1 Calculus was known to ancient Egyptians or Atlanteans

Egyptian mathematics, while capable, shows no evidence of calculus-like reasoning. Claims that ancient civilizations possessed calculus have no evidential basis.

---

## COUNTER-ARGUMENTS & CRITICISMS

| Claim | Counter-Argument | Source |
|-------|------------------|--------|
| Newton invented calculus | Leibniz invented it independently; Kerala school developed key components 250 years earlier | Joseph, 2011 |
| Leibniz's notation is superior | Newton's is more natural for time-dependent physical problems (dot notation for velocity, acceleration) | Guicciardini, 1999 |
| Kerala results were transmitted to Europe | No documentary evidence of transmission exists | Plofker, 2009 |
| Infinitesimals were always logically suspect | Robinson proved they can be rigorously defined; Leibniz's intuition was correct | Robinson, 1966 |
| Calculus requires the real number continuum | Constructive and discrete versions of calculus exist | Bishop, 1967 |

---

## IMAGES

| Description | Source | Type |
|-------------|--------|------|
| Newton's *Principia* title page (1687) | Various | Book illustration |
| Leibniz's 1684 *Acta Eruditorum* calculus paper | Various | Journal page |
| Madhava series for π/4 (modern notation) | Various | Mathematical formula |
| Archimedes Palimpsest — method of mechanical theorems | Walters Art Museum | Manuscript photograph |
| Epsilon-delta definition diagram | Various | Mathematical diagram |

---

## BIBLIOGRAPHY

1. Newton, Isaac. *The Mathematical Papers of Isaac Newton*. Edited by D.T. Whiteside. 8 vols. Cambridge: Cambridge University Press, 1967–1981.
2. Leibniz, Gottfried Wilhelm. "Nova Methodus pro Maximis et Minimis." *Acta Eruditorum* (1684): 467–473.
3. Joseph, George Gheverghese. *The Crest of the Peacock: Non-European Roots of Mathematics*. 3rd ed. Princeton: Princeton University Press, 2011.
4. Rajagopal, C.T., and M.S. Rangachari. "On an Untapped Source of Medieval Keralese Mathematics." *Archive for History of Exact Sciences* 18 (1978): 89–102.
5. Robinson, Abraham. *Non-Standard Analysis*. Amsterdam: North-Holland, 1966.
6. Boyer, Carl B. *The History of the Calculus and Its Conceptual Development*. New York: Dover, 1959.
7. Guicciardini, Niccolò. *Reading the Principia: The Debate on Newton's Mathematical Methods for Natural Philosophy from 1687 to 1736*. Cambridge: Cambridge University Press, 1999.
8. Hall, A. Rupert. *Philosophers at War: The Quarrel between Newton and Leibniz*. Cambridge: Cambridge University Press, 1980.
9. Berkeley, George. *The Analyst*. 1734. In *The Works of George Berkeley*, edited by A.A. Luce and T.E. Jessop, vol. 4. London: Nelson, 1951.
10. Cauchy, Augustin-Louis. *Cours d'analyse de l'École Royale Polytechnique*. 1821. Translated by Robert E. Bradley and C. Edward Sandifer. New York: Springer, 2009.
11. Grabiner, Judith V. *The Origins of Cauchy's Rigorous Calculus*. Cambridge: MIT Press, 1981.
12. Plofker, Kim. *Mathematics in India*. Princeton: Princeton University Press, 2009.
13. Katz, Victor J. "Ideas of Calculus in Islam and India." *Mathematics Magazine* 68 (1995): 163–174.
14. Stillwell, John. *Mathematics and Its History*. 3rd ed. New York: Springer, 2010.
15. Bressoud, David M. *A Radical Approach to Real Analysis*. 2nd ed. Washington, DC: Mathematical Association of America, 2007.
16. Edwards, C.H., Jr. *The Historical Development of the Calculus*. New York: Springer, 1979.
17. Bell, John L. *A Primer of Infinitesimal Analysis*. Cambridge: Cambridge University Press, 1998.
18. Netz, Reviel, and William Noel. *The Archimedes Codex*. Philadelphia: Da Capo Press, 2007.
19. Dunham, William. *The Calculus Gallery: Masterpieces from Newton to Lebesgue*. Princeton: Princeton University Press, 2005.
20. Jyeshthadeva. *Yuktibhāṣā (Rationale in Mathematical Astronomy of Jyeṣṭhadeva)*. Edited by K.V. Sarma. Translated by K. Ramasubramanian et al. 2 vols. New Delhi: Hindustan Book Agency, 2008.

---

## CROSS-REFERENCE INDEX

| Topic | Section | Document |
|-------|---------|----------|
| Infinity and paradoxes | V | [V03 — Infinity Paradoxes](V03_Infinity_Paradoxes_Mathematical_Philosophy.md) |
| Ethnomathematics | V | [V04 — Ethnomathematics](V04_Ethnomathematics_Indigenous_Systems.md) |
| General relativity | Q | [ZA08 — General Relativity](../ZA_Physics_Quantum/ZA08_General_Special_Relativity.md) |
| Epistemology | P | P03 — Epistemology |

---

*Document V11 · Created Mar 07, 2026 · TheoriesOfAnything Knowledge Base*
