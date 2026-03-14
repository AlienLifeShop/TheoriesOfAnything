# L_4_09 — Selective Sweeps and Positive Selection in Humans

> **Source Count:** 14 | **Weighted Score:** 40 | **Source Confidence:** [4/5] | **Primary Tier:** 1–2 | **Last Updated:** March 9, 2026
> **Keywords:** selective sweep, positive selection, natural selection, allele frequency, hitchhiking, extended haplotype homozygosity, iHS, Fst, population differentiation, LCT, SLC24A5, EDAR, adaptation, genomic scan, recent human evolution
> **Category Tags:** genetics, evolution, population genetics, adaptation, genomics
> **Cross-References:** [L_3_03 — Lactase Persistence Gene-Culture](../L3_Adaptation_Traits/L_3_03_Lactase_Persistence_Gene_Culture.md) · [L_1_05 — Human Skin Color Evolution](../L1_Human_Evolution_Species/L_1_05_Human_Skin_Color_Evolution.md) · [L_5_11 — Genetic Adaptation Altitude](../L5_Health_Microbiome_Applied/L_5_11_Altitude_Adaptation.md) · [L_2_02 — Population Genetics Hardy-Weinberg](../L2_Population_Regional_Genetics/L_2_02_Population_Genetics_Hardy_Weinberg.md)

---

## QUICK SUMMARY

A **selective sweep** occurs when a beneficial allele rises rapidly in frequency under **positive natural selection**, carrying nearby linked variants along with it (**genetic hitchhiking**) and reducing genetic variation across the surrounding chromosomal region. Detecting selective sweeps in the human genome is one of the primary methods for identifying loci that have undergone **recent adaptive evolution** — revealing how human populations have adapted to local environments (diet, disease, climate, altitude) over the last ~50,000–100,000 years. Statistical methods for identifying sweeps include: (1) **Extended Haplotype Homozygosity (EHH) / iHS tests** — detecting unusually long haplotype blocks (indicative of a favored allele that swept to high frequency faster than recombination could break down surrounding linkage disequilibrium); (2) **Fst-based population differentiation** — identifying loci with extreme allele-frequency differences between populations, suggesting local adaptation; (3) **Composite likelihood ratio (CLR) / SweepFinder** — modeling the site frequency spectrum expected around a sweep; (4) **Tajima's D and related neutrality tests** — detecting shifts in allele frequency distributions. Landmark examples of detected selective sweeps include: **LCT** (lactase persistence, strongest sweep in European genomes, ~7,500 years ago — L_3_03), **SLC24A5** (light skin pigmentation in Europeans — L_1_05), **EDAR** (ectodysplasin A receptor, affecting hair thickness, tooth morphology, and sweat gland density in East Asians), **EPAS1** (altitude adaptation in Tibetans — L_4_09), and **DARC/Duffy** (Duffy-null allele conferring malaria resistance in sub-Saharan Africans). Genome-wide scans have identified hundreds of loci with evidence of positive selection, though distinguishing true adaptive sweeps from demographic effects (population bottlenecks, expansions) remains a methodological challenge.

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Scholarly Consensus)

### 1.1 Theory of Selective Sweeps
- Maynard Smith & Haigh (1974) first described the hitchhiking effect: when a beneficial mutation sweeps to fixation, linked neutral variants "hitchhike" to high frequency, creating a valley of reduced diversity surrounding the selected site
- **Hard sweeps** occur when a single new beneficial mutation rapidly reaches fixation; **soft sweeps** occur when selection acts on standing variation (multiple haplotypes carrying the beneficial allele, leaving weaker footprints)
- The genomic signature of a recent hard sweep: (a) reduced nucleotide diversity near the selected site; (b) excess of high-frequency derived alleles; (c) extended haplotype homozygosity (long blocks of identical sequence); (d) skewed allele-frequency spectrum (negative Tajima's D)

### 1.2 Classic Examples of Human Selective Sweeps
- **LCT/MCM6** (lactase persistence): the −13,910*T allele enabling adult lactose digestion shows the strongest signal of positive selection in European genomes; the selected haplotype extends ~1 Mb — evidence of a sweep within the last ~7,500 years, coinciding with dairy farming adoption (Bersaglieri et al., 2004, *American Journal of Human Genetics*)
- **SLC24A5** (rs1426654): a single amino acid change (Ala111Thr) explains ~25–38% of the skin pigmentation difference between Europeans and West Africans; the derived allele is nearly fixed in Europeans (~99%) and shows strong evidence of positive selection within the last ~10,000–20,000 years (Lamason et al., 2005, *Science*)
- **EDAR** (rs3827760, V370A): the derived allele at high frequency in East Asians and Native Americans (~93% and ~100% respectively, near-zero in Europeans/Africans) is associated with thicker hair, increased eccrine sweat gland density, shovel-shaped incisors, and smaller mammary glands; estimated to have been under selection for ~30,000 years (Kamberov et al., 2013, *Cell*)
- **Duffy/DARC** (FY*O allele): the Duffy-null allele, which eliminates the Duffy antigen receptor for chemokines on red blood cells, confers near-complete resistance to *Plasmodium vivax* malaria; it is at or near fixation in sub-Saharan Africa and virtually absent elsewhere, representing one of the most extreme Fst values in the human genome

### 1.3 Genome-Wide Selection Scans
- Voight et al. (2006, *PLoS Biology*): applied the integrated haplotype score (iHS) test across the genome, identifying ~300 candidate regions under recent positive selection in HapMap populations — enriched for genes involved in immunity, metabolism, skin/hair pigmentation, and sensory perception
- Sabeti et al. (2007, *Nature*): introduced the cross-population extended haplotype homozygosity (XP-EHH) test and identified strong signals at known adaptive loci plus many novel candidates, including genes in the Wnt signaling and innate immunity pathways

---

## 2. CREDIBLE CLAIMS (Tier 2 — Academic / Debated but Supported)

### 2.1 Soft Sweeps and Polygenic Adaptation
- Increasingly, researchers recognize that much human adaptation may have occurred through **soft sweeps** (selection on preexisting standing variation, leaving subtler genomic signatures) or **polygenic adaptation** (simultaneous small allele-frequency shifts at many loci, each below genome-wide significance — Pritchard et al., 2010, *Current Biology*)
- Polygenic adaptation is harder to detect than classic hard sweeps but may be the dominant mode of human adaptation for complex traits like height, body mass, and skin pigmentation
- Berg & Coop (2014, *PLoS Genetics*): developed methods to detect polygenic adaptation by testing whether genome-wide association study (GWAS) effect alleles show coordinated frequency shifts across populations; identified signals consistent with polygenic selection on height among European populations (though these results were later debated due to population structure confounds)

### 2.2 Distinguishing Selection from Demography
- Population bottlenecks, expansions, and admixture can mimic signatures of selection (e.g., creating extended haplotypes or skewed allele-frequency spectra)
- Modern approaches use demographic models fitted to genome-wide data to establish null expectations, then identify outlier loci exceeding neutral predictions — reducing (but not eliminating) false positives

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Possible but Unverified)

### 3.1 Ongoing Selection in Modern Humans
- Some available evidence suggests that natural selection continues to act in modern human populations (e.g., selection on variants associated with age at first reproduction, educational attainment, and cardiovascular risk factors in the UK Biobank and Icelandic populations — Mostafavi et al., 2017, *PLoS Biology*)
- Whether these signals represent genuine ongoing natural selection or methodological artifacts (ascertainment bias, population stratification) remains debated

---

## 4. DUBIOUS CLAIMS (Tier 4 — No Credible Source / Contradicted by Evidence)

### 4.1 Human Evolution Has Stopped
- **[DEBUNKED]** The popular claim that human evolution has "stopped" because modern medicine and technology have eliminated natural selection is incorrect; while the strength and direction of selection pressures have changed, genetic variation in survival and reproduction persists, and allele-frequency changes continue in all human populations

### Counter-Arguments
- The pace and mechanisms of human evolution have shifted (e.g., from dramatic hard sweeps to subtle polygenic adaptation and cultural niche construction), but evolutionary change has not ceased

---

## IMAGES

| # | Description | Filename | Source | License |
|---|-------------|----------|--------|---------|
*No images assigned yet.*

---

## BIBLIOGRAPHY

1. Maynard Smith, J. & Haigh, J. "The Hitch-Hiking Effect of a Favourable Gene." *Genetical Research* 23.1 (1974): 23–35. DOI: 10.1017/s0016672300014634
2. Voight, B.F. et al. "A Map of Recent Positive Selection in the Human Genome." *PLoS Biology* 4.3 (2006): e72. DOI: 10.1371/journal.pbio.0040072
3. Sabeti, P.C. et al. "Genome-Wide Detection and Characterization of Positive Selection in Human Populations." *Nature* 449 (2007): 913–918. DOI: 10.1038/nature06250.
4. Bersaglieri, T. et al. "Genetic Signatures of Strong Recent Positive Selection at the Lactase Gene." *American Journal of Human Genetics* 74.6 (2004): 1111–1120. DOI: 10.1086/421051
5. Lamason, R.L. et al. "SLC24A5, a Putative Cation Exchanger, Affects Pigmentation in Zebrafish and Humans." *Science* 310.5755 (2005): 1782–1786. DOI: 10.1126/science.1116238.
6. Kamberov, Y.G. et al. "Modeling Recent Human Evolution in Mice by Expression of a Selected EDAR Variant." *Cell* 152.4 (2013): 691–702.
7. Pritchard, J.K. et al. "The Genetics of Human Adaptation: Hard Sweeps, Soft Sweeps, and Polygenic Adaptation." *Current Biology* 20.4 (2010): R208–R215.
8. Berg, J.J. & Coop, G. "A Population Genetic Signal of Polygenic Adaptation." *PLoS Genetics* 10.8 (2014): e1004412.
9. Mostafavi, H. et al. "Identifying Genetic Variants That Affect Viability in Large Cohorts." *PLoS Biology* 15.9 (2017): e2002458.
10. Nielsen, R. et al. "Recent and Ongoing Selection in the Human Genome." *Nature Reviews Genetics* 8 (2007): 857–868.
11. Hermisson, J. & Pennings, P.S. "Soft Sweeps: Molecular Population Genetics of Adaptation from Standing Genetic Variation." *Genetics* 169.4 (2005): 2335–2352.
12. Fan, S. et al. "Going Global by Adapting Local: A Review of Recent Human Adaptation." *Science* 354.6308 (2016): 54–59.
13. Racimo, F. et al. "Evidence for Archaic Adaptive Introgression in Humans." *Nature Reviews Genetics* 16 (2015): 359–371.
14. Grossman, S.R. et al. "Identifying Recent Adaptations in Large-Scale Genomic Data." *Cell* 152.4 (2013): 703–713.

---

## CROSS-REFERENCE INDEX

| Related Doc | Connection |
|-------------|-----------|
| [L_3_03 — Lactase Persistence](../L3_Adaptation_Traits/L_3_03_Lactase_Persistence_Gene_Culture.md) | Classic sweep example |
| [L_1_05 — Skin Color Evolution](../L1_Human_Evolution_Species/L_1_05_Human_Skin_Color_Evolution.md) | SLC24A5 selection |
| [L_5_11 — Altitude Adaptation](../L5_Health_Microbiome_Applied/L_5_11_Altitude_Adaptation.md) | EPAS1 sweep |
| [L_2_02 — Population Genetics](../L2_Population_Regional_Genetics/L_2_02_Population_Genetics_Hardy_Weinberg.md) | Allele frequency theory |

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
