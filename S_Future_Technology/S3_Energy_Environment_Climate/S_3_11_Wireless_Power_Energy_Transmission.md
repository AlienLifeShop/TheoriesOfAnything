# S_3_11 — Wireless Power and Energy Transmission

> **Source Count:** 0 | **Weighted Score:** 0 | **Source Confidence:** [1/5] | **Primary Tier:** 1–3 | **Last Updated:** March 10, 2026
> **Keywords:** wireless power, energy transmission, inductive coupling, resonant coupling, microwave power beaming, Nikola Tesla, Qi standard, WiTricity, space-based solar power, SBSP, rectenna, far-field power, electromagnetic radiation safety, Wardenclyffe Tower
> **Category Tags:** future technology, energy, physics, engineering, space
> **Cross-References:** [S_3_06 — Renewable Energy](S_3_06_Renewable_Energy_Transformation.md) · [S_3_02 — Energy Futures](S_3_02_Energy_Futures_Fusion_Thorium.md) · [S_4_10 — Space Elevators](../S4_Space_Defense_Risk/S_4_10_Space_Elevators_Launch_Technology.md) · [Q_1_01 — Cosmology](../../Q_Cosmology_Physics/Q1_Foundations_Cosmological_Models/Q_1_01_Anthropic_Principle_Fine_Tuning.md)

---

## QUICK SUMMARY

**Wireless power transmission (WPT)** transfers electrical energy without physical conductors using electromagnetic fields. **Near-field (non-radiative)**: **Inductive coupling** — two coils in close proximity transfer power via oscillating magnetic field; mature technology used in electric toothbrush chargers (since ~1990s), **Qi standard** (Wireless Power Consortium, 2010) for smartphone charging (5–15 W at ≤4 cm range), and increasingly for EV wireless charging (WiTricity, 11 kW at ~10–25 cm air gap; tested by BMW, Hyundai, Genesis); efficiency is high (85–95%) at close range but drops rapidly with distance. **Resonant inductive coupling** — matched resonant frequencies extend range and efficiency; MIT's Marin Soljačić et al. (2007) demonstrated 60 W transfer at 2 meters with ~40% efficiency, leading to WiTricity's commercial technology; the technique enables "spatial freedom" (charge devices positioned freely within a zone rather than precisely on a pad). **Far-field (radiative)**: **Microwave power beaming** — converting electricity to microwaves (typically 2.45 GHz or 5.8 GHz), transmitting through the atmosphere, and converting back to DC via a **rectenna** (rectifying antenna array); demonstrated by William C. Brown (NASA/Raytheon, 1964 — powered a helicopter via microwave beam) and Japanese experiments (2015 — JAXA transmitted 1.8 kW over 55 meters at ~55% efficiency in a lab setting); the key application is **Space-Based Solar Power (SBSP)**: satellites in geostationary orbit collect solar energy 24/7 (no night, no weather, ~8× more energy per m² than ground solar) and beam it as microwaves to Earth-based rectennas; first proposed by Peter Glaser (1968); studied extensively by NASA (1979 SPS reference design: ~5 GW satellite, ~10 km × 5 km), DOE, JAXA, ESA, and China (which announced plans for a demonstration SBSP satellite by 2028). **Laser power beaming** — focused laser beams can transmit power to specific receivers; demonstrated for powering UAVs (PowerLight Technologies, now Equinox Space); useful for niche applications (powering drones, lunar rovers in permanently shadowed craters) but atmospheric absorption and eye safety limit terrestrial use. **Tesla's vision**: Nikola Tesla's Wardenclyffe Tower (1901–1917, Long Island) intended to transmit power wirelessly through the Earth's atmosphere/ground; the project failed commercially and the physics of efficient long-range atmospheric power transmission as Tesla envisioned it does not work — air is a poor conductor and energy would dissipate rapidly. **Current state**: near-field WPT is commercially mature and growing; far-field power beaming works in demonstration but SBSP remains economically challenged — estimated costs of $10–$50 billion for a first operational satellite, with electricity costs initially far above terrestrial solar; launch cost reductions (Starship) could change the economics if costs fall below $100/kg to LEO.

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Scholarly Consensus)

### 1.1 Near-Field Wireless Charging Is Commercially Mature
- Qi-standard inductive charging is used by billions of smartphones and accessories worldwide; efficiency reaches 85–95% at close coupling distances; WiTricity-based resonant wireless EV charging (SAE J2954 standard, 11 kW) has been demonstrated to achieve >90% DC-to-DC efficiency at ~15 cm air gap; the technology is proven, standardized, and commercially deployed

### 1.2 Microwave Power Beaming Is Physically Demonstrated
- Converting electricity to microwaves and back to DC via rectennas is well-established physics — William C. Brown at Raytheon demonstrated this in the 1960s; rectenna conversion efficiency of 80–90% has been achieved in laboratory conditions; the engineering challenge for SBSP is one of scale, cost, and space infrastructure, not fundamental physics

---

## 2. CREDIBLE CLAIMS (Tier 2 — Academic / Debated but Supported)

### 2.1 Space-Based Solar Power May Become Viable
- Recent reviews (European Space Agency 2022 SOLARIS study, US Naval Research Laboratory beam experiments, Caltech SSPP in-orbit demonstration 2023) maintain that SBSP is technically feasible; Caltech's Space Solar Power Demonstrator (launched January 2023) successfully transmitted power wirelessly from orbit for the first time; the question is economic — current estimates suggest SBSP electricity would cost 5–20× more than terrestrial solar unless launch costs fall dramatically and satellite manufacturing scales; proponents argue SBSP's advantage (baseload power 24/7, no storage needed, no land use) justifies the premium for certain applications

### 2.2 Wireless EV Charging on Roadways
- Dynamic wireless charging — embedding inductive coils in roadways to charge EVs while driving — has been demonstrated (Electreon in Sweden and Israel, small test tracks); this would theoretically eliminate range anxiety and reduce battery size requirements; challenges include enormous infrastructure cost ($1–3 million/km), efficiency losses versus wired charging, and the circular dependency of needing widespread adoption before investment is justified

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Possible but Unverified)

### 3.1 Global Wireless Energy Grid
- The vision of transmitting clean energy from high-solar regions (Sahara, space) to population centers via microwave or laser beams, replacing copper/aluminum power lines — this is physically conceivable but would require decades of development, enormous capital, and international cooperation; geopolitical control of energy beams raises security concerns; no serious engineering program is pursuing this at scale

---

## 4. DUBIOUS CLAIMS (Tier 4 — No Credible Source / Contradicted by Evidence)

### 4.1 Tesla's Wardenclyffe Could Have Provided Free Global Energy
- **[DEBUNKED]** Popular myths suggest Tesla's Wardenclyffe Tower was a working system suppressed by J.P. Morgan because it would have provided free energy; the physics does not support efficient long-range atmospheric power transmission at the frequencies and methods Tesla proposed; the Earth's atmosphere is a highly lossy medium; Tesla's vision was ahead of its time in concept but practically infeasible with any known physics; the project failed for technical and financial reasons, not conspiracy

### Counter-Arguments
- Electromagnetic radiation safety: microwave power beaming at SBSP-relevant power densities (~23 mW/cm² at the rectenna center for a 5 GW system) is within international exposure guidelines but public perception of "microwave beams from space" could face severe opposition regardless of actual safety
- Space debris and satellite vulnerability: GEO SBSP satellites would be enormous (~km-scale) and vulnerable to debris impacts; a catastrophic failure could scatter debris in the geostationary belt
- The declining cost of terrestrial solar + battery storage may close the window for SBSP economic viability before it can be deployed — ground solar is now $20–$40/MWh while SBSP estimates are $100–$500/MWh; SBSP advocates argue baseload advantage and land-use savings, but 4-hour batteries + overbuilt solar may achieve similar reliability more cheaply
- Near-field wireless charging is significantly less efficient than wired charging (85–95% vs. 97–99% for wired); at global scale, the efficiency gap translates to substantial wasted energy

---

## IMAGES

| # | Description | Filename | Source | License |
|---|-------------|----------|--------|---------|
*No images assigned yet.*

---

## BIBLIOGRAPHY

- **Kurs, A. et al**. "Wireless Power Transfer via Strongly Coupled Magnetic Resonances." *Science* 317 (2007): 83–86. DOI: 10.1126/science.1143254.
- **Brown, W**. C. "The History of Power Transmission by Radio Waves." *IEEE Trans. Microwave Theory and Techniques* 32 (1984): 1230–1242. DOI: 10.1109/tmtt.1984.1132833
- **Glaser, P**. E. "Power from the Sun: Its Future." *Science* 162 (1968): 857–861. DOI: 10.1126/science.162.3856.857.
- **National Research Council**. *Laying the Foundation for Space Solar Power.* National Academies Press (2001). DOI: 10.17226/10202
- **European Space Agency**. "SOLARIS: Preparing for Space-Based Solar Power." (2022).
- **Caltech**. "Space Solar Power Demonstrator: In-Orbit Results." (2023).
- **Wireless Power Consortium**. "Qi Specification 2.0." (2023).
- **Shinohara, N**. "Wireless Power Transfer via Radiowaves." *IEICE Trans. Electronics* E96-C (2013): 1045–1054. DOI: 10.1002/9781118863008
- **Sasaki, S. et al**. "A New Concept of Solar Power Satellite: Tethered-SPS." *Acta Astronautica* 60 (2007): 153–165.
- **Seif, J**. "The Wardenclyffe Tower: Tesla's Dream of Global Wireless Power." *IEEE Power and Energy Magazine* 12 (2014): 84–92.
- **Electreon**. "Dynamic Wireless Charging: Pilot Results." (2023).

---

## CROSS-REFERENCE INDEX

| Related Doc | Connection |
|-------------|-----------|
| [S_3_06 — Renewable Energy](S_3_06_Renewable_Energy_Transformation.md) | Energy technology |
| [S_3_02 — Energy Futures](S_3_02_Energy_Futures_Fusion_Thorium.md) | Power generation |
| [S_4_10 — Space Elevators](../S4_Space_Defense_Risk/S_4_10_Space_Elevators_Launch_Technology.md) | Space infrastructure |
| [Q_1_01 — Cosmology](../../Q_Cosmology_Physics/Q1_Foundations_Cosmological_Models/Q_1_01_Anthropic_Principle_Fine_Tuning.md) | Solar energy physics |

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
