# ZF_4_12 — Underwater Acoustics and the SOFAR Channel

> **Source Count:** 0 | **Weighted Score:** 0 | **Source Confidence:** [1/5] | **Primary Tier:** 1–2 | **Last Updated:** March 10, 2026
> **Keywords:** underwater acoustics, SOFAR channel, sound propagation, deep sound channel, sonar, SOSUS, hydrophone, whale communication, acoustic tomography, ocean noise, sound speed profile, acoustic refraction, shadow zone, convergence zone, ambient noise
> **Category Tags:** oceanography, acoustics, marine biology, military history, ocean monitoring
> **Cross-References:** [ZF_4_04 — Marine Bioacoustics](ZF_4_04_Ocean_Acoustics_Sound_Channels.md) · [J_1_04 — Ancient Acoustic Technology](../../J_Ancient_Technology/J1_Energy_Acoustic_Advanced/J_1_04_Acoustic_Vibrational_Technology.md) · [S_3_10 — Unexplained Sounds](../../S_Future_Technology/S3_Energy_Environment_Climate/S_3_10_Ocean_Technology_Deep_Sea.md) · [ZF_3_12 — Submarines and History of Exploration](../ZF3_Maritime_History_Culture/ZF_3_12_Submarines_History_Exploration.md)

---

## QUICK SUMMARY

**Sound** is the dominant long-range information carrier in the ocean — electromagnetic radiation (light, radio) is rapidly absorbed in seawater, but sound can travel thousands of kilometers with remarkably little loss, making acoustics the primary tool for underwater communication, navigation, detection, and scientific observation. The speed of sound in seawater (~1,450–1,560 m/s — roughly 4.3× faster than in air) depends on three variables: **temperature** (increases ~4.5 m/s per °C), **salinity** (increases ~1.3 m/s per psu), and **pressure** (increases ~1.7 m/s per 100 m depth). In most ocean basins, the interplay of decreasing temperature and increasing pressure with depth creates a characteristic sound speed minimum at approximately 600–1,200 m depth — this minimum defines the axis of the **SOFAR channel** (Sound Fixing and Ranging), also called the **deep sound channel**, discovered independently by Maurice Ewing and J. Lamar Worzel (1948) and Leonid Brekhovskikh (USSR, 1946). Sound waves generated near the SOFAR axis are refracted (bent) back toward the axis by Snell's law: waves traveling upward enter faster water and are bent back down; waves traveling downward enter faster water (due to pressure) and are bent back up — trapping the sound in a waveguide with cylindrical spreading loss (~1/r) rather than the spherical spreading (~1/r²) of unconfined sound. This channeling allows extraordinarily long-range propagation: in 1960, a 1-kg explosive charge detonated in the SOFAR channel off Perth, Australia, was detected by hydrophones in Bermuda — a distance of **19,200 km**, nearly halfway around the globe. The SOFAR channel has three consequential applications: **(1) military surveillance** — the U.S. Navy's **SOSUS** (Sound Surveillance System), deployed during the Cold War (1950s–1990s), consisted of arrays of bottom-mounted hydrophones connected by undersea cable to shore processing facilities, primarily for tracking Soviet submarines by their acoustic signatures (cavitation, machinery tonals, propeller blade-rate harmonics); **(2) ocean acoustic tomography** — pioneered by Munk and Wunzel (1979), uses precisely timed sound pulses transmitted across ocean basins to measure water temperature along the ray path (since sound speed depends on temperature) — enabling basin-scale temperature monitoring that complements point measurements from Argo floats; **(3) marine biology** — baleen whales (especially blue whales, fin whales) produce extremely low-frequency calls (14–25 Hz) that propagate along the SOFAR channel axis, enabling communication across entire ocean basins — fin whale 20 Hz calls have been detected at ranges >3,000 km. **Anthropogenic ocean noise** has increased by ~32 dB in low-frequency bands (<300 Hz) over the 20th century, driven by commercial shipping (the dominant source), seismic airgun surveys (oil/gas exploration), and naval sonar. This noise increase has been shown to affect marine mammal behavior, communication range (for right whales, communication range may have shrunk from ~1,600 km historically to ~160 km today — a 90% reduction), and potentially foraging success and reproductive rates.

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Scholarly Consensus)

### 1.1 Sound Speed Profile and the SOFAR Channel
- Sound speed in seawater follows the empirical equation: c ≈ 1449.2 + 4.6T − 0.055T² + 0.00029T³ + (1.34 − 0.010T)(S − 35) + 0.016z (UNESCO formula; T = temperature °C, S = salinity psu, z = depth m)
- The SOFAR channel axis (sound speed minimum) lies at ~600–1,200 m depth at mid-latitudes, shallowing toward the poles (where cold surface water brings the minimum near the surface) and deepening in warm tropical waters
- Ewing and Worzel (1948) demonstrated that small explosive charges detonated near the SOFAR axis could be detected at ranges >3,000 km — proposing its use as a signaling system for downed pilots (the original "Sound Fixing and Ranging" application)
- The SOFAR channel functions as an acoustic waveguide: sound is continuously refracted toward the axis of minimum speed, with energy trapped between the upper and lower turning depths — propagation loss follows cylindrical spreading (~1/r) rather than spherical (~1/r²), enabling transmission across ocean basins

### 1.2 SOSUS and Military Submarine Detection
- The U.S. Navy developed SOSUS (Sound Surveillance System) beginning in the early 1950s under Project Jezebel/Caesar — the system consisted of large bottom-mounted hydrophone arrays (typically at depths of 1,000–3,000 m) positioned along continental margins in the Atlantic and Pacific, connected to shore stations by submarine cable
- SOSUS was designed to detect and track Soviet submarines by their acoustic signatures: machinery noise, propeller cavitation, and tonal signatures unique to each submarine class; at peak capability, SOSUS could detect submarines at ranges >1,000 km
- After the Cold War, portions of SOSUS were declassified and repurposed for scientific use — detecting submarine volcanic eruptions, earthquake T-phases, and tracking whale calls across ocean basins (Nishimura & Conlon, 1993; Stafford et al., 1999)

### 1.3 Anthropogenic Ocean Noise
- Low-frequency ocean ambient noise (<300 Hz) has increased by approximately 3.3 dB per decade (10 dB total from 1960 to 2000), primarily driven by the doubling of the global commercial shipping fleet between 1965 and 2003
- Seismic airgun arrays used in hydrocarbon exploration produce impulsive sounds of 220–260 dB re 1 μPa at source, detectable at ranges >4,000 km in the SOFAR channel
- Military mid-frequency active sonar (MFA, 1–10 kHz, 235+ dB source level) has been implicated in mass strandings of beaked whales (Ziphius cavirostris) — D'Amico et al. (2009) documented 12+ stranding events temporally and spatially coincident with naval sonar exercises

---

## 2. CREDIBLE CLAIMS (Tier 2 — Academic / Debated but Supported)

### 2.1 Ocean Acoustic Tomography
- Munk and Wunzel (1979) proposed that precisely timed sound pulses transmitted between known source-receiver pairs across ocean transects could be used to measure average temperature along each ray path — since sound speed depends on temperature, travel-time changes reveal temperature changes
- The U.S. ATOC (Acoustic Thermometry of Ocean Climate) project in the 1990s demonstrated that basin-scale temperature trends could be measured with precision of ~0.01°C using trans-Pacific acoustic paths — but was controversial due to concerns about effects on marine mammals
- Modern ocean monitoring increasingly relies on Argo floats and satellite altimetry, but acoustic methods remain uniquely capable of providing depth-integrated temperature measurements across entire ocean basins in near-real-time

### 2.2 Whale Communication via SOFAR Channel
- Blue whale calls (15–25 Hz fundamental) and fin whale 20 Hz pulses are produced at or near the SOFAR channel axis depth and propagate for thousands of kilometers — Stafford et al. (1998) tracked fin whale calls on SOSUS arrays at ranges >3,000 km
- Payne and Webb (1971) first hypothesized that fin whales use the SOFAR channel for long-range communication, estimating a "pre-industrial" communication range of ~1,600 km — now reduced by ~90% due to increased shipping noise in the 20 Hz band
- Whether whales consciously exploit the SOFAR channel or simply vocalize at depths that happen to coincide with the channel axis is debated — but the match between whale call frequencies, source depths, and SOFAR propagation characteristics is striking

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Possible but Unverified)

### 3.1 "The Bloop" and Unidentified Acoustic Events
- In 1997, NOAA's autonomous hydrophone arrays detected several ultra-low-frequency sounds of unknown origin (notably "The Bloop," "Slow Down," "Julia," and "Upsweep") — initially, their source was debated (biological? geological? anthropogenic?)
- NOAA subsequently attributed most of these sounds to icequakes — the fracturing and calving of large icebergs — based on frequency content, propagation characteristics, and correlation with satellite-observed iceberg positions (see O_1_02)
- Some internet speculation attributed these sounds to unknown deep-sea creatures, but no credible evidence supports a biological origin for the events

---

## 4. DUBIOUS CLAIMS (Tier 4 — No Credible Source / Contradicted by Evidence)

### 4.1 Atlantis Detected via Underwater Sonar
- **[NO CREDIBLE EVIDENCE]** Claims that sonar surveys have detected ruins of Atlantis or other lost civilizations on the ocean floor confuse natural geological formations (e.g., rectangular jointing patterns in basalt, tectonic lineaments) with artificial structures — no verifiable sonar survey has identified anthropogenic structures inconsistent with known maritime archaeology

---

## COUNTER-ARGUMENTS

- **ATOC controversy**: **Walter Munk's** Acoustic Thermometry of Ocean Climate (ATOC) program — proposing to use low-frequency sound transmission through the SOFAR channel to measure ocean temperature changes — generated significant controversy over potential harm to marine mammals. Environmentalists and some marine biologists argued that chronic low-frequency noise could disrupt whale communication and behavior, while ATOC proponents maintained the sound levels were below harmful thresholds. The controversy highlighted the tension between oceanographic research needs and marine mammal protection
- **Cetacean SOFAR channel use**: Whether large whales consciously exploit the SOFAR channel for long-range acoustic communication or whether their vocalizations simply happen to propagate through it as a byproduct of the ocean's acoustic physics is debated — direct evidence of intentional SOFAR-mediated communication is difficult to obtain

---

## IMAGES

| # | Description | Filename | Source | License |
|---|-------------|----------|--------|---------|
*No images assigned yet.*

---

## BIBLIOGRAPHY

- **Ewing, M. & Worzel, J.L. "Long-Range Sound Transmission." *GSA Memoir 27* (1948): 1–32.**
- **Urick, R.J**. *Principles of Underwater Sound.* 3rd ed. New York: McGraw-Hill, 1983.
- **Munk, W. et al**. *Ocean Acoustic Tomography.* Cambridge: Cambridge University Press, 1995. ISBN: 0511886217
- **Munk, W**. & Wunzel, C. "Ocean Acoustic Tomography: A Scheme for Large Scale Monitoring." *Deep-Sea Research* 26A (1979): 123–161. DOI: 10.1016/0198-0149(79)90073-6
- **Payne, R**. S. & Webb, D. "Orientation by Means of Long Range Acoustic Signaling in Baleen Whales." *Annals of the New York Academy of Sciences* 188 (1971): 110–141. DOI: 10.1111/j.1749-6632.1971.tb13093.x.
- **Stafford, K.M. et al**. "Long-Range Detection and Localization of Blue Whale Calls in the Northeast Pacific Ocean Using Military Hydrophone Arrays." *JASA* 104 (1998): 3616–3625. DOI: 10.1121/1.423944
- **Andrew, R.K. et al**. "Ocean Ambient Sound: Comparing the 1960s with the 1990s for a Receiver off the California Coast." *Acoustics Research Letters Online* 3 (2002): 65–70. DOI: 10.1121/1.1461915
- **McDonald, M.A. et al**. "Increases in Deep Ocean Ambient Noise in the Northeast Pacific West of San Nicolas Island, California." *JASA* 120 (2006): 711–718. DOI: 10.1121/1.2216565
- **D'Amico, A. et al**. "Beaked Whale Strandings and Naval Exercises." *Aquatic Mammals* 35 (2009): 452–472. DOI: 10.1578/AM.35.4.2009.452.
- **Sohn, R.A. et al**. "Three-Dimensional Tomographic Imaging of Upper Ocean Temperature Using SOSUS Hydrophones." *Journal of Geophysical Research* 100 (1995): 6607–6614. DOI: 10.1029/95JC00380
- **Jensen, F.B. et al**. *Computational Ocean Acoustics.* 2nd ed. New York: Springer, 2011. DOI: 10.1007/978-1-4419-8678-8
- **Wilcock, W.S.D. et al**. "Sounds in the Ocean at 1–100 Hz." *Annual Review of Marine Science* 6 (2014): 117–140. DOI: 10.1146/annurev-marine-121211-172423
- **Fox, C.G. et al**. "Hydroacoustic Detection of a Volcanic Eruption on the Gorda Ridge, June–July 1996." *Deep-Sea Research II* 48 (2001): 2331–2354. DOI: 10.1016/S0967-0645(00)00173-2


## CROSS-REFERENCE INDEX

| Related Doc | Connection |
|-------------|-----------|
*No cross-references yet.*

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
