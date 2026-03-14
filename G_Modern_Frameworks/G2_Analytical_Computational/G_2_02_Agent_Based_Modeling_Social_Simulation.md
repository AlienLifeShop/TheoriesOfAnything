# G_2_02 — Agent-Based Modeling and Social Simulation

> **Source Count:** 19 | **Weighted Score:** 48 | **Source Confidence:** [5/5] | **Primary Tier:** 1–2 | **Last Updated:** March 9, 2026
> **Keywords:** agent-based modeling, ABM, social simulation, computational archaeology, emergence, artificial societies, Sugarscape, NetLogo, complex adaptive systems, Monte Carlo, evolutionary dynamics, forager models, cultural transmission, settlement patterns, collapse modeling, Epstein, Axtell
> **Category Tags:** modern-frameworks, computational-methods, archaeology, social-science, simulation, complexity
> **Cross-References:** [G_3_05 — Self-Organization Emergence](../G3_Theoretical_Frameworks/G_3_05_Self_Organization_Emergence.md) · [G_3_06 — Systems Collapse Complexity](../G3_Theoretical_Frameworks/G_3_06_Systems_Collapse_Complexity_Theory.md) · [G_2_01 — Network Science Trade](G_2_01_Network_Science_Ancient_Trade.md) · [ZD_1_01 — Information Computation](../../ZD_Information_Computation/ZD1_Foundations_Theory/ZD_1_01_Algorithms_Computation_Limits.md) · [ZC_1_01 — Social Science Overview](../../ZC_Social_Science/ZC1_Psychology_Behavior/ZC_1_01_Social_Psychology_Conformity_Obedience.md)

---

## QUICK SUMMARY

**Agent-based modeling (ABM)** is a computational framework in which large numbers of autonomous "agents" — each following simple, individually specified rules — interact with one another and their environment, and complex collective patterns **emerge** from the bottom up without being explicitly programmed. Introduced to social science by **Joshua Epstein** and **Robert Axtell** (*Growing Artificial Societies*, 1996), ABM has become a major tool for studying phenomena that resist top-down analytical solutions: ancient settlement dynamics, the spread of agricultural practices, the collapse of civilizations, the evolution of cooperation, and the transmission of cultural traditions across generations. In archaeology specifically, ABMs have simulated prehistoric forager movement across landscapes, modeled the Ancestral Puebloan abandonment of Long House Valley (the "Artificial Anasazi" project, Axtell et al. 2002), explored the collapse of the Classic Maya polities, and investigated how agricultural innovations spread across Neolithic Europe. The power of ABM lies in its ability to test hypotheses about **mechanisms** — not merely correlating variables but asking "If individual people followed these plausible behavioral rules, would the large-scale pattern we observe actually emerge?" The framework has exposed how simple rules generate surprisingly complex collective behavior, and conversely, how apparently complex social phenomena can sometimes be explained by surprisingly simple micro-level mechanisms.

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Archaeological Record)

### 1.1 Foundations of Agent-Based Modeling
- **Thomas Schelling** (1971, *Journal of Mathematical Sociology*): demonstrated that even mild individual preferences for same-type neighbors produce stark residential **segregation** at the macro level — an early example of emergent social patterning from simple agent rules
- **Epstein & Axtell** (1996, *Growing Artificial Societies: Social Science from the Bottom Up*): created **Sugarscape**, a foundational ABM in which agents harvest resources on a landscape, trade, reproduce, and die — generating emergent wealth inequality, migration patterns, cultural group formation, and combat, all from minimal rules
- ABMs are built in platforms such as **NetLogo** (Wilensky, 1999, Northwestern University) and **Mesa** (Python-based), enabling reproducibility and wide adoption

### 1.2 The Artificial Anasazi Project
- **Axtell, Epstein, Dean, Gumerman, Swedlund, Harburger, and Parker** (*Proceedings of the National Academy of Sciences* 99, suppl. 3, 2002: 7275–7279):
  - Built an ABM of Ancestral Puebloan (Anasazi) households in Long House Valley, northeastern Arizona, ca. 800–1350 CE
  - Agents represented households making decisions about farming location based on maize productivity, water availability, and social factors
  - Environmental data from paleoclimate reconstructions (tree-ring-derived precipitation and temperature) drove the model
  - The model reproduced broad patterns of population growth and settlement location, but **could not fully reproduce the complete abandonment** of the valley ca. 1300 CE using environmental factors alone — suggesting social/political factors (warfare, religious pull factors to the south) were also necessary
  - This was significant as a demonstration both of the power and the limits of environmental-determinist explanations

### 1.3 Spread of Neolithic Agriculture
- ABMs have modeled the spread of farming from the Fertile Crescent across Europe (ca. 9000–4000 BCE):
  - **Demic diffusion models** (based on Ammerman and Cavalli-Sforza's 1984 wave-of-advance model) vs. **cultural diffusion** (adoption by indigenous hunter-gatherers) — ABMs test which mechanism better fits the observed archaeological and genetic evidence
  - Fort (2012, *PNAS*) and related work used agent-based simulations showing that a combination of demic diffusion with ~1 km/year advance and local cultural adoption best fits the radiocarbon dates and ancient DNA evidence

### 1.4 Evolution of Cooperation
- ABMs have been essential in studying the emergence of cooperation:
  - Axelrod's **iterated Prisoner's Dilemma tournaments** (1984) showed that **Tit-for-Tat** — a simple reciprocal strategy — outperforms complex strategies
  - Nowak & May (1992, *Nature*): spatial ABMs on grids showed that cooperation can persist even without memory or reputation, purely through **spatial clustering** — cooperators form clusters that resist invasion by defectors

---

## 2. CREDIBLE CLAIMS (Tier 2 — Academic / Debated but Supported)

### 2.1 Maya Collapse Modeling
- ABMs have explored the Classic Maya collapse (ca. 800–1000 CE):
  - Heckbert et al. (2010) modeled Maya agricultural intensification and environmental degradation, showing how short-term rational decisions (clearing forest, intensifying cultivation) could lead to long-term systemic collapse when soil depletion exceeded recovery rates
  - These models support the "self-organized criticality" view of collapse: systems reach tipping points not because of one dramatic cause but through gradual accumulation of stress
- **Counter-Argument:** ABM results are sensitive to parameter choices; critics argue that models can be tuned to produce almost any outcome, raising questions about their truly predictive (vs. post-hoc explanatory) power

### 2.1a VILLAGES Project (Kohler et al.) — Mesa Verde
- **Village Ecodynamics Project (VEP / VILLAGES)** — Timothy Kohler and collaborators modeled Ancestral Pueblo communities in the central Mesa Verde region, southwestern Colorado, 600–1300 CE
- Agents represent households making decisions about farming, hunting, resource sharing, and conflict on GIS-derived landscapes
- **Key finding:** Models that include inter-group conflict and social stratification better reproduce the archaeological settlement record than models with purely environmental/subsistence drivers — supporting the argument that social dynamics are central to understanding Puebloan history (Kohler et al. 2000; Kohler & van der Leeuw 2007)

### 2.1b Trade Network and Landscape ABMs
- **MERCURY model** (Brughmans & Poblome 2016): ABM of Roman tableware distribution exploring how redistribution, market exchange, and down-the-line trade produce different archaeological distribution patterns — results suggest that observed Roman *terra sigillata* distributions are most consistent with a combination of mechanisms
- **MedLanD** (Barton et al. 2010): Mediterranean landscape dynamics modeling long-term feedback loops between agropastoral land use, soil erosion, vegetation succession, and climate variability — illuminating iterative cycles of cultivation, erosion, abandonment, and re-cultivation

### 2.2 Cultural Transmission and Drift
- ABMs of cultural transmission (Bentley et al., 2004; Mesoudi, 2011) have demonstrated that:
  - Changes in artifact styles (pottery decoration, tool forms) can result from **neutral drift** (random copying) rather than functional selection
  - This has implications for interpreting archaeological style changes — some patterns attributed to cultural meaning may reflect stochastic processes
  - Models of **prestige-biased transmission** (copying high-status individuals) vs. **conformist transmission** (copying the majority) generate different distributional signatures that can be tested against archaeological data

### 2.3 Validation Challenges
- A major methodological debate concerns **validation**: how do we know an ABM is "right" rather than merely fitting data?
  - Pattern-oriented modeling (Grimm et al., 2005) proposes testing models against multiple independent empirical patterns simultaneously
  - Equifinality — different models producing the same output — remains a fundamental challenge

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Possible but Unverified)

### 3.1 Cognitive Agent Architectures
- Incorporating more realistic **cognitive architectures** into archaeological agents — moving beyond simple rule-based decision-making to agents with memory, learning, cultural transmission, and bounded rationality — is an active research frontier. BDI (Belief-Desire-Intention) architectures and reinforcement learning approaches are being explored but remain largely experimental in archaeological contexts (Romanowska et al. 2021).

### 3.2 ABMs for Megastructure Construction
- Researchers have proposed ABMs to model the labor organization required for constructing megalithic monuments (Stonehenge, Göbekli Tepe, Egyptian pyramids):
  - These models attempt to estimate minimum population sizes, coordination requirements, and social hierarchy necessary for such projects
  - While informative, such models depend heavily on assumptions about labor productivity, motivation, social organization, and construction techniques that are poorly constrained by evidence
  - **Counter-Argument:** Reverse-engineering social organization from monumental architecture remains speculative; ABMs add quantitative rigor but do not eliminate fundamental uncertainties about ancient social structures

---

## 4. DUBIOUS CLAIMS (Tier 4 — No Credible Source / Contradicted by Evidence)

### 4.1 ABMs "Prove" Lost Civilizations
- **[DEBUNKED]** Claims that agent-based simulations have "proven" the existence of lost advanced civilizations (e.g., pre-Ice Age global maritime cultures) by showing they are "computationally possible" confuse possibility with evidence; ABMs can show that a scenario is internally consistent but cannot demonstrate that it actually occurred — external archaeological evidence remains required

---

## IMAGES

| # | Description | Filename | Source | License |
|---|-------------|----------|--------|---------|
*No images assigned yet.*

---

## Counter-Arguments & Criticisms

No significant counter-arguments exist in the scholarly literature for the core claims presented here. The topic of Agent Based Modeling Social Simulation represents established knowledge within modern theoretical frameworks with no active scholarly dispute over the fundamental claims presented in this document.

## BIBLIOGRAPHY

1. Epstein, J.M. and Axtell, R. *Growing Artificial Societies: Social Science from the Bottom Up.* MIT Press (1996). DOI: 10.7551/mitpress/3374.001.0001
2. Axtell, R.L. et al. "Population Growth and Collapse in a Multiagent Model of the Kayenta Anasazi." *PNAS* 99, suppl. 3 (2002): 7275–7279. DOI: 10.1073/pnas.092080799
3. Schelling, T.C. "Dynamic Models of Segregation." *Journal of Mathematical Sociology* 1, no. 2 (1971): 143–186. DOI: 10.1080/0022250x.1971.9989794
4. Axelrod, R. *The Evolution of Cooperation.* Basic Books (1984).
5. Nowak, M.A. and May, R.M. "Evolutionary Games and Spatial Chaos." *Nature* 359 (1992): 826–829. DOI: 10.1038/359826a0.
6. Fort, J. "Synthesis Between Demic and Cultural Diffusion in the Neolithic Transition in Europe." *PNAS* 109, no. 46 (2012): 18669–18673. DOI: 10.1073/pnas.1200662109
7. Heckbert, S. et al. "Growing the Ancient Maya Social-Ecological System." In *Proceedings of the International Environmental Modelling and Software Society* (2010).
8. Bentley, R.A. et al. "Random Drift and Culture Change." *Proceedings of the Royal Society B* 271 (2004): 1443–1450.
9. Mesoudi, A. *Cultural Evolution: How Darwinian Theory Can Explain Human Culture.* University of Chicago Press (2011).
10. Grimm, V. et al. "Pattern-Oriented Modeling of Agent-Based Complex Systems." *Science* 310 (2005): 987–991.
11. Wilensky, U. *NetLogo.* Center for Connected Learning, Northwestern University (1999).
12. Ammerman, A.J. and Cavalli-Sforza, L.L. *The Neolithic Transition and the Genetics of Populations in Europe.* Princeton University Press (1984).
13. Gilbert, N. *Agent-Based Models.* 2nd ed. SAGE (2019).
14. Kohler, T.A. and van der Leeuw, S.E., eds. *The Model-Based Archaeology of Socionatural Systems.* SAR Press (2007).
15. Kohler, Timothy A. et al. "Be There Then." *American Antiquity* 65.1 (2000): 137–154.
16. Brughmans, Tom and Poblome, Jeroen. "MERCURY: An Agent-Based Model of Tableware Trade in the Roman East." *JASSS* 19.1 (2016): 3.
17. Barton, C. Michael et al. "Land Use, Water and Mediterranean Landscapes." *Phil. Trans. R. Soc. A* 368.1931 (2010): 5275–5297.
18. Romanowska, Iza, Wren, Colin D., and Crabtree, Stefani A. *Agent-Based Modeling for Archaeology*. SFI Press, 2021.
19. Lake, Mark W. "Trends in Archaeological Simulation." *JAMT* 21.2 (2014): 258–287.

---

## CROSS-REFERENCE INDEX

| Related Doc | Connection |
|-------------|-----------|
| [G_3_05 — Self-Organization Emergence](../G3_Theoretical_Frameworks/G_3_05_Self_Organization_Emergence.md) | Emergence as foundational concept for ABM |
| [G_3_06 — Systems Collapse Complexity](../G3_Theoretical_Frameworks/G_3_06_Systems_Collapse_Complexity_Theory.md) | Collapse dynamics modeled via ABM |
| [G_2_01 — Network Science Trade](G_2_01_Network_Science_Ancient_Trade.md) | Network analysis complementary to ABM |
| [ZC_1_01 — Social Science](../../ZC_Social_Science/ZC1_Psychology_Behavior/ZC_1_01_Social_Psychology_Conformity_Obedience.md) | Social science methodology |
| [W_4_10 — Pueblo Hopi Navajo](../../W_World_Civilizations/W4_Americas_Pacific_Indigenous/W_4_10_Pueblo_Hopi_Navajo_Southwest.md) | Ancestral Puebloan societies modeled |

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
