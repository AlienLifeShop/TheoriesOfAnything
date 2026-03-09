# L25 — Paleogenomics Methods and Ancient DNA

> **Document ID:** L25
> **Section:** L_Genetics_Origins
> **Keywords:** paleogenomics, ancient DNA, aDNA, ancient DNA extraction, petrous bone, DNA degradation, deamination, cytosine deamination, contamination, authentication, next-generation sequencing, NGS, capture enrichment, hybridization capture, shotgun sequencing, library preparation, UDG treatment, single-stranded library, molecular damage patterns, mapDamage, post-mortem damage, ancient DNA revolution, Svante Pääbo, Nobel Prize 2022, environmental DNA, sediment aDNA, cave sediment, proteomic paleontology, ZooMS, dental calculus, paleoproteomics
> **Category Tags:** genetics, human-origins, nde-afterlife, ecology-environment
> **Cross-References:** Z05 — Ancient DNA · [L24 — Ancient African Genetics](L24_Ancient_African_Genetics.md) · Z08 — Human Migration Genetics · [Z29 — Forensic Genetics](L52_Forensic_Genetics_DNA_Identification.md) · [Z25 — Mitochondrial Genetics](L48_Mitochondrial_Genetics_Diseases.md)
> **Reliability Tier:** Tier 1 (Nobel Prize-recognized methodology with rigorous authentication standards)
> **Last Updated:** Mar 7, 2026 | **Source Count:** 10 | **Weighted Score:** 28 | **Source Confidence:** [3/5] | **Confidence:** High

---

## QUICK SUMMARY

**Paleogenomics** — the study of ancient genomes — has transformed archaeology, anthropology, and evolutionary biology over the past two decades, recognized by the 2022 **Nobel Prize in Physiology or Medicine** awarded to **Svante Pääbo** for his pioneering work sequencing the Neanderthal genome. Ancient DNA (aDNA) is typically highly **degraded** — fragmented to 30–80 bp average length, chemically modified by post-mortem **cytosine deamination** (C→U transitions concentrated at fragment termini, the hallmark damage pattern), present at extremely low quantities mixed with overwhelming microbial DNA (often >95% of extracted DNA is microbial), and vulnerable to contamination from modern human DNA. The methodological revolution enabling modern paleogenomics rests on several key innovations: **next-generation sequencing (NGS)** — massively parallel sequencing (Illumina platforms) ideally suited to short, fragmented aDNA molecules (vs. Sanger sequencing which required longer intact fragments); **single-stranded library preparation** (Gansauge & Meyer 2013) — recovering DNA fragments that denature in standard double-stranded protocols, increasing yield 2–10× especially from the most degraded samples; **hybridization capture enrichment** — using synthetic RNA or DNA probes (baits) to selectively pull target sequences (e.g., all human DNA, specific genes, mtDNA) from a complex mixture of microbial and endogenous DNA, dramatically increasing the proportion of informative sequences (from <1% to 30–60% human in enriched libraries); **petrous bone extraction** (Pinhasi et al. 2015) — the dense inner ear bone preserves up to 100× more endogenous DNA than other skeletal elements (teeth are second-best) due to its extreme density limiting microbial colonization; **authentication criteria** including characteristic post-mortem damage patterns (verified by mapDamage/PMDtools software), short fragment length distributions, consistent phylogenetic placement, contamination estimation (proportion of modern human mtDNA), and sex determination consistency; **sediment aDNA** (Slon et al. 2017) — recovering ancient hominin and animal DNA directly from cave sediments without macroscopic fossils, expanding paleogenomic sampling to sites where bones are absent; and **paleoproteomics** (ZooMS, mass spectrometry-based protein identification from bone collagen) — providing taxonomic identification and even phylogenetic information from samples too old or too degraded for DNA survival (e.g., *Homo antecessor* ~800,000 years old, Welker et al. 2020). The oldest authenticated ancient DNA to date comes from ~2-million-year-old sediments in Greenland (Kjær et al. 2022) and ~1.2-million-year-old mammoth teeth (van der Valk et al. 2021), far exceeding the previously assumed ~500,000-year theoretical limit for DNA survival.

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Established)

### 1.1 DNA Degradation and Damage Patterns

- **Fragmentation:** After cell death, endogenous nucleases and hydrolysis cleave DNA — ancient DNA molecules are typically 30–80 bp (some as short as 20 bp, rarely >200 bp); fragment length decreases with age and temperature of preservation
- **Cytosine deamination:** The signature chemical modification — hydrolytic deamination converts cytosine to uracil (read as thymine by polymerases) → C→T transitions at 5' ends and G→A transitions at 3' ends of fragments; frequency increases with age and is concentrated in the terminal 1–3 positions; this damage pattern serves as an authentication criterion — it is present in genuine ancient DNA but absent in modern contamination
- **Depurination and strand breaks:** Loss of purine bases (adenine, guanine) creates abasic sites → strand breakage; explains the fragmented nature of aDNA
- **Cross-links:** Inter-strand cross-links from Maillard reactions (sugar–amino acid) impede PCR amplification and library preparation; enzymatic treatment (PreCR, Endonuclease VIII) can partially repair these
- **Preservation factors:** Cold, dry, stable environments preserve DNA best — permafrost (Siberia, Greenland), high-altitude caves, arid caves (dry African sites), waterlogged anoxic sediments; tropical heat and humidity are worst (see L24)

### 1.2 Sample Selection and Extraction

- **Petrous bone revolution (Pinhasi et al. 2015):** The petrous portion of the temporal bone — the densest bone in the mammalian skeleton — yields dramatically more endogenous DNA than other skeletal elements; systematic testing showed 4–16% endogenous human DNA in petrous bones vs. <1% in most other bones from the same skeletons; this single advance transformed the field by making marginal samples salvageable
- **Teeth:** Second-best source — cementum (root) preserves better than dentine; provides independent verification of petrous bone results from the same individual
- **Dental calculus:** Mineralized plaque contains dietary DNA (plant, animal), oral microbiome DNA, and human host DNA — provides information on diet, disease, and oral health not obtainable from bone alone (Warinner et al. 2014)
- **Extraction protocols:** Silica-based extraction in dedicated clean rooms (positive-pressure with HEPA filtration, UV irradiation, full-body protective clothing); bone surfaces are bleach-decontaminated and UV-treated before drilling/grinding; multiple extraction blanks and library blanks at every step

### 1.3 Library Preparation and Sequencing

- **Double-stranded library preparation:** Standard aDNA protocol — blunt-end repair → adapter ligation → fill-in → amplification; works for fragments >30 bp
- **Single-stranded library preparation (Gansauge & Meyer 2013):** Denatures DNA to single strands → ligates adapters to single-stranded molecules directly; recovers 2–10× more unique molecules from the same extract, especially the shortest and most damaged fragments; critical for the most degraded samples (very old, warm climates)
- **UDG treatment:** Uracil-DNA glycosylase removes deaminated cytosines before library amplification — eliminates C→T artifacts from downstream sequences but slightly reduces library complexity; partial UDG treatment preserves damage at terminal positions for authentication while cleaning internal positions
- **Next-generation sequencing:** Illumina short-read platforms are ideal — read lengths of 50–150 bp match aDNA fragment lengths; single-end and paired-end sequencing; low DNA quantity compensated by deep sequencing; cost per genome has dropped from >$100,000 (2010) to <$500 (2025) for low-coverage genomes

### 1.4 Enrichment Strategies

- **Shotgun sequencing:** Sequences all DNA in a library — typically >95% is microbial/environmental; useful for samples with high endogenous content (permafrost, petrous bone with >5% endogenous DNA)
- **In-solution hybridization capture:** Synthetic biotinylated RNA or DNA probes (baits) designed to match target sequences → hybridized with the aDNA library → captured on streptavidin beads → eluted and sequenced; enriches target sequences 100–1,000-fold
  - *"1240k capture" (Mathieson et al. 2015):* ~1.24 million informative SNPs targeted — population-level human variation; the workhorse for population paleogenomics; >90% of published ancient human genomes use this panel
  - *mtDNA capture:* Complete mitochondrial genome enrichment — requires much less starting DNA than nuclear genome analysis; the entry-level analysis for poorly preserved samples
  - *Whole-genome capture:* Probes tiling the entire human genome — used for higher-resolution analyses; more expensive but avoids ascertainment bias of SNP panels

---

## 2. CREDIBLE CLAIMS (Tier 2 — Strong Evidence, Active Research)

### 2.1 Authentication and Contamination Control

- **Contamination — the central challenge:** Modern human DNA from excavators, laboratory personnel, and reagents can infiltrate ancient samples; aDNA labs enforce strict protocols:
  - Physical separation: Extraction and library preparation in dedicated clean rooms separate from post-amplification labs; one-way workflow
  - Negative controls: Extraction blanks, library blanks processed alongside samples at every step
  - **mapDamage/PMDtools:** Software quantifying C→T transition rates at fragment termini — genuine aDNA shows elevated damage (>10% at first position for Pleistocene-age samples); modern contamination shows flat damage profiles
  - Ancient DNA criteria: (1) Short fragment length distribution consistent with degradation; (2) Characteristic damage patterns; (3) Contamination estimation — mtDNA-based (proportion of non-matching mtDNA sequences) and nuclear-based (X-chromosome contamination in males); (4) Consistent sex determination between methods; (5) Reproducibility — independent extraction and library from same specimen
- **Contamination estimation:** For males, X chromosome contamination is estimated from heterozygosity at known SNPs (males are hemizygous → any heterozygous calls indicate contamination); ANGSD and contamMix software tools are standard

### 2.2 Sediment aDNA (Sedimentary Ancient DNA)

- **Innovation (Slon et al. 2017):** Ancient DNA extracted from **cave sediments** without any macroscopic fossils — hominin DNA, Neanderthal DNA, Denisovan DNA, and animal DNA recovered from sediment layers in Denisova Cave and other sites; expands paleogenomics to sites and time periods without skeletal remains
- **Process:** Sediment samples collected under sterile conditions → DNA extracted → capture enrichment for mtDNA of target taxa → sequencing and authentication (same damage patterns as bone-derived aDNA)
- **Achievements:** Neanderthal mtDNA detected in sediments from 12 European cave sites (Slon et al. 2017; Zavala et al. 2021); nuclear DNA recovery from sediment is much more challenging but has been achieved (Vernot et al. 2021 — nuclear DNA from Denisova Cave and Galería de las Estatuas, Spain)
- **Environmental DNA (eDNA) for ecosystems:** Sediment aDNA also recovers DNA from plants, animals, and microorganisms — reconstructing ancient ecosystems without macrofossils; the 2-million-year-old Greenland eDNA (Kjær et al. 2022) revealed a forested Arctic ecosystem with mastodons, reindeer, and diverse plants

### 2.3 Paleoproteomics

- **ZooMS (Zooarchaeology by Mass Spectrometry):** Collagen peptide mass fingerprinting from bone fragments — rapid, low-cost taxonomic identification; can screen thousands of unidentified bone fragments and identify species from fragments too small for morphological identification; ZooMS identified a Neanderthal-Denisovan hybrid individual (Denisova 11/"Denny") by screening thousands of bone chips from Denisova Cave (Douka et al. 2019)
- **Deep-time proteomics:** Proteins survive longer than DNA — enamel proteome from 1.77-million-year-old *Homo erectus* (Welker et al. 2020 — *Homo antecessor* ~800,000 years old, from Atapuerca, Spain); amino acid sequence from collagen and enamel proteins can provide phylogenetic information beyond DNA survival limits
- **Dental calculus proteomics:** Medieval dental calculus showing β-lactoglobulin (milk protein) reveals dairy consumption history (Warinner et al. 2014; Hendy et al. 2018)

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Emerging / Theoretical)

### 3.1 Pushing the Age Limit

- **2-million-year-old eDNA (Kjær et al. 2022):** DNA from Greenland sediments dated to ~2 million years ago — far exceeding previous oldest authenticated ancient DNA (~1.2 million years from mammoth teeth); suggests DNA survival in permafrost may extend further; however, these are short fragments adsorbed to mineral particles, and recovery is site-specific
- **Theoretical limits:** DNA half-life calculations predict complete hydrolysis of 500 bp fragments within ~6.8 million years at 15°C (Allentoft et al. 2012), but much longer survival is possible in cold (<0°C) stable environments where degradation kinetics slow dramatically; the practical limit depends heavily on preservation conditions

### 3.2 Epigenomics of Ancient DNA

- **Ancient methylation:** Deamination patterns differ for methylated vs. unmethylated cytosines (5-methylcytosine deaminates to thymine, not uracil — thus not removed by UDG); this difference allows computational reconstruction of ancient methylation maps from shotgun sequencing data; applied to Neanderthal and Denisovan methylation revealing gene regulation differences from modern humans (Gokhman et al. 2014, 2019); highly promising but technically challenging

---

## 4. DUBIOUS CLAIMS (Tier 4 — Fringe / Unsubstantiated)

### 4.1 "Jurassic Park" DNA Recovery [DEBUNKED]

- Claims of DNA recovery from amber-preserved insects (millions of years old) or dinosaur bones have been thoroughly debunked — all published Cretaceous/Jurassic DNA results were artifacts of modern contamination or microbial DNA; DNA chemistry imposes hard degradation limits (even under ideal preservation, no recoverable DNA sequences beyond ~6–7 million years); dinosaur "DNA" claims from the 1990s have been retracted or discredited

---

## IMAGES

| # | Description | Source |
|---|-------------|--------|
| 1 | C→T damage pattern from mapDamage output | Jónsson et al. 2013 |
| 2 | Petrous bone anatomy and sampling location | Pinhasi et al. 2015 |
| 3 | In-solution hybridization capture workflow | Mathieson et al. 2015 |

---

## BIBLIOGRAPHY

1. Pääbo, S. (2014). *Neanderthal Man: In Search of Lost Genomes*. Basic Books.
2. Pinhasi, R. et al. (2015). "Optimal Ancient DNA Yields from the Inner Ear Part of the Human Petrous Bone." *PLoS ONE*, 10(6), e0129102.
3. Gansauge, M.-T. & Meyer, M. (2013). "Single-Stranded DNA Library Preparation for the Sequencing of Ancient or Damaged DNA." *Nature Protocols*, 8(4), 737–748.
4. Slon, V. et al. (2017). "Neandertal and Denisovan DNA from Pleistocene Sediments." *Science*, 356(6338), 605–608.
5. Mathieson, I. et al. (2015). "Genome-Wide Patterns of Selection in 230 Ancient Eurasians." *Nature*, 528, 499–503.
6. Kjær, K. H. et al. (2022). "A 2-Million-Year-Old Ecosystem in Greenland Uncovered by Environmental DNA." *Nature*, 612, 283–291.
7. Allentoft, M. E. et al. (2012). "The Half-Life of DNA in Bone: Measuring Decay Kinetics in 158 Dated Fossils." *Proceedings of the Royal Society B*, 279(1748), 4724–4733.
8. Welker, F. et al. (2020). "The Dental Proteome of Homo antecessor." *Nature*, 580, 235–238.
9. Gokhman, D. et al. (2014). "Reconstructing the DNA Methylation Maps of the Neandertal and the Denisovan." *Science*, 344(6183), 523–527.
10. Warinner, C. et al. (2014). "Pathogens and Host Immunity in the Ancient Human Oral Cavity." *Nature Genetics*, 46(4), 336–344.

---

## CROSS-REFERENCE INDEX

- **Z05 — Ancient DNA:** Core ancient DNA findings and key genomes sequenced
- **[L24 — Ancient African Genetics](L24_Ancient_African_Genetics.md):** Technical challenges of aDNA in tropical Africa
- **Z08 — Human Migration Genetics:** Paleogenomic evidence for migration routes
- **[Z29 — Forensic Genetics](L52_Forensic_Genetics_DNA_Identification.md):** Shared degraded DNA recovery techniques
- **[Z25 — Mitochondrial Genetics](L48_Mitochondrial_Genetics_Diseases.md):** mtDNA capture and analysis in ancient samples

---

*Last verified: Mar 07, 2026 — All sources peer-reviewed or from established paleogenomics literature*
