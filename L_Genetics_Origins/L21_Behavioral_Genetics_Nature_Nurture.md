# L21 — Behavioral Genetics: Nature and Nurture

> **Document ID:** L21
> **Section:** L_Genetics_Origins
> **Keywords:** behavioral genetics, nature nurture, twin study, heritability, adoption study, gene-environment interaction, gene-environment correlation, shared environment, non-shared environment, personality genetics, Big Five, psychiatric genetics, schizophrenia genetics, depression genetics, addiction genetics, MAOA, serotonin transporter, candidate gene, GWAS replication, epigenetics behavior, animal models, knockout mouse
> **Category Tags:** genetics, human-origins, psychology, ecology-environment
> **Cross-References:** [L20 — Intelligence Genetics](L20_Genetics_of_Intelligence_Cognition.md) · [L16 — Population Genetics](L16_Population_Genetics_Hardy_Weinberg.md) · ZC01 — IQ and Intelligence · K05 — Neural Correlates of Consciousness · [Z13 — Gene Expression Regulation](L28_Gene_Expression_Regulation.md)
> **Reliability Tier:** Tier 2 (established methods with evolving findings)
> **Last Updated:** Mar 7, 2026 | **Source Count:** 10 | **Weighted Score:** 24 | **Source Confidence:** [3/5] | **Confidence:** Moderate

---

## QUICK SUMMARY

Behavioral genetics — the scientific study of how genetic and environmental factors contribute to individual differences in behavior — has transformed our understanding of human psychology over the past half-century. Through twin studies, adoption studies, and increasingly GWAS, the field has established **three robust "laws"** (articulated by Eric Turkheimer, 2000): **(1) All human behavioral traits are heritable** (typical h² = 0.30–0.60); **(2) The effect of being raised in the same family (shared environment) is smaller than the effect of genes** (usually <0.10 for personality, somewhat larger for adolescent behaviors); **(3) A substantial portion of variance in complex behavioral traits is not accounted for by genes or shared environment** — non-shared environmental factors and their interactions with genes account for the remaining variance. The field has undergone a painful methodological reckoning since ~2010: hundreds of **candidate gene findings** (e.g., the serotonin transporter gene 5-HTTLPR × stress → depression interaction, Caspi et al., 2003; MAOA × childhood maltreatment → antisocial behavior) have largely **failed to replicate** in large GWAS-era samples, representing one of the most significant replication crises in science. Modern behavioral genetics is now firmly GWAS-based, revealing that virtually all behavioral traits are **massively polygenic** — influenced by thousands of variants of tiny effect, with no single "gene for" any normal-range behavioral trait. Psychiatric genetics has been most successful: **schizophrenia GWAS** (Trubetskoy et al., 2022, >300,000 cases) identified 287 loci; **major depression GWAS** (>1, million participants) identified >200 loci; **substance use disorders** are substantially heritable (40–60%) with emerging genetic architecture. The field demonstrates that the nature-versus-nurture dichotomy is false — genes and environments are inextricably intertwined through gene-environment interaction (G×E), gene-environment correlation (rGE), and epigenetic mechanisms.

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Established)

### 1.1 Turkheimer's Three Laws of Behavioral Genetics
- **First Law — Everything is heritable:** Meta-analysis of 2,748 twin studies encompassing ~14.5 million twin pairs (Polderman et al., 2015) found median heritability across all behavioral traits = 0.49; virtually no measured human behavioral trait shows zero heritability; personality (Big Five) h² ≈ 0.40–0.60; psychopathology h² ≈ 0.30–0.80; substance use h² ≈ 0.40–0.60; attitudes and values h² ≈ 0.30–0.50; even religiosity h² ≈ 0.30–0.45
- **Second Law — Shared environment smaller than genetic effects:** By adulthood, shared family environment (C) typically explains <10% of personality variance; C larger during childhood/adolescence but decreases with age; C somewhat larger for antisocial behavior in youth (~15%), substance use initiation (~20%), and religious attendance (~25%); shared environmental effects persistently important for some outcomes (educational attainment, delinquency in adolescence)
- **Third Law — Non-shared environment substantial:** Non-shared environment (E) includes unique experiences (different peer groups, differential parental treatment, stochastic developmental events, measurement error); typically accounts for 30–50% of variance; difficult to identify specific non-shared environmental factors — Plomin & Daniels (1987) "Why are children in the same family so different?" remains partially unanswered

### 1.2 Twin and Adoption Study Methods
- **Classical twin design:** Compare MZ (identical, 100% shared DNA) and DZ (fraternal, ~50% shared DNA) twin correlations; if MZ correlation > DZ correlation, genetic influence inferred; Falconer's formula: h² ≈ 2(rMZ - rDZ); assumptions: equal environments (MZ and DZ share environments equally — "equal environments assumption," EEA); violations of EEA studied extensively — modest effects on estimates but do not invalidate method
- **Adoption studies:** Separate genetic from environmental influences by studying adopted children (compare with biological vs. adoptive parents); Colorado Adoption Project, Texas Adoption Project, Swedish Adoption/Twin Study of Aging (SATSA); generally confirm twin study heritability estimates
- **Twins Reared Apart:** Minnesota Study of Twins Reared Apart (MISTRA, Bouchard et al., 1990) — studied MZ twins separated early in life; IQ correlation r ≈ 0.70–0.78; personality correlations ~0.50; remarkable behavioral similarities despite different rearing environments; criticized for self-selection biases and small samples but consistent with larger twin studies
- **SNP-based heritability (GCTA):** Estimates heritability using unrelated individuals from GWAS data; confirms substantial genetic contribution but typically lower than twin estimates (h²_SNP ≈ 50–70% of twin h²); the gap ("missing heritability") reflects rare variants, structural variants, gene-gene interactions, and inflated twin estimates from assortative mating and gene-environment correlation

### 1.3 The Candidate Gene Replication Crisis
- **Serotonin transporter (5-HTTLPR) × stress → depression:** Caspi et al. (2003, *Science*) reported that the short allele of the serotonin transporter promoter polymorphism interacted with stressful life events to predict depression; massively influential (>10,000 citations); meta-analyses reached conflicting conclusions; large pre-registered study (Border et al., 2019, N = 620,000) found NO association of 5-HTTLPR with depression, and NO G×E interaction; now considered non-replicated
- **MAOA × childhood maltreatment → antisocial behavior:** Caspi et al. (2002, *Science*); widely cited; some replications but inconsistent across studies; not confirmed in large GWAS; effect size, if real, much smaller than initially reported
- **Broader failure:** Systematic review (Duncan & Keller, 2011; Border et al., 2019) concluded that virtually all pre-GWAS candidate gene association findings for psychiatric and behavioral traits have failed to replicate in adequately powered samples; reasons: small sample sizes, publication bias, multiple testing without correction, population stratification, poor measurement; represents one of the most thorough replication failures in biomedicine
- **Lesson:** Individual common genetic variants have negligibly small effects on complex behavioral traits; only massive GWAS with proper multiple-testing correction can reliably detect them; has reshaped the field entirely

### 1.4 Psychiatric Genetics (GWAS Era)
- **Schizophrenia:** Most genetically tractable psychiatric disorder; h² ≈ 0.79 (twin studies); Trubetskoy et al. (2022, PGC3) GWAS of 76,755 cases + 243,649 controls → 287 loci; enrichment in synaptic genes, voltage-gated ion channels, glutamate signaling; notable hit: *C4* complement gene (structural alleles affecting C4A expression → synaptic pruning — Sekar et al., 2016); polygenic score explains ~7% of variance on liability scale
- **Major depression:** h² ≈ 0.37 (twin studies, lower than schizophrenia); Howard et al. (2019, >1.2 million participants) → 102 loci; expanded in subsequent studies to >200 loci; enrichment in prefrontal brain regions, neuronal development
- **Bipolar disorder:** h² ≈ 0.60–0.85; Mullins et al. (2021) → 64 loci; significant genetic overlap with schizophrenia (r_g ≈ 0.68) and depression (r_g ≈ 0.44)
- **Autism spectrum:** h² ≈ 0.65–0.90; substantial rare variant contribution (de novo CNVs, de novo coding mutations — in addition to common variant architecture); >100 GWAS loci; genetically heterogeneous
- **Cross-disorder genetics:** Psychiatric disorders share substantial genetic liability; genetic correlations positive for most pairs (schizophrenia-bipolar r_g ≈ 0.68; depression-anxiety r_g ≈ 0.80; ADHD-depression r_g ≈ 0.40); suggests shared biological pathways and questions categorical diagnostic boundaries

---

## 2. CREDIBLE CLAIMS (Tier 2 — Strong Evidence, Active Research)

### 2.1 Gene-Environment Interplay
- **Gene-environment interaction (G×E):** Genetic effects depend on environmental context (and vice versa); established for some traits: *FKBP5* genotype moderates cortisol stress response; *ApoE4* × head injury → Alzheimer's risk; *ALDH2* × alcohol exposure → cancer risk; G×E for psychiatric outcomes remains difficult to detect reliably at individual genetic variant level; polygenic × environment interactions more plausible but even harder to study statistically
- **Gene-environment correlation (rGE):** Passive rGE (parents provide both genes and environments), evocative rGE (child's genetically influenced behavior evokes environmental responses), active rGE (individuals seek environments matching their genotypes); rGE explains why "environmental" measures are partially heritable — SES, marital status, peer group, TV watching, even stressful life events show genetic influence (h² ≈ 0.20–0.40)
- **"Nature of nurture":** Plomin & Bergeman (1991); supposed environmental measures are substantially genetically mediated; implications: correlations between "environment" and outcomes may partly reflect shared genetic influences → genetic confounding in observational studies

### 2.2 Personality Genetics
- **Big Five personality traits (Openness, Conscientiousness, Extraversion, Agreeableness, Neuroticism):** Each moderately heritable (h² ≈ 0.40–0.60); GWAS (de Moor et al., 2012; Lo et al., 2017; up to N > 600,000) identified genome-wide significant loci for each trait but effect sizes extremely small; polygenic scores explain <5% of variance; neuroticism best powered — >170 loci (Nagel et al., 2018)
- **Genetic stability:** Same genetic factors influence personality across the lifespan; mean-level change (maturity: increasing conscientiousness, decreasing neuroticism) largely environmentally driven; rank-order stability increasingly genetic

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Emerging / Theoretical)

### 3.1 Epigenetics and Behavioral Inheritance
- Stress, early adversity, and environmental exposures can modify epigenetic marks (DNA methylation, histone modifications) in brain and peripheral tissues; animal models: maternal behavior (licking/grooming in rats) affects offspring stress response via epigenetic modification of glucocorticoid receptor (*NR3C1*) promoter (Weaver et al., 2004); human studies: childhood adversity associated with altered DNA methylation at *NR3C1*, *FKBP5*, *SLC6A4* in blood/brain tissue
- **Transgenerational behavioral epigenetics:** Claims that behavioral effects transmit across multiple generations via epigenetic mechanisms (beyond direct exposure); animal evidence exists (mice — Dias & Ressler, 2014, olfactory fear conditioning); human evidence very limited and contested; mechanisms for stable multigenerational behavioral epigenetic transmission remain unclear; field active but replication challenging

### 3.2 Gene Editing for Psychiatric Conditions
- With psychiatric genetics identifying biological pathways (synaptic pruning in schizophrenia, glutamate signaling, serotonin metabolism), future gene-based therapies theoretically possible for severe Mendelian psychiatric conditions (e.g., Rett syndrome — *MECP2*); for common polygenic conditions, genetic architecture (thousands of tiny-effect variants) makes gene editing impractical; pharmacogenomics (matching psychiatric medications to genotype) more realistic near-term application

---

## 4. DUBIOUS CLAIMS (Tier 4 — Fringe / Unsubstantiated)

### 4.1 The "Warrior Gene" [OVERSIMPLIFIED]
- Media portrayal of low-activity MAOA allele as a "warrior gene" predisposing carriers to violence; original finding (Caspi et al., 2002) was an interaction effect (MAOA × maltreatment), not a main effect; subsequent replications inconsistent; effect if present is very small; used inappropriately in legal defense cases; ignores that violence is a complex outcome influenced by thousands of genetic and environmental factors; popularized narrative grossly misrepresents the biology

### 4.2 Single Genes Determine Specific Behaviors [UNFOUNDED]
- No reliable evidence for "a gene for" risk-taking, homosexuality, criminality, political orientation, or other complex behaviors operating through a single major locus; all behavioral traits are massively polygenic (thousands of variants); candidate gene era repeatedly failed to identify reliable single-gene associations; deterministic genetic narratives for complex behavior are scientifically unsupported

---

## IMAGES

| # | Description | Source |
|---|-------------|--------|
| 1 | Twin study design (MZ vs. DZ comparison) | Standard behavioral genetics texts |
| 2 | Heritability estimates across behavioral traits | Polderman et al. (2015) |
| 3 | Candidate gene failure: 5-HTTLPR replication | Border et al. (2019) |
| 4 | Psychiatric cross-disorder genetic correlation matrix | PGC Cross-Disorder Group |

---

## BIBLIOGRAPHY

1. Polderman, T. J. C. et al. (2015). "Meta-Analysis of the Heritability of Human Traits Based on Fifty Years of Twin Studies." *Nature Genetics*, 47, 702–709.
2. Turkheimer, E. (2000). "Three Laws of Behavior Genetics and What They Mean." *Current Directions in Psychological Science*, 9(5), 160–164.
3. Border, R. et al. (2019). "No Support for Historical Candidate Gene or Candidate Gene-by-Interaction Hypotheses for Major Depression Across Multiple Large Samples." *American Journal of Psychiatry*, 176(5), 376–387.
4. Caspi, A. et al. (2003). "Influence of Life Stress on Depression: Moderation by a Polymorphism in the 5-HTT Gene." *Science*, 301, 386–389.
5. Trubetskoy, V. et al. (2022). "Mapping Genomic Loci Implicates Genes and Synaptic Biology in Schizophrenia." *Nature*, 604, 502–508.
6. Bouchard, T. J. et al. (1990). "Sources of Human Psychological Differences: The Minnesota Study of Twins Reared Apart." *Science*, 250, 223–228.
7. Plomin, R. et al. (2013). *Behavioral Genetics*. 6th ed. Worth Publishers.
8. Nagel, M. et al. (2018). "Meta-Analysis of Genome-Wide Association Studies for Neuroticism in 449,484 Individuals." *Nature Genetics*, 50, 920–927.
9. Weaver, I. C. G. et al. (2004). "Epigenetic Programming by Maternal Behavior." *Nature Neuroscience*, 7, 847–854.
10. Kendler, K. S. et al. (2011). "The Structure of Genetic and Environmental Risk Factors for DSM-IV Personality Disorders: A Multivariate Twin Study." *Archives of General Psychiatry*, 68(1), 29–36.

---

## CROSS-REFERENCE INDEX

- **[L20 — Intelligence Genetics](L20_Genetics_of_Intelligence_Cognition.md):** Cognitive ability as the most studied behavioral genetic trait
- **[L16 — Population Genetics](L16_Population_Genetics_Hardy_Weinberg.md):** Allele frequency dynamics underlying behavioral variation
- **ZC01 — IQ and Intelligence:** Psychological measurement of heritable traits
- **K05 — Neural Correlates of Consciousness:** Brain basis of behavior
- **[Z13 — Gene Expression Regulation](L28_Gene_Expression_Regulation.md):** Epigenetic mechanisms modulating behavioral gene expression
- **[Z07 — Epigenetic Inheritance](L21_Epigenetic_Inheritance_Transgenerational.md):** Transgenerational behavioral epigenetics

---

*Last verified: Mar 07, 2026 — All sources peer-reviewed or from established behavioral genetics literature*
