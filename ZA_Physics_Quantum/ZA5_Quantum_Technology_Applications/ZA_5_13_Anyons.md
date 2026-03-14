# ZA_5_13 — Anyons and Fractional Quantum Hall Effect

> **Source Count:** 21 | **Weighted Score:** 59 | **Source Confidence:** [5/5] | **Primary Tier:** 1 | **Last Updated:** March 13, 2026
> **Keywords:** anyons, fractional quantum Hall effect, topological order, non-Abelian anyons, braiding, Laughlin wave function, fractional charge, topological quantum computing, FQHE, composite fermions
> **Category Tags:** physics, quantum-mechanics, condensed-matter, topology, quantum-computing
> **Cross-References:** [ZA_4_15 — Condensed Matter Physics](../ZA4_Condensed_Matter_Thermodynamics/ZA_4_15_Condensed_Matter_Physics.md) · [ZA_5_05 — Quantum Error Correction](ZA_5_05_Quantum_Error_Correction.md) · [Q_1_16 — Cosmology](../../Q_Cosmology_Physics/Q1_Foundations_Cosmological_Models/Q_1_16_History_of_Cosmology.md)

---

## QUICK SUMMARY

**Anyons** are quasiparticles that exist exclusively in **two-dimensional** systems and obey quantum statistics intermediate between bosons and fermions — when two identical anyons are exchanged, the wave function acquires a phase $e^{i\theta}$ where $0 < \theta < \pi$ (Abelian anyons) or, more dramatically, the system's quantum state undergoes a **unitary matrix transformation** that depends on the topology of the exchange path (non-Abelian anyons). This exotic possibility, impossible in three dimensions where statistics are restricted to bosons ($\theta = 0$) and fermions ($\theta = \pi$) by the topology of the permutation group, was first recognized theoretically by **Jon Magne Leinaas and Jan Myrheim** (1977) and named "anyons" by **Frank Wilczek** (1982). The physical realization of anyons occurs in the **fractional quantum Hall effect (FQHE)**: when a two-dimensional electron gas (2DEG) in a strong perpendicular magnetic field ($B \sim 5-15$ T) is cooled to millikelvin temperatures, the Hall conductance is quantized at fractional values $\sigma_{xy} = \nu \frac{e^2}{h}$ with $\nu = 1/3, 2/5, 5/2, ...$ The FQHE state at $\nu = 1/3$ (Tsui, Störmer, Gossard, 1982) is described by **Laughlin's wave function** (1983), which represents an incompressible quantum liquid whose elementary excitations (quasiholes) carry **fractional electric charge** $e^* = e/3$ and **fractional statistics** $\theta = \pi/3$ — both experimentally confirmed (fractional charge by shot noise measurements, de-Picciotto et al. and Saminadayar et al., 1997; fractional statistics confirmed by interferometry experiments, Bartolomei et al., 2020; Nakamura et al., 2020). The $\nu = 5/2$ state (Moore-Read state) is believed to host **non-Abelian anyons** whose braiding operations are not commutative — making them the basis for **topological quantum computing** (Kitaev, 2003), where quantum information is stored in the global topological properties of anyon configurations and is inherently protected from local perturbations and decoherence.

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Established)

### 1.1 Fractional Quantum Hall Effect
- **Discovery** (Tsui, Störmer, Gossard, 1982; Nobel Prize to Laughlin, Störmer, Tsui in 1998): in a high-mobility GaAs/AlGaAs 2DEG at $B \sim 15$ T and $T \sim 0.5$ K, the Hall resistance exhibits a plateau at $R_{xy} = h/(e^2/3)$ with vanishing longitudinal resistance — the first observation of the FQHE at filling fraction $\nu = 1/3$
- **Laughlin wave function** (1983): $\Psi_m = \prod_{i<j}(z_i - z_j)^m e^{-\sum|z_k|^2/4l_B^2}$ (with $m$ odd integer, $z_i = x_i + iy_i$ complex coordinates, $l_B$ magnetic length) — describes an incompressible quantum liquid at $\nu = 1/m$; the wave function has no adjustable parameters and captures the essential physics
- **Fractional charge**: quasihole excitations of the $\nu = 1/3$ state carry charge $e^* = e/3$ — confirmed by shot-noise experiments (de-Picciotto et al., 1997; Saminadayar et al., 1997) measuring the Fano factor of current fluctuations through a quantum point contact

### 1.2 Abelian Anyonic Statistics
- **Fractional statistics**: when two $e/3$ quasiholes at $\nu = 1/3$ are exchanged, the wave function acquires phase $e^{i\pi/3}$ — neither bosonic (0) nor fermionic ($\pi$); this Abelian anyon statistics was confirmed experimentally by Bartolomei et al. (2020) using anyon collision experiments and by Nakamura et al. (2020) using Fabry-Pérot interferometry
- **Composite fermion theory** (Jain, 1989): the FQHE hierarchy is elegantly explained by attaching $2p$ magnetic flux quanta to each electron, forming "composite fermions" that experience a reduced effective magnetic field and fill integer Landau levels — explains the fractions $\nu = n/(2pn \pm 1)$ forming the Jain sequences

### 1.3 Mathematical Framework
- **Braid group**: in 2D, particle exchange is described by the braid group $B_n$ rather than the permutation group $S_n$ — because particles cannot pass through each other in 2D, the path topology of exchanges matters (braids are not simply permutations); the one-dimensional representations of $B_n$ give Abelian anyons; higher-dimensional representations give non-Abelian anyons

---

## 2. CREDIBLE CLAIMS (Tier 2 — Academic / Debated but Supported)

### 2.1 Non-Abelian Anyons
- **Moore-Read (Pfaffian) state** (1991): proposed wave function for the $\nu = 5/2$ FQHE plateau — $\Psi = \text{Pf}\left(\frac{1}{z_i - z_j}\right) \prod_{i<j}(z_i - z_j)^2 e^{-\sum|z_k|^2/4l_B^2}$ — where the Pfaffian factor produces non-Abelian quasiparticle statistics; the quasiholes obey **Ising anyon** fusion rules
- **Experimental status of $\nu = 5/2$**: the $5/2$ plateau is well established experimentally, but definitive proof that its quasiparticles are non-Abelian remains elusive; recent thermal conductance measurements (Banerjee et al., 2018) and upstream noise experiments have produced conflicting results regarding the topological order

### 2.2 Topological Quantum Computing
- **Kitaev's proposal** (2003): encode qubits in the fusion space of non-Abelian anyons and perform quantum gates by braiding anyons around each other; the quantum information is stored non-locally (in the topological charge of the anyon configuration) and is thus immune to local perturbations — providing intrinsic **topological protection** against decoherence
- **Microsoft's approach**: major investment in topological quantum computing using Majorana zero modes (a type of non-Abelian anyon) at the ends of topological superconductor nanowires; definitive demonstration of topological Majorana qubits is still in progress

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Possible but Unverified)

### 3.1 Universal Topological Quantum Computing
- **Fibonacci anyons**: a theoretical anyon model with fusion rule $\tau \times \tau = 1 + \tau$ — their braiding alone is computationally universal (can approximate any quantum gate to arbitrary precision); proposed to exist in the $\nu = 12/5$ FQHE state (Read-Rezayi state, 1999); no experimental confirmation of Fibonacci anyons exists

---

## 4. DUBIOUS CLAIMS (Tier 4 — No Credible Source / Contradicted by Evidence)

### 4.1 Anyons Can Exist in Three Dimensions
- **[INCORRECT]** The fundamental topological argument (the fundamental group of configuration space is $B_n$ in 2D vs. $S_n$ in 3D) restricts anyons to two-dimensional systems; in 3D, the spin-statistics theorem enforces only bosonic or fermionic statistics for point particles; certain extended objects (strings, loops) in 3D can exhibit analogous exotic statistics, but these are distinct from anyons proper


## COUNTER-ARGUMENTS AND CRITICAL PERSPECTIVES

### Experimental Evidence Remains Indirect
While Bartolomei et al. (2020) and Nakamura et al. (2020) provided strong evidence for anyonic statistics, these experiments measured statistical phase shifts consistent with anyons rather than directly observing braiding operations. The interpretation of these experiments depends on theoretical models of the measurement process, and some physicists argue the evidence remains circumstantial rather than definitive.

### Topological Quantum Computing Faces Enormous Engineering Hurdles
The theoretical elegance of topological quantum computation using non-Abelian anyons (intrinsic error protection via topological encoding) has not translated into practical devices. Majorana zero modes — the leading candidate for non-Abelian anyons — have proven difficult to identify unambiguously in solid-state experiments; several high-profile claims (Mourik et al. 2012, retracted Zhang et al. 2021) have been disputed or retracted, raising concerns about confirmation bias in the field.

### Fractional Quantum Hall States Require Extreme Conditions
The fractional quantum Hall effect — the primary physical platform for anyons — requires ultra-high-purity semiconductor heterostructures, temperatures below 50 mK, and magnetic fields of 5–15 Tesla. These conditions are incompatible with scalable, room-temperature technologies, limiting anyon-based applications to fundamental physics research for the foreseeable future.

### Alternative Approaches May Surpass Topological Error Correction
Conventional (non-topological) quantum error correction schemes using surface codes and superconducting qubits have advanced substantially and may achieve fault tolerance before topological approaches mature. Google's demonstration of below-threshold error correction with surface codes suggests that the engineering path through conventional QEC may be shorter than waiting for reliable non-Abelian anyons.

---
---

## IMAGES

| # | Description | Filename | Source | License |
|---|-------------|----------|--------|---------|
*No images assigned yet.*

---

## BIBLIOGRAPHY

1. Tsui, Daniel C., Horst L. Störmer, and Arthur C. Gossard. "Two-Dimensional Magnetotransport in the Extreme Quantum Limit." *Physical Review Letters* 48.22 (1982): 1559–1562. DOI: 10.1103/physrevlett.48.1559
2. Laughlin, R. B. "Anomalous Quantum Hall Effect: An Incompressible Quantum Fluid with Fractionally Charged Excitations." *Physical Review Letters* 50.18 (1983): 1395–1398. DOI: 10.1103/physrevlett.50.1395
3. Wilczek, Frank. "Quantum Mechanics of Fractional-Spin Particles." *Physical Review Letters* 49.14 (1982): 957–959. DOI: 10.1103/physrevlett.49.957
4. Jain, Jainendra K. *Composite Fermions*. Cambridge: Cambridge University Press, 2007.
5. Nayak, Chetan, et al. "Non-Abelian Anyons and Topological Quantum Computation." *Reviews of Modern Physics* 80.3 (2008): 1083–1159. DOI: 10.1103/revmodphys.80.1083
6. Bartolomei, H., et al. "Fractional Statistics in Anyon Collisions." *Science* 368.6487 (2020): 173–177. DOI: 10.1126/science.aaz5601
7. Nakamura, J., et al. "Direct Observation of Anyonic Braiding Statistics." *Nature Physics* 16 (2020): 931–936.
8. Kitaev, Alexei. "Fault-Tolerant Quantum Computation by Anyons." *Annals of Physics* 303.1 (2003): 2–30.
9. Stern, Ady. "Non-Abelian States of Matter." *Nature* 464 (2010): 187–193.
10. Das Sarma, Sankar, Michael Freedman, and Chetan Nayak. "Topologically Protected Qubits from a Possible Non-Abelian Fractional Quantum Hall State." *Physical Review Letters* 94.16 (2005): 166802.
11. Arovas, Daniel, J. R. Schrieffer, and Frank Wilczek. "Fractional Statistics and the Quantum Hall Effect." *Physical Review Letters* 53.7 (1984): 722–723.
12. Wen, Xiao-Gang. "Topological Orders and Edge Excitations in Fractional Quantum Hall States." *Advances in Physics* 44.5 (1995): 405–473.
13. Stormer, Horst L. "Nobel Lecture: The Fractional Quantum Hall Effect." *Reviews of Modern Physics* 71.4 (1999): 875–889.
14. Halperin, Bertrand I. "Statistics of Quasiparticles and the Hierarchy of Fractional Quantized Hall States." *Physical Review Letters* 52.18 (1984): 1583–1586.
15. Moore, Gregory, and Nicholas Read. "Nonabelions in the Fractional Quantum Hall Effect." *Nuclear Physics B* 360.2–3 (1991): 362–396.
16. Field, Brad, and Tarun Simula. "Introduction to Topological Quantum Computation with Non-Abelian Anyons." *Quantum Science and Technology* 3.4 (2018): 045004.
17. Sarma, Sankar Das, and Ady Stern. "Proposal for a Topological Quantum Computer." *Science* 309.5735 (2005): 738.
18. Bonderson, Parsa, Alexei Kitaev, and Kirill Shtengel. "Detecting Non-Abelian Statistics in the ν = 5/2 Fractional Quantum Hall State." *Physical Review Letters* 96.1 (2006): 016803.
19. Prange, Richard E., and Steven M. Girvin, eds. *The Quantum Hall Effect*. 2nd ed. New York: Springer, 1990. ISBN 9780387971773
20. Wen, Xiao-Gang. *Quantum Field Theory of Many-Body Systems*. Oxford: Oxford University Press, 2004. ISBN 9780198530947
21. Wilczek, Frank. *Fractional Statistics and Anyon Superconductivity*. Singapore: World Scientific, 1990. ISBN 9789810200480


---

## CROSS-REFERENCE INDEX

| Related Doc | Connection |
|-------------|-----------|
| [ZA_5_11](../ZA4_Condensed_Matter_Thermodynamics/ZA_4_15_Condensed_Matter_Physics.md) | Condensed matter physics |
| [ZA_3_13](ZA_5_05_Quantum_Error_Correction.md) | Quantum error correction |
| [Q_1_16](../../Q_Cosmology_Physics/Q1_Foundations_Cosmological_Models/Q_1_16_History_of_Cosmology.md) | Cosmology |

---

*Generated from V4 expansion plan. Last Updated: March 11, 2026*

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
