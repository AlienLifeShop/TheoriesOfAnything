# G_4_14 — Replication Crisis and What It Means for Ancient Claims

> **Source Count:** 13 | **Weighted Score:** 37 | **Source Confidence:** [4/5] | **Primary Tier:** 1–2 | **Last Updated:** March 10, 2026
> **Keywords:** replication crisis, reproducibility, p-hacking, HARKing, publication bias, open science, pre-registration, Ioannidis, Open Science Collaboration, file drawer problem, effect size, statistical significance, meta-analysis, questionable research practices, underpowered studies, scientific fraud
> **Category Tags:** modern-frameworks, methodology, statistics, science policy, epistemology
> **Cross-References:** [H_2_04 — Academic Suppression](../../H_Suppression_and_Thesis/H2_Institutional_Academic_Suppression/H_2_04_Scientific_Censorship_Paradigm_Defense.md) · [H_2_03 — Peer Review Problems](../../H_Suppression_and_Thesis/H2_Institutional_Academic_Suppression/H_2_03_Academic_Gatekeeping_Paradigm_Resistance.md) · [T_1_01 — Psychology Overview](../../T_Psychology_Social/T1_Foundations_Theories/T_1_01_Jungian_Archetypes_Collective_Unconscious.md) · [G_2_03 — Bayesian Reasoning](../G2_Analytical_Computational/G_2_03_Bayesian_Reasoning_Archaeological_Inference.md)

---

## QUICK SUMMARY

The **replication crisis** refers to the discovery, beginning in the early 2010s, that a substantial proportion of findings published in peer-reviewed scientific journals — particularly in psychology, social science, and biomedical research — fail to replicate when independent researchers attempt to reproduce them using the original methods. The landmark study was the **Open Science Collaboration** (OSC, 2015, *Science*), which attempted to replicate 100 psychology studies published in three top journals: only **36%** produced statistically significant results in the same direction as the original, and the average effect size of replications was roughly **half** the original. This crisis was anticipated by **John Ioannidis**'s influential paper "Why Most Published Research Findings Are False" (2005, *PLOS Medicine*), which used Bayesian reasoning to show that in fields with low prior probability of true effects, small sample sizes, flexible statistical analysis, and strong publication bias, the majority of statistically significant results will be false positives. The structural causes are now well-documented: **(1) p-hacking** — researchers (often unconsciously) test multiple analyses, variables, or subgroups until they find p < 0.05, inflating the false positive rate far beyond the nominal 5%; **(2) HARKing** (Hypothesizing After Results are Known) — presenting post-hoc discoveries as if they were a priori predictions; **(3) publication bias** — journals preferentially publish "positive" (statistically significant) results, creating a "file drawer" of unreported null results; **(4) underpowered studies** — small sample sizes that can only detect large effects, meaning that any significant result is likely an overestimate (the "winner's curse"). For **ancient claims and alternative history**, the replication crisis has profound implications: many archaeological and historical claims rest on studies from fields now known to have replication problems (e.g., priming effects, social psychology experiments used to explain ancient behavior, small-sample genetic studies). More broadly, the crisis provides a framework for understanding why extraordinary claims based on a single study — no matter how high-profile the journal — should be treated with caution. The response to the crisis has been the **open science movement**: pre-registration of hypotheses and analysis plans before data collection, mandatory data sharing, registered reports (peer review before results are known), and a shift from null-hypothesis significance testing (NHST) toward estimation-based approaches (effect sizes with confidence intervals) and Bayesian methods. These reforms are gradually being adopted in archaeology and ancient studies, but the field still relies heavily on small-sample, unreplicated findings.

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Scholarly Consensus)

### 1.1 Scope of the Replication Crisis
- **Open Science Collaboration (2015)**: attempted replications of 100 psychology studies — 97% of originals had p < 0.05; only 36% of replications achieved p < 0.05 in the same direction; mean effect size in replications was ~50% of original
- **Camerer et al. (2018, *Nature Human Behaviour*)**: replicated 21 social science experiments published in *Nature* and *Science* (2010–2015) — 62% replicated (13/21), but effect sizes were on average 50% smaller than originally reported
- **Errington et al. (2021, *eLife*)**: the Reproducibility Project: Cancer Biology attempted to replicate 193 experiments from 53 high-impact cancer biology papers — only 50% of replications produced results consistent with the original in effect size and direction
- **Begley & Ellis (2012, *Nature*)**: scientists at Amgen attempted to replicate 53 "landmark" preclinical cancer studies — only 6 (11%) could be confirmed

### 1.2 Structural Causes — P-hacking and Publication Bias
- **P-hacking** (Simmons, Nelson, & Simonsohn, 2011): researchers exploit "researcher degrees of freedom" — decisions about which variables to include, when to stop collecting data, which outliers to exclude, how to split continuous variables — to obtain p < 0.05; simulations show that even a few such decisions can inflate the false positive rate from 5% to >50%
- **Publication bias**: Fanelli (2010, *PLOS ONE*) found that the proportion of papers reporting "positive" results increased from ~70% in 1990 to ~86% in 2007 — a pattern inconsistent with a stable base rate of true discoveries; Franco et al. (2014) traced NSF-funded studies and found that 60% of null results were never written up ("file drawer problem")
- **Underpowered studies**: Button et al. (2013, *Nature Reviews Neuroscience*) estimated that the median statistical power in neuroscience is ~21% — meaning most studies have an 80% chance of missing a true effect, and any "significant" finding from such a study is likely inflated ("winner's curse")

### 1.3 Ioannidis's Bayesian Argument
- Ioannidis (2005) formalized why most published findings are likely false using a Bayesian framework:
  - With a prior probability of 10% that a hypothesis is true, a false positive rate of 5%, and 80% power → Positive Predictive Value (PPV) ≈ 64% (i.e., 36% of significant results are false positives)
  - With lower priors (exploratory research, ~1% true hypotheses), PPV drops below 20% — most significant results are false positives
  - Add p-hacking, selective reporting, and publication bias → PPV drops further, potentially below 50% even for "well-powered" studies
- This framework explains why fields with low prior probabilities and high analytical flexibility (social psychology, nutritional epidemiology, candidate gene studies) have been most affected by the crisis

---

## 2. CREDIBLE CLAIMS (Tier 2 — Academic / Debated but Supported)

### 2.1 Implications for Archaeology and Ancient Studies
- Many archaeological interpretations rely on small-sample studies, limited replication opportunities (unique sites, unrepeatable excavations), and researcher degrees of freedom in interpreting material evidence
- Palmer (2020) and others have argued that archaeology is partially insulated from the replication crisis because its empirical basis is material (artifacts, stratigraphy) rather than statistical tests of human behavior — but that subfields relying on statistical methods (aDNA studies, stable isotope analysis, agent-based models) are fully susceptible to the same problems
- The field of **archaeogenetics** has experienced its own replication concerns: early candidate-gene studies of population origins (often based on small samples and mtDNA haplogroup frequencies) have been superseded or contradicted by whole-genome studies — a pattern analogous to the "candidate gene" crisis in behavioral genetics

### 2.2 Open Science Reforms
- **Pre-registration**: uploading hypotheses, methods, and analysis plans to public registries (e.g., OSF, AsPredicted) before data collection — prevents HARKing and constrains p-hacking
- **Registered Reports**: journals peer-review the introduction and methods sections *before* results are known, and commit to publishing regardless of outcome — eliminating publication bias by design; >300 journals now offer this format
- **Data and code sharing**: mandated by an increasing number of journals and funders (NIH, Wellcome Trust), enabling computational reproducibility — though compliance remains uneven

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Possible but Unverified)

### 3.1 Has the Crisis Undermined Public Trust in Science?
- Some commentators worry that awareness of the replication crisis has reduced public trust in science — providing ammunition for science deniers and conspiracy theorists who argue that "science can't be trusted"
- Survey data are mixed: Pew Research (2020) showed that public trust in science remained relatively stable during 2016–2020, though trust in specific institutions (CDC, FDA) fluctuated more; in practice, most public distrust appears driven by political polarization rather than awareness of methodological problems
- For alternative history, the risk is that the replication crisis is selectively cited to dismiss mainstream findings while uncritically accepting unreplicated fringe claims — a double standard

---

## 4. DUBIOUS CLAIMS (Tier 4 — No Credible Source / Contradicted by Evidence)

### 4.1 The Replication Crisis Proves Mainstream Science Is a Conspiracy
- **[MISAPPLICATION]** The replication crisis demonstrates systemic methodological weaknesses and perverse incentive structures — not deliberate fraud or coordinated suppression; the crisis was identified, documented, and addressed by the scientific community itself, which is evidence of science's self-correcting capacity, not its failure

---

## Counter-Arguments & Criticisms

No significant counter-arguments exist in the scholarly literature for the core claims in this document. Replication Crisis and What It Means for Ancient Claims represents established scientific and methodological consensus with no active scholarly dispute over the fundamental claims presented here.

---

## IMAGES

| # | Description | Filename | Source | License |
|---|-------------|----------|--------|---------|
*No images assigned yet.*

---

## BIBLIOGRAPHY

1. Open Science Collaboration. "Estimating the Reproducibility of Psychological Science." *Science* 349 (2015): aac4716. DOI: 10.1126/science.aac4716.
2. Ioannidis, J.P.A. "Why Most Published Research Findings Are False." *PLOS Medicine* 2 (2005): e124. DOI: 10.1371/journal.pmed.0020124
3. Simmons, J.P. et al. "False-Positive Psychology: Undisclosed Flexibility in Data Collection and Analysis Allows Presenting Anything as Significant." *Psychological Science* 22 (2011): 1359–1366. DOI: 10.1177/0956797611417632
4. Camerer, C.F. et al. "Evaluating the Replicability of Social Science Experiments in Nature and Science between 2010 and 2015." *Nature Human Behaviour* 2 (2018): 637–644. DOI: 10.1038/s41562-018-0399-z.
5. Begley, C.G. & Ellis, L.M. "Raise Standards for Preclinical Cancer Research." *Nature* 483 (2012): 531–533. DOI: 10.1038/483531a.
6. Button, K.S. et al. "Power Failure: Why Small Sample Size Undermines the Reliability of Neuroscience." *Nature Reviews Neuroscience* 14 (2013): 365–376. DOI: 10.1038/nrn3475
7. Fanelli, D. "'Positive' Results Increase Down the Hierarchy of the Sciences." *PLOS ONE* 5 (2010): e10068. DOI: 10.1371/journal.pone.0010068
8. Franco, A. et al. "Publication Bias in the Social Sciences: Unlocking the File Drawer." *Science* 345 (2014): 1502–1505. DOI: 10.1126/science.1255484.
9. Nosek, B.A. et al. "The Preregistration Revolution." *PNAS* 115 (2018): 2600–2606. DOI: 10.1073/pnas.1708274114
10. Errington, T.M. et al. "Investigating the Replicability of Preclinical Cancer Biology." *eLife* 10 (2021): e71601. DOI: 10.7554/eLife.71601.
11. Munafò, M.R. et al. "A Manifesto for Reproducible Science." *Nature Human Behaviour* 1 (2017): 0021. DOI: 10.1038/s41562-016-0021.
12. Kerr, N.L. "HARKing: Hypothesizing After the Results are Known." *Personality and Social Psychology Review* 2 (1998): 196–217. DOI: 10.1207/s15327957pspr0203_4
13. Chambers, C.D. *The Seven Deadly Sins of Psychology: A Manifesto for Reforming the Culture of Scientific Practice.* Princeton: Princeton University Press, 2017.


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
