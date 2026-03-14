# ZA_4_11 — Time Crystals and Discrete Time Symmetry Breaking

> **Source Count:** 13 | **Weighted Score:** 39 | **Source Confidence:** [4/5] | **Primary Tier:** 1–2 | **Last Updated:** March 9, 2026
> **Keywords:** time crystal, discrete time crystal, DTC, time translation symmetry breaking, Floquet, many-body localization, MBL, Frank Wilczek, period doubling, subharmonic response, NV center, trapped ion, Google Sycamore, prethermalization, non-equilibrium phase, spontaneous symmetry breaking, time order
> **Category Tags:** physics-quantum, condensed-matter, non-equilibrium, time-symmetry, phase-of-matter, experimental-physics
> **Cross-References:** [ZA_4_06 — Phase Transitions](ZA_4_06_Phase_Transitions_Symmetry_Breaking.md) · [ZA_3_02 — Symmetry](../ZA3_Particle_Nuclear_Physics/ZA_3_02_Symmetry_Noether_Theorem.md) · [ZA_2_01 — Time Physics](../ZA2_Gravity_Spacetime_Cosmology/ZA_2_01_Time_Physics_Philosophy.md) · [ZA_1_05 — Decoherence](../ZA1_Quantum_Foundations/ZA_1_05_Quantum_Decoherence_Measurement_Problem.md) · [ZA_5_02 — Quantum Computing](../ZA5_Quantum_Technology_Applications/ZA_5_02_Quantum_Computing_Qubit_Technologies.md)

---

## QUICK SUMMARY

A **time crystal** is a phase of matter that spontaneously breaks **time-translation symmetry** — the fundamental physical principle that the laws of physics are the same at all times (which, via Noether's theorem, is linked to energy conservation). In conventional crystals, atoms arrange themselves in a spatially periodic pattern that breaks the continuous translational symmetry of space into a discrete one. By analogy, Nobel laureate **Frank Wilczek** proposed in 2012 that a system could exist in its lowest energy state while exhibiting periodic motion — a "crystal in time" that spontaneously oscillates without energy input. Wilczek's original **equilibrium time crystal** proposal was subsequently proven impossible by **Watanabe and Oshikawa** (2015, *Physical Review Letters* 114: 251603) and by **Bruno** (2013) — a system in thermal equilibrium cannot break time-translation symmetry in its ground state. However, in 2016, theoretical work by **Khemani, Lazarides, Moessner, and Sondhi** and independently by **Else, Bauer, and Nayak** showed that **periodically driven (Floquet) systems** far from equilibrium can exhibit a robust form of time-crystalline order: the **discrete time crystal** (DTC), in which the system responds at a period that is an integer multiple (typically double) of the driving period — **period doubling** that persists indefinitely and is robust against perturbations, constituting a genuine non-equilibrium phase of matter. In 2017, two groups independently demonstrated discrete time crystals experimentally: **Zhang et al.** using a chain of trapped ytterbium ions (*Nature* 543: 217–220), and **Choi et al.** using nitrogen-vacancy (NV) centers in diamond (*Nature* 543: 221–225). In 2021, the **Google Quantum AI** team used their **Sycamore** quantum processor (20 qubits) to realize a discrete time crystal, exploiting the system's many-body localization to prevent thermalization (Mi et al., *Nature* 601: 531–536, 2022). Time crystals represent a fundamentally new category of non-equilibrium matter — phases stabilized not by energy minimization but by the interplay of periodic driving, interactions, and disorder.

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Archaeological Record)

### 1.1 Theoretical Development
- **Frank Wilczek** (2012, *Physical Review Letters* 109: 160401) proposed that a quantum-mechanical system could spontaneously break continuous time-translation symmetry in its ground state — analogous to how a spatial crystal breaks spatial translation symmetry; he called such a system a "time crystal" or "quantum time crystal"
- This original equilibrium proposal was **disproved**:
  - Patrick **Bruno** (2013, *PRL* 111: 070402) showed that Wilczek's specific model did not actually exhibit time-crystalline behavior
  - **Watanabe and Oshikawa** (2015, *PRL* 114: 251603) proved a no-go theorem: in thermal equilibrium (and for the ground state), continuous time-translation symmetry cannot be spontaneously broken — an equilibrium time crystal is impossible
- The concept was rescued in a modified form by **Floquet (periodically driven) systems**:
  - **Khemani, Lazarides, Moessner, and Sondhi** (2016) and independently **Else, Bauer, and Nayak** (2016, *PRL* 117: 090402) proposed the **discrete time crystal** (DTC): a periodically driven system that responds with a period that is an integer multiple of the driving period (spontaneous breaking of **discrete** time-translation symmetry)
  - The key insight: a Floquet system is driven with period $T$, imposing a discrete time symmetry $t \to t + T$; a DTC responds at period $2T$ (or $nT$), breaking this discrete symmetry — this is allowed because the no-go theorem applies only to equilibrium/continuous symmetry breaking
  - Stability requires **many-body localization** (MBL) — the system must avoid thermalizing (absorbing energy from the drive until it reaches infinite temperature), which would destroy the temporal order

### 1.2 Experimental Realizations
- **Zhang et al.** (2017, *Nature* 543: 217–220) at University of Maryland/JQI: used a chain of 10 trapped $^{171}\text{Yb}^+$ ions with laser-induced spin-spin interactions; observed robust period-doubled oscillations in the spin dynamics that persisted over many driving cycles and were stable against perturbations — the first observation of a DTC
- **Choi et al.** (2017, *Nature* 543: 221–225) at Harvard: used approximately $10^6$ nitrogen-vacancy (NV) spin impurities in a diamond crystal; observed period-doubled magnetization oscillations surviving hundreds of drive cycles — a DTC in a solid-state platform
- Both experiments demonstrated the **hallmarks of a DTC**: (1) subharmonic response at period 2T, (2) rigidity (the response frequency is locked to 2T regardless of small perturbations to the drive), (3) persistence over many cycles (though eventually limited by decoherence/finite system size)
- **Mi et al.** (Google Quantum AI, *Nature* 601: 531–536, 2022): realized a DTC on the Sycamore quantum processor using 20 superconducting qubits — demonstrated many-body localization and period-doubling in a programmable quantum system; the processor's digital control allowed precise tuning of disorder, interactions, and drive parameters

### 1.3 Many-Body Localization (MBL) Connection
- **MBL** is a quantum phenomenon in which strong disorder prevents a many-body system from thermalizing — the system retains memory of its initial conditions indefinitely, even at finite energy density
- MBL is essential for DTC stability: without it, the driven system would absorb energy and heat to infinite temperature, destroying any temporal order
- Basko, Aleiner, and Altshuler (2006) provided the foundational theory of MBL; Pal and Huse (2010) demonstrated it numerically; Schreiber et al. (2015, *Science* 349: 842) observed MBL experimentally in cold atoms in optical lattices
- **Counter-Argument:** The existence of MBL in the strict thermodynamic limit remains debated — some numerical available evidence suggests it may be a finite-size crossover rather than a true phase; this would affect whether DTCs are rigorously stable phases or extremely long-lived prethermal states

---

## 2. CREDIBLE CLAIMS (Tier 2 — Academic / Debated but Supported)

### 2.1 Prethermal Time Crystals
- **Prethermal time crystals** can exist even without MBL — in clean (disorder-free) driven systems, a prethermal regime can emerge where the system appears to be in a DTC phase for exponentially long times (exponential in the driving frequency) before eventually thermalizing:
  - Else, Bauer, and Nayak (2017) and Machado et al. (2020) developed the theoretical framework
  - Kyprianidis et al. (*Science* 372: 1192, 2021) observed a prethermal DTC in a trapped-ion system
- Prethermal DTCs are significant because they do not require the (possibly fragile) assumption of MBL — they are more robust phenomena, though inherently transient on very long timescales

### 2.2 Time Crystals in Other Platforms
- DTC behavior has been observed or claimed in diverse systems:
  - Magnon condensates in superfluid helium-3 (Autti et al., *Nature Materials* 20: 171, 2021)
  - Dissipative systems (open quantum systems coupled to environments)
  - Photonic and phononic systems
- Whether all these realizations represent the "same" phase of matter is debated — the definition of what counts as a "time crystal" has expanded considerably from Wilczek's original proposal

### 2.3 Classification of Non-Equilibrium Phases
- Time crystals have stimulated broader theoretical work on **non-equilibrium phases of matter** — phases stabilized by driving rather than by energy minimization:
  - Floquet topological phases (periodically driven systems exhibiting topological properties absent in equilibrium)
  - Floquet symmetry-protected topological phases
  - The classification of non-equilibrium phases is an active frontier in condensed matter theory, extending the equilibrium Landau paradigm to driven quantum systems

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Possible but Unverified)

### 3.1 Applications of Time Crystals
- Proposed applications include ultra-precise timekeeping, quantum memory, and quantum simulation of non-equilibrium phenomena — but all remain theoretical; no practical device exploiting time-crystalline order has been demonstrated
- **Counter-Argument:** Time crystals, as currently realized, are small, require extreme conditions (cryogenic temperatures, strong lasers, quantum processors), and their potential practical advantages over existing technologies are unclear

---

## 4. DUBIOUS CLAIMS (Tier 4 — No Credible Source / Contradicted by Evidence)

### 4.1 "Perpetual Motion from Time Crystals"
- **[DEBUNKED]** Media misrepresentations have described time crystals as "perpetual motion machines" that oscillate forever without energy input; in reality, discrete time crystals require continuous energy input from the periodic drive — they are perpetually driven, not perpetually moving; they do not violate thermodynamics

---

## IMAGES

| # | Description | Filename | Source | License |
|---|-------------|----------|--------|---------|
*No images assigned yet.*

---

## Counter-Arguments & Criticisms

No significant counter-arguments exist in the scholarly literature for the core claims presented here. The topic of Time Crystals Discrete Symmetry represents established knowledge within quantum physics and theoretical physics with no active scholarly dispute over the fundamental claims presented in this document.

## BIBLIOGRAPHY

1. Wilczek, F. "Quantum Time Crystals." *Physical Review Letters* 109, no. 16 (2012): 160401. DOI: 10.1103/physrevlett.109.160401
2. Watanabe, H. and Oshikawa, M. "Absence of Quantum Time Crystals." *Physical Review Letters* 114, no. 25 (2015): 251603. DOI: 10.1103/physrevlett.114.251603
3. Bruno, P. "Impossibility of Spontaneously Rotating Time Crystals: A No-Go Theorem." *Physical Review Letters* 111, no. 7 (2013): 070402. DOI: 10.1103/physrevlett.111.070402
4. Else, D.V., Bauer, B., and Nayak, C. "Floquet Time Crystals." *Physical Review Letters* 117, no. 9 (2016): 090402. DOI: 10.1103/physrevlett.117.090402
5. Khemani, V., Lazarides, A., Moessner, R., and Sondhi, S.L. "Phase Structure of Driven Quantum Systems." *Physical Review Letters* 116, no. 25 (2016): 250401. DOI: 10.1103/physrevlett.116.250401
6. Zhang, J. et al. "Observation of a Discrete Time Crystal." *Nature* 543 (2017): 217–220.
7. Choi, S. et al. "Observation of Discrete Time-Crystalline Order in a Disordered Dipolar Many-Body System." *Nature* 543 (2017): 221–225.
8. Mi, X. et al. "Time-Crystalline Eigenstate Order on a Quantum Processor." *Nature* 601 (2022): 531–536.
9. Else, D.V., Bauer, B., and Nayak, C. "Prethermal Phases of Matter Protected by Time-Translation Symmetry." *Physical Review X* 7 (2017): 011026.
10. Kyprianidis, A. et al. "Observation of a Prethermal Discrete Time Crystal." *Science* 372, no. 6547 (2021): 1192–1196.
11. Basko, D.M., Aleiner, I.L., and Altshuler, B.L. "Metal-Insulator Transition in a Weakly Interacting Many-Electron System with Localized Single-Particle States." *Annals of Physics* 321, no. 5 (2006): 1126–1205.
12. Sacha, K. and Zakrzewski, J. "Time Crystals: A Review." *Reports on Progress in Physics* 81, no. 1 (2018): 016401.
13. Zaletel, M.P. et al. "Colloquium: Quantum and Classical Discrete Time Crystals." *Reviews of Modern Physics* 95, no. 3 (2023): 031001.

---

## CROSS-REFERENCE INDEX

| Related Doc | Connection |
|-------------|-----------|
| [ZA_4_06 — Phase Transitions](ZA_4_06_Phase_Transitions_Symmetry_Breaking.md) | Symmetry breaking in time dimension |
| [ZA_3_02 — Symmetry](../ZA3_Particle_Nuclear_Physics/ZA_3_02_Symmetry_Noether_Theorem.md) | Time-translation symmetry and Noether's theorem |
| [ZA_2_01 — Time Physics](../ZA2_Gravity_Spacetime_Cosmology/ZA_2_01_Time_Physics_Philosophy.md) | Nature of time and temporal order |
| [ZA_1_05 — Decoherence](../ZA1_Quantum_Foundations/ZA_1_05_Quantum_Decoherence_Measurement_Problem.md) | Decoherence limiting DTC lifetime |
| [ZA_5_02 — Quantum Computing](../ZA5_Quantum_Technology_Applications/ZA_5_02_Quantum_Computing_Qubit_Technologies.md) | Google Sycamore DTC realization |

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
