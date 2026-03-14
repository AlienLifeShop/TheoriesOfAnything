# V_3_12 — Statistics and Hypothesis Testing

> **Document ID:** V_3_12
> **Section:** V_Mathematics_Information
> **Keywords:** statistics, hypothesis testing, p-value, significance, confidence interval, null hypothesis, Type I error, Type II error, power, Fisher, Neyman, Pearson, t-test, ANOVA, chi-squared, regression, effect size, meta-analysis, Bayesian statistics, frequentist, replication crisis, multiple testing, Bonferroni
> **Category Tags:** mathematics, information
> **Cross-References:** [V_3_07 — Probability Theory](V_3_07_Probability_Theory_Randomness_Bayes.md) · [V_3_11 — Mathematical Optimization](V_3_11_Mathematical_Optimization.md) · [ZC_1_01 — Psychology Overview](../../ZC_Social_Science/ZC1_Psychology_Behavior/ZC_1_01_Social_Psychology_Conformity_Obedience.md) · [R_3_09 — Molecular Phylogenetics](../../R_Biology_Evolution/R3_Mechanisms_Genetics/R_3_09_Molecular_Phylogenetics_Tree_of_Life.md) · [ZA_3_07 — Particle Accelerators](../../ZA_Physics_Quantum/ZA3_Particle_Nuclear_Physics/ZA_3_07_Particle_Accelerators_Colliders.md)
> **Reliability Tier:** Tier 1 (well-documented, peer-reviewed)
> **Last Updated:** Mar 07, 2026 | **Source Count:** 10 | **Weighted Score:** 22 | **Source Confidence:** [3/5] | **Confidence:** High (well-documented, peer-reviewed)

---

## QUICK SUMMARY

Statistics — the science of collecting, analyzing, and interpreting data under uncertainty — underpins virtually every empirical science, from medicine and psychology to physics and economics. Modern statistical hypothesis testing grew from two competing frameworks: R. A. Fisher's significance testing (1925), which introduced $p$-values as measures of evidence against a null hypothesis, and the Neyman-Pearson framework (1933), which formalized hypothesis testing as a decision procedure between null ($H_0$) and alternative ($H_1$) hypotheses with controlled error rates (Type I: false positive, $\alpha$; Type II: false negative, $\beta$; power: $1-\beta$). The $p < 0.05$ threshold, though widely used, is arbitrary — Fisher intended $p$-values as continuous measures of evidence, not rigid pass/fail criteria. The replication crisis (2010s) revealed that many published findings with $p < 0.05$ fail to replicate, driven by $p$-hacking, publication bias, underpowered studies, and misunderstanding of what $p$-values actually mean ($p$ is NOT the probability that $H_0$ is true). The American Statistical Association's 2019 statement declared that "$p$-values should not be used as the primary basis for scientific conclusions" and urged moving beyond "statistical significance." Modern best practices emphasize effect sizes, confidence intervals, pre-registration, Bayesian methods, and meta-analysis. Bayesian statistics, which directly computes the probability of hypotheses given data via Bayes' theorem, offers a philosophically coherent alternative but introduces prior specification as a subjective element.

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Established Statistics)

### 1.1 Hypothesis Testing Frameworks
- **[KEY FINDING]** A $p$-value is the probability of observing data as extreme as or more extreme than the observed data, assuming $H_0$ is true — it is NOT the probability that $H_0$ is true, NOT the probability the result occurred by chance, and NOT the probability of making an error; these misinterpretations are pervasive even among scientists (Greenland et al., 2016); correct interpretation requires understanding the sampling distribution under $H_0$
- **Fisher significance testing (1925):** $p$-values as continuous measures of evidence against $H_0$ — small $p$-values suggest the data are unlikely under $H_0$; Fisher considered $p = 0.05$ a "convenient level" but not a rigid cutoff; he recommended integrating $p$-values with prior knowledge and replication
- **Neyman-Pearson framework (1933):** Hypothesis testing as a decision between $H_0$ and $H_1$ — pre-specify $\alpha$ (acceptable Type I error rate, typically 0.05); design study with adequate power ($1-\beta$, typically 0.80); reject $H_0$ if test statistic falls in the rejection region; power depends on effect size, sample size, and $\alpha$; Cohen (1988) provided power analysis guidelines
- **Standard tests:** Student's $t$-test (means of one or two groups; Gosset, 1908); ANOVA (comparing >2 group means; Fisher, 1925); chi-squared test (categorical data; Pearson, 1900); F-test (variance ratios); Mann-Whitney $U$ (nonparametric rank test); Kruskal-Wallis (nonparametric ANOVA); each has assumptions (normality, independence, homoscedasticity) that must be checked

### 1.2 Estimation and Confidence Intervals
- **Point estimation:** Sample statistics (mean $\bar{x}$, variance $s^2$, proportion $\hat{p}$) estimate population parameters — properties of good estimators: unbiasedness (expected value equals parameter), consistency (converges to parameter as $n \to \infty$), efficiency (minimum variance); maximum likelihood estimation (MLE, Fisher, 1922) provides a general framework
- **Confidence intervals:** A 95% CI means: if we repeated the experiment many times, 95% of the constructed intervals would contain the true parameter — NOT that there is a 95% probability the parameter lies in this specific interval (frequentist interpretation; the parameter is fixed); CIs convey both point estimate and precision; increasingly recommended over $p$-values alone
- **Effect sizes:** Standardized measures of the magnitude of an effect — Cohen's $d$ (standardized mean difference: 0.2 small, 0.5 medium, 0.8 large), $r$ (correlation coefficient), $\eta^2$ (proportion of variance explained in ANOVA), odds ratio (OR, for binary outcomes); effect sizes are essential because statistical significance depends on sample size ($n$ large enough makes any tiny effect "significant")

### 1.3 Regression and Modeling
- **Linear regression:** $y = \beta_0 + \beta_1 x + \varepsilon$ — least squares estimation minimizes $\sum (y_i - \hat{y}_i)^2$; Gauss (1809) and Legendre (1805); Gauss-Markov theorem: OLS estimators are BLUE (best linear unbiased estimators) under standard assumptions; multiple regression extends to $p$ predictors: $y = X\beta + \varepsilon$
- **Generalized linear models (GLMs):** Extend linear regression to non-normal distributions — logistic regression (binary outcomes, logit link), Poisson regression (count data, log link), gamma regression (positive continuous); McCullagh and Nelder (1989); estimated via maximum likelihood; the backbone of applied statistics
- **Model selection:** AIC (Akaike Information Criterion, 1973): $AIC = 2k - 2\ln(\hat{L})$ — penalizes model complexity; BIC (Bayesian Information Criterion, Schwarz, 1978): $BIC = k\ln(n) - 2\ln(\hat{L})$ — stronger complexity penalty; cross-validation for prediction accuracy; regularization (LASSO, ridge) for high-dimensional models

### 1.4 Multiple Testing and Modern Corrections
- **Multiple testing problem:** Testing $m$ hypotheses at $\alpha = 0.05$ yields expected $0.05m$ false positives by chance — Bonferroni correction: use $\alpha/m$ per test (controls family-wise error rate, conservative); Holm's step-down procedure (less conservative); Benjamini-Hochberg (1995) controls false discovery rate (FDR): proportion of rejections that are false positives; FDR is standard in genomics where thousands of simultaneous tests are routine
- **$5\sigma$ standard in physics:** Particle physics requires $p < 2.87 \times 10^{-7}$ ($5\sigma$) to claim discovery — the Higgs boson was announced at $5\sigma$ in 2012; this severe threshold accounts for the look-elsewhere effect (searching many channels simultaneously) and the extraordinary nature of the claim

---

## 2. CREDIBLE CLAIMS (Tier 2 — Academic / Debated but Supported)

### 2.1 Replication Crisis
- **Reproducibility Project: Psychology (2015):** Open Science Collaboration attempted to replicate 100 published psychology results — only 36–47% replicated successfully; average effect sizes were half the originals; "replication crisis" galvanized reform across sciences
- **Causes:** $p$-hacking (trying many analyses until $p < 0.05$, also called "researcher degrees of freedom," Simmons et al., 2011); publication bias (journals preferentially publish positive results); HARKing (Hypothesizing After Results are Known); underpowered studies (median power ~50% in psychology, Szucs and Ioannidis, 2017); "Ioannidis (2005): Most Published Research Findings Are False" — landmark paper arguing that when studies are low-powered, the expected proportion of true positives among significant results is alarmingly low
- **Reforms:** Pre-registration (specifying hypotheses and analysis before data collection); Registered Reports (peer review before data collection); open data and open code; larger sample sizes; replications valued rather than penalized; ASA 2019 statement: "Don't say 'statistically significant'" — recommends reporting $p$-values alongside effect sizes, confidence intervals, and contextual interpretation

### 2.2 Bayesian Statistics
- **Bayes' theorem applied to hypotheses:** $P(H|D) = \frac{P(D|H)P(H)}{P(D)}$ — directly computes the probability of a hypothesis given data; Bayes factors $BF_{10} = P(D|H_1)/P(D|H_0)$ quantify evidence for $H_1$ vs. $H_0$; Jeffreys' scale: $BF > 10$ strong evidence, $BF > 100$ decisive; avoids many problems of $p$-values
- **MCMC methods:** Markov chain Monte Carlo (Metropolis et al., 1953; Geman and Geman, 1984; Hastings, 1970) makes Bayesian inference computationally feasible — BUGS, JAGS, Stan software; hierarchical models, mixture models, and complex likelihoods are naturally handled; Bayesian methods dominate in astrophysics, epidemiology, and machine learning
- **Prior specification debate:** Bayesian analysis requires choosing priors — uninformative/flat priors, Jeffreys priors, weakly informative priors (Gelman et al.); sensitivity analysis assesses how conclusions change with different priors; critics argue priors introduce subjectivity; proponents argue all statistical analyses involve subjective choices (model selection, test choice) and Bayesian methods make these explicit

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Possible but Unverified)

### 3.1 Future of Statistical Methodology
- **Post-p-value statistics:** Whether the scientific community will successfully transition away from the $p < 0.05$ paradigm — some advocate replacing threshold-based testing with estimation-based approaches (effect sizes, CIs), calibrated $p$-values (Benjamin et al., 2018: redefine significance as $p < 0.005$), or Bayesian methods; cultural change is slow
- **Causal inference revolution:** Pearl's do-calculus and structural causal models formalize causation beyond correlation — DAGs (directed acyclic graphs), potential outcomes framework (Rubin), and instrumental variables enable causal conclusions from observational data under stated assumptions; "the ladder of causation" (Pearl and Mackenzie, 2018); transforming epidemiology, economics, and social science

---

## 4. DUBIOUS CLAIMS (Tier 4 — No Credible Source / Contradicted by Evidence)

### 4.1 "$p < 0.05$ Proves the Hypothesis Is True"
- **[FALSE]** A $p$-value below 0.05 does not prove $H_1$ is true or that $H_0$ is false — $p$-values are computed under $H_0$; they cannot tell you the probability that a hypothesis is true without additional information (prior probability, via Bayes' theorem); this misunderstanding is the most common statistical error in published science

---

## IMAGES

| # | Description | Filename | Source | License |
|---|-------------|----------|--------|---------|
| 1 | Diagram comparing frequentist and Bayesian approaches to hypothesis testing | — | — | — |

---

## Counter-Arguments & Criticisms

No significant counter-arguments exist in the scholarly literature for the core claims presented here. The topic of Statistics Hypothesis Testing represents established knowledge within mathematics and information theory with no active scholarly dispute over the fundamental claims presented in this document.

## BIBLIOGRAPHY

1. Fisher, R. A. *Statistical Methods for Research Workers*. Oliver and Boyd, 1925.
2. Neyman, J. and Pearson, E. S. "On the Problem of the Most Efficient Tests of Statistical Hypotheses." *Philosophical Transactions of the Royal Society A*, vol. 231, 1933, pp. 289–337. DOI: 10.1098/rsta.1933.0009.
3. Greenland, S. et al. "Statistical Tests, P Values, Confidence Intervals, and Power: A Guide to Misinterpretations." *European Journal of Epidemiology*, vol. 31, 2016, pp. 337–350. DOI: 10.1007/s10654-016-0149-3
4. Ioannidis, J. P. A. "Why Most Published Research Findings Are False." *PLoS Medicine*, vol. 2, 2005, e124. DOI: 10.1371/journal.pmed.0020124
5. Open Science Collaboration. "Estimating the Reproducibility of Psychological Science." *Science*, vol. 349, 2015, aac4716. DOI: 10.1126/science.aac4716.
6. Benjamini, Y. and Hochberg, Y. "Controlling the False Discovery Rate: A Practical and Powerful Approach to Multiple Testing." *Journal of the Royal Statistical Society B*, vol. 57, 1995, pp. 289–300. DOI: 10.1111/j.2517-6161.1995.tb02031.x
7. Wasserstein, R. L. et al. "Moving to a World Beyond 'p < 0.05'." *American Statistician*, vol. 73, sup. 1, 2019, pp. 1–19.
8. Gelman, A. et al. *Bayesian Data Analysis*. CRC Press, 3rd edition, 2013.
9. Cohen, J. *Statistical Power Analysis for the Behavioral Sciences*. Lawrence Erlbaum, 2nd edition, 1988.
10. Pearl, J. and Mackenzie, D. *The Book of Why: The New Science of Cause and Effect*. Basic Books, 2018.

---

## CROSS-REFERENCE INDEX

| Related Doc | Connection |
|-------------|-----------|
| [V_3_07 — Probability Theory](V_3_07_Probability_Theory_Randomness_Bayes.md) | Probability theory provides the mathematical foundation for all statistical inference |
| [V_3_11 — Mathematical Optimization](V_3_11_Mathematical_Optimization.md) | MLE and model fitting are optimization problems; regularization connects to shrinkage estimation |
| [ZC_1_01 — Psychology Overview](../../ZC_Social_Science/ZC1_Psychology_Behavior/ZC_1_01_Social_Psychology_Conformity_Obedience.md) | The replication crisis has had its most visible impact in psychology; reforms reshaping the field |
| [R_3_09 — Molecular Phylogenetics](../../R_Biology_Evolution/R3_Mechanisms_Genetics/R_3_09_Molecular_Phylogenetics_Tree_of_Life.md) | Bayesian phylogenetics uses MCMC and posterior probabilities for tree inference |
| [ZA_3_07 — Particle Accelerators](../../ZA_Physics_Quantum/ZA3_Particle_Nuclear_Physics/ZA_3_07_Particle_Accelerators_Colliders.md) | The 5-sigma discovery threshold in particle physics is the most stringent significance standard in science |

---

*New research document — Phase 9 expansion. Last Updated: Mar 07, 2026*

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
