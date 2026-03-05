# I00 — Section I Sweep Update (2026-02-27)

> Scope: `I01`–`I07` (UAP_Disclosure)  
> Purpose: Add consolidated new findings, source confirmations, and image acquisition status from the Feb 2026 sweep.

---

## 1) Source Confirmation Snapshot (Verified)

The following were directly confirmed from official/public primary sources during this sweep pass:

1. **AARO Reporting Trends page is live and current to Jan 15, 2026**  
   - URL: https://www.aaro.mil/UAP-Cases/UAP-Reporting-Trends/  
   - Confirmed content includes closed-case resolution outcomes, morphology distributions, and altitude distributions.

2. **NARA UAP Records portal and Record Group 615 are live**  
   - URL: https://www.archives.gov/research/topics/uaps  
   - Confirmed content explicitly states NARA established the UAP Records Collection under 2024 NDAA sections 1841–1843 and is adding records on a rolling basis.

3. **FBI Vault UFO collection is live**  
   - URL: https://vault.fbi.gov/UFO  
   - Confirmed content includes multi-part historical FBI UFO files and an official scope disclaimer.

4. **NOAA official domain resources are live for marine/ocean reference context**  
   - URL: https://www.noaa.gov/  
   - Confirmed as valid agency source domain for ocean, charting, and hydroacoustics-linked references.

5. **NASA UAP media assets are available via NASA Science CDN**  
   - Verified downloadable assets include:
     - https://science.nasa.gov/wp-content/uploads/2023/09/uap-report-cover-9-2023.png
     - https://science.nasa.gov/wp-content/uploads/2022/06/uap-meeting-2023-e1692299097471.jpeg

---

## 2) High-Value Additions to Apply Across I01–I07

These are now confirmed as safe add-only updates for section usage:

- **Institutional baseline correction:** AARO trend data shows most closed cases resolve to conventional objects; this is a required control baseline for all anomaly interpretation in `I02`, `I04`, and `I07`.
- **Records governance confirmation:** NARA RG-615 process confirms the disclosure bottleneck is partly procedural (transfer, review, exemptions), not only evidentiary.
- **Methodological guardrail:** Separate four classes in each doc where applicable:
  1) testimony/process evidence,
  2) documentary evidence,
  3) physical artifact evidence,
  4) replicated lab evidence.
- **Uncertainty handling standard:** Use explicit `UNCERTAIN` label where a claim lacks primary chain-of-custody, peer review, or official confirmation.

---

## 3) Image Acquisition Update (This Pass)

### 3.1 Downloaded from direct official/public URLs

- `images/I_UAP_Disclosure/T1_I01_nasa_001_uap_study_report_2023.png`
- `images/I_UAP_Disclosure/T1_I01_nara_001_freedom250_graphic.svg`
- `images/I_UAP_Disclosure/T1_I07_noaa_001_noaa_digital_logo.svg`
- `images/I_UAP_Disclosure/T1_I07_noaa_002_us_flag_small.png`

### 3.2 Normalized by filename alias (existing local source copied to expected corpus naming)

- `T1_I01_nasa_001_uap_study_report_2023.jpg`
- `T1_I02_uap_003_gofast_video_still_2015.jpg`
- `T2_I06_researcher_005_george_knapp_portrait.jpg`
- `T2_I07_uso_003_shag_harbour_memorial.jpg`
- `T1_I07_uso_010_autec_andros_island_aerial.jpg`
- `T3_I05_crash_006_dalnegorsk_height_611_1986.jpg`

### 3.3 Pending image items

A significant number of image filenames referenced in `I01`–`I07` still point to files not present under exact expected names.

- Current referenced filename count: `78`
- Remaining missing by exact filename after this pass: `63`

These require either:
- direct-download from source URLs,
- file-level remapping in docs to existing local assets, or
- controlled fair-use/manual rights workflow for non-public-domain items.

---

## 4) Per-Document Source-Confirmation Notes

### I01
- Confirmed: AARO trend infrastructure, NARA UAP portal/RG-615 continuity.
- `UNCERTAIN`: direct canonical NASA page URL for Mark McInerney article path changed (404 on prior link variant).

### I02
- Confirmed: AARO trend controls support adding a case-confidence rubric.
- `UNCERTAIN`: Some historical media-image assets require rights-cleared source retrieval.

### I03
- Confirmed: NASA UAP report cover/media assets available from NASA CDN.
- Confirmed: AARO trend baseline supports stricter null-hypothesis framing for propulsion inference.

### I04
- Confirmed: NARA and AARO pages support process-evidence framing for nuclear-adjacent archival claims.
- `UNCERTAIN`: several historical nuclear/UAP visuals depend on archive/manual retrieval.

### I05
- Confirmed: FBI Vault UFO corpus available for documentary verification pipeline.
- Confirmed: chain-of-custody guardrail remains mandatory for tiering crash-material claims.

### I06
- Confirmed: institutional/process layer can be documented with hearing/public records + AARO/NARA governance context.
- `UNCERTAIN`: portrait licensing varies for some individuals.

### I07
- Confirmed: NOAA/NARA official resources available for ocean-context and records-context references.
- Confirmed: trans-medium claims should be evaluated with conventional baseline + sensor-chain requirements.

---

## 5) Operational Next Step Queue

1. Resolve the `63` remaining image filename gaps by either:
   - adding direct source URLs in `*_SOURCE.md` stubs, or
   - updating doc filenames to already-downloaded equivalents.
2. Append a short “Source Confirmation (2026-02-27)” subsection into each of `I01`–`I07` with the verified URLs above.
3. Re-run a section image integrity check and produce final zero-missing report.

---

## 6) Reliability/Tier Policy Reinforcement

- Tier 1 must map to directly verifiable primary records or official releases.
- Tier 2 may include strong but debated evidence where method and provenance are explicit.
- Tier 3/4 claims must carry explicit evidentiary caveats and counter-arguments.
- Any unresolved or inaccessible source should be marked `UNCERTAIN` immediately rather than implied as confirmed.

---

## Bibliography

1. Kean, Leslie. *UFOs: Generals, Pilots, and Government Officials Go on the Record*. Harmony Books, 2010.
2. Hynek, J. Allen. *The UFO Experience: A Scientific Inquiry*. Henry Regnery, 1972.
3. Vallée, Jacques. *Passport to Magonia: On UFOs, Folklore, and Parallel Worlds*. Henry Regnery, 1969.
4. Elizondo, Luis. *Imminent: Inside the Pentagon's Hunt for UFOs*. William Morrow, 2024.
5. Dolan, Richard M. *UFOs and the National Security State*. 2 vols. Keyhole Publishing, 2002–2009.
6. Lacatski, James T., Kelleher, Colm A. & Knapp, George. *Inside the U.S. Government Covert UFO Program: Initial Revelations*. RTMA, 2023.
