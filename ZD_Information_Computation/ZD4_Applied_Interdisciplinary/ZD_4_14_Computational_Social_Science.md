# ZD_4_14 — Computational Social Science: Agent-Based Modeling, Digital Trace Data, and Social Simulation

> **Source Count:** 21 | **Weighted Score:** 52 | **Source Confidence:** [5/5] | **Primary Tier:** 1 | **Last Updated:** March 11, 2026
> **Keywords:** computational social science, agent-based modeling, social simulation, digital trace data, computational text analysis, big data, social networks, NLP, ABM, complex systems
> **Category Tags:** information-computation, social-science, data-science, complex-systems, methodology
> **Cross-References:** [ZC_5_11 — Digital Sociology](../../ZC_Social_Science/ZC5_Modern_Applied_Social_Science/ZC_5_11_Digital_Sociology.md) · [ZD_4_13 — Network Science](ZD_4_13_Network_Science.md) · [ZD_1_02 — Mathematics Information](../ZD1_Foundations_Theory/ZD_1_02_Information_Theory.md)

---

## QUICK SUMMARY

**Computational social science** (CSS) is the interdisciplinary field that applies computational methods — agent-based modeling, social network analysis, natural language processing, machine learning, simulation, and large-scale data analysis — to study social phenomena: human behavior, social structures, cultural dynamics, political processes, economic interactions, and collective action. CSS emerged as a distinct field in the late 2000s (Lazer et al., *Science*, 2009 — the landmark manifesto "Computational Social Science" signed by 15 leading researchers from computer science, political science, sociology, and economics) as the convergence of three developments: (1) **Unprecedented digital data** — social media platforms, mobile phones, web searches, financial transactions, government records, and sensor networks generate continuous, granular, large-scale data about human behavior ("digital trace data") at a scale impossible through traditional surveys, interviews, or field studies; (2) **Computational power** — modern hardware enables simulation of complex social systems with millions of interacting agents, processing of petabyte-scale datasets, and training of sophisticated machine learning models; (3) **Methodological advances** — natural language processing enables automated analysis of text at massive scale (political speeches, social media posts, legislative bills, news articles, historical documents), network science provides tools for analyzing social structures, and machine learning enables pattern discovery in high-dimensional social data. Key methodological approaches include: **Agent-based modeling (ABM)** — simulating social systems from the bottom up by defining individual agents with simple behavioral rules and observing emergent macro-level patterns (Schelling's segregation model, 1971 — demonstrating that mild individual preferences for same-group neighbors can produce extreme spatial segregation; Epstein and Axtell's "Sugarscape," 1996 — modeling wealth distribution, trade, cultural transmission, and conflict through interacting agents on a grid); **Computational text analysis** — topic modeling (LDA), sentiment analysis, word embeddings, and transformer-based NLP applied to corpora of political texts, social media, court decisions, and historical documents to measure ideology, detect framing, track cultural change, and identify emerging narratives; **Digital trace data analysis** — using records of online behavior (tweets, search queries, call records, GPS traces, transaction logs) as observational data for social science — studying mobility patterns, information diffusion, political polarization, health behaviors, and economic activity; **Social simulation** — using computational models to test theoretical mechanisms: how do social norms emerge? How does misinformation spread? What institutional designs promote cooperation? Under what conditions do revolutions occur?

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Established)

### 1.1 Agent-Based Modeling
- **Schelling's segregation model (1971)**: one of the earliest and most influential agent-based models — agents on a grid move if fewer than a threshold fraction of their neighbors are of the same type; even with mild preferences (e.g., wanting at least 30% same-type neighbors), extreme segregation emerges; demonstrated that macro-level patterns can arise from micro-level behaviors without any central coordination or extreme individual preferences
- **Epstein and Axtell, "Growing Artificial Societies" (Sugarscape, 1996)**: agents forage for "sugar" (resources) on a landscape, trade, reproduce, die, and develop cultural tags; from simple rules emerge wealth inequality, Pareto distributions of wealth, trade networks, and cultural clustering; established agent-based modeling as a method for "growing" social phenomena from the bottom up
- **NetLogo and Mesa**: NetLogo (Wilensky, 1999) — widely used agent-based modeling environment for education and research; Mesa (Python-based ABM framework) — popular for researchers who prefer Python integration with data science tools

### 1.2 Computational Text Analysis
- **Topic modeling (LDA — Blei, Ng, Jordan, 2003)**: Latent Dirichlet Allocation — unsupervised model that discovers latent "topics" (distributions over words) in document corpora; applied to congressional speeches (identifying policy topics), newspaper archives (tracking agenda change), social media (detecting emerging concerns), and historical documents (chronicling discourse evolution); Roberts et al.'s Structural Topic Model (STM) allows incorporating metadata (time, author characteristics) into topic estimation
- **Sentiment and ideology measurement**: applying NLP to measure political ideology from text — Wordscores (Laver et al., 2003), Wordfish, and neural methods estimate party/legislator positions from speeches and manifestos; social media sentiment analysis (opinion mining) at scale enables real-time tracking of public attitudes, though methodological challenges (sarcasm, context, demographic bias in social media populations) remain

### 1.3 Digital Trace Data
- **Lazer et al. (2009, Science)**: the founding manifesto — argued that digital trace data offers unprecedented opportunities for social science but requires interdisciplinary collaboration, new methodological training, ethical frameworks, and institutional support; sparked rapid growth of CSS programs, centers, and summer institutes worldwide
- **Call detail records and mobility**: Gonzalez et al. (2008, Nature) — analyzed anonymized mobile phone location data of 100,000 users over 6 months; found that human mobility follows Lévy flight-like patterns with high regularity; de Montjoye et al. (2013, Nature Scientific Reports) — showed that only 4 spatiotemporal data points are typically sufficient to uniquely identify 95% of individuals in a mobile phone dataset, highlighting privacy risks

---

## 2. CREDIBLE CLAIMS (Tier 2 — Academic / Debated but Supported)

### 2.1 Challenges and Critiques
- **Digital trace data biases**: social media data systematically over-represents certain demographics (younger, more urban, more politically engaged populations); search data and web behavior are shaped by platform design; the "streetlight effect" — researchers study what data is available rather than what questions are most important; Olteanu et al. (2019) and Ruths and Pfeffer (2014) systematically documented biases in digital trace data for social research
- **Algorithmic confounding**: social media platforms use recommendation algorithms that shape the data researchers observe — the content users see, engage with, and share is heavily influenced by algorithmic curation; observing behavior on a platform is observing behavior shaped by the algorithm, not "natural" behavior; this creates fundamental methodological challenges for causal inference

### 2.2 Ethics of Computational Social Science
- **Informed consent and privacy**: the Facebook emotional contagion experiment (Kramer, Guillory, and Hancock, 2014) — manipulated News Feeds of ~700,000 users without informed consent, provoking widespread criticism about the ethics of large-scale experimentation on social media users; raised questions about whether terms of service constitute informed consent and whether academic IRB review standards apply to industry collaborations
- **Surveillance and dual use**: the same techniques used to study social phenomena (tracking mobility, analyzing communication networks, identifying influence patterns) can be used for surveillance, manipulation, and social control; Zuboff's "surveillance capitalism" critique highlights the tension between computational social science as knowledge production and as a tool of corporate/state power

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Possible but Unverified)

### 3.1 LLM-Based Social Simulation
- **Using LLMs as social agents**: recent proposals (Park et al., "Generative Agents," 2023) use large language models to simulate human behavior in social environments — LLM agents plan, communicate, form relationships, and coordinate; whether LLM-based simulations can provide genuine social scientific insight or merely reproduce biases and stereotypes in training data is actively debated

---

## 4. DUBIOUS CLAIMS (Tier 4 — No Credible Source / Contradicted by Evidence)

### 4.1 Big Data Replaces Theory
- **[MISLEADING]** The "big data" enthusiasm sometimes implied that sufficient data volume could substitute for theoretical frameworks — "let the data speak for itself"; however, without theoretical grounding, data patterns are uninterpretable (correlation without causal mechanisms), biased data at scale produces biased conclusions at scale, and the choice of what to measure, how to operationalize, and what patterns to look for is always theory-laden; CSS requires integration of computational methods with social science theory, not replacement of theory by data

---

## COUNTER-ARGUMENTS

- **Digital trace biases**: **Matthew Salganik** (*Bit by Bit*, 2017) highlighted that digital trace data (social media posts, web logs) are non-representative, algorithmically confounded, and subject to platform-specific selection effects — findings from Twitter or Reddit may not generalize to broader populations. **Olteanu et al.** (2019) cataloged systematic biases in social media data used for research
- **Replication and transparency**: Computational social science studies often rely on proprietary platform data that cannot be shared for replication, raising concerns about reproducibility. The tension between data access for research and privacy protection (especially post-GDPR and Cambridge Analytica) has led **King and Persily** (2019) to propose independent data access institutions
- **LLM-based social simulation**: The emerging practice of using LLMs as simulated human subjects (**Argyle et al.**, 2023; **Park et al.**, 2023) raises methodological questions about whether language model outputs validly represent human attitudes and behaviors or merely reflect training data distributions and biases

---

## IMAGES

| # | Description | Filename | Source | License |
|---|-------------|----------|--------|---------|
*No images assigned yet.*

---

## BIBLIOGRAPHY

1. Lazer, David, et al. "Computational Social Science." *Science* 323.5915 (2009): 721–723. DOI: 10.1126/science.1167742
2. Epstein, Joshua M., and Robert Axtell. *Growing Artificial Societies: Social Science from the Bottom Up*. Washington, DC: Brookings, 1996. DOI: 10.1177/000169939804100106
3. Salganik, Matthew J. *Bit by Bit: Social Research in the Digital Age*. Princeton: Princeton University Press, 2018. DOI: 10.1126/science.aaq0679
4. Blei, David M., Andrew Y. Ng, and Michael I. Jordan. "Latent Dirichlet Allocation." *JMLR* 3 (2003): 993–1022. DOI: 10.7551/mitpress/1120.003.0082
5. Schelling, Thomas C. "Dynamic Models of Segregation." *Journal of Mathematical Sociology* 1.2 (1971): 143–186. DOI: 10.1080/0022250x.1971.9989794
6. Gonzalez, Marta C., Cesar A. Hidalgo, and Albert-László Barabási. "Understanding Individual Human Mobility Patterns." *Nature* 453.7196 (2008): 779–782.
7. Grimmer, Justin, Margaret E. Roberts, and Brandon M. Stewart. *Text as Data: A New Framework for Machine Learning and the Social Sciences*. Princeton: Princeton University Press, 2022.
8. Park, Joon Sung, et al. "Generative Agents: Interactive Simulacra of Human Behavior." *UIST* (2023): Article 2.
9. Lazer, David, et al. "Computational Social Science." *Science* 323.5915 (2009): 721–723.
10. Salganik, Matthew J. *Bit by Bit: Social Research in the Digital Age*. Princeton: Princeton University Press, 2018.
11. Epstein, Joshua M. *Generative Social Science: Studies in Agent-Based Computational Modeling*. Princeton: Princeton University Press, 2006.
12. Watts, Duncan J. "A Twenty-First Century Science." *Nature* 445 (2007): 489.
13. Conte, Rosaria, et al. "Manifesto of Computational Social Science." *European Physical Journal Special Topics* 214.1 (2012): 325–346.
14. Cioffi-Revilla, Claudio. *Introduction to Computational Social Science: Principles and Applications*. 2nd ed. Cham: Springer, 2017.
15. Bail, Christopher A., et al. "Exposure to Opposing Views on Social Media Can Increase Political Polarization." *Proceedings of the National Academy of Sciences* 115.37 (2018): 9216–9221.
16. Axelrod, Robert. *The Evolution of Cooperation*. rev. ed. New York: Basic Books, 2006 [1984].
17. King, Gary. "Ensuring the Data-Rich Future of the Social Sciences." *Science* 331.6018 (2011): 719–721.
18. Centola, Damon. "The Spread of Behavior in an Online Social Network Experiment." *Science* 329.5996 (2010): 1194–1197.
19. Lazer, David, et al. "The Parable of Google Flu: Traps in Big Data Analysis." *Science* 343.6176 (2014): 1203–1205.
20. Macy, Michael W., and Robert Willer. "From Factors to Actors: Computational Sociology and Agent-Based Modeling." *Annual Review of Sociology* 28 (2002): 143–166.
21. Grimmer, Justin, Margaret E. Roberts, and Brandon M. Stewart. *Text as Data: A New Framework for Machine Learning and the Social Sciences*. Princeton: Princeton University Press, 2022.


---

## CROSS-REFERENCE INDEX

| Related Doc | Connection |
|-------------|-----------|
| [ZC_5_11](../../ZC_Social_Science/ZC5_Modern_Applied_Social_Science/ZC_5_11_Digital_Sociology.md) | Digital sociology |
| [ZD_5_05](ZD_4_13_Network_Science.md) | Network science |
| [ZD_1_02](../ZD1_Foundations_Theory/ZD_1_02_Information_Theory.md) | Mathematics/information |

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
