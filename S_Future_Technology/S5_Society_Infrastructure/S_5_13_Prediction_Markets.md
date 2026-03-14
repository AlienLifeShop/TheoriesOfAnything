# S_5_13 — Prediction Markets: Collective Intelligence and Crowd Forecasting

> **Source Count:** 10 | **Weighted Score:** 23 | **Source Confidence:** [3/5] | **Primary Tier:** 2 | **Last Updated:** March 11, 2026
> **Keywords:** prediction market, forecasting, wisdom of crowds, information aggregation, betting market, Polymarket, Metaculus, PredictIt, Iowa Electronic Markets, Augur, futarchy, crowd forecasting, Tetlock, superforecasting, calibration, Brier score, efficient market hypothesis
> **Category Tags:** future-technology, prediction-markets, collective-intelligence, forecasting, crowd-wisdom
> **Cross-References:** V_4_11 — Game Theory · [S_1_14 — Internet of Things](../S1_AI_Computing_Digital/S_1_14_Quantum_Internet.md) · [ZC_4_08 — Social Science Overview](../../ZC_Social_Science/ZC4_Anthropology_Culture/ZC_4_08_Structuralism_Social_Science.md)

---

## QUICK SUMMARY

**Prediction markets** — markets where participants buy and sell contracts whose payoffs depend on the outcome of future events — aggregate dispersed information into probability estimates with remarkable accuracy, often outperforming polls, expert panels, and statistical models. The core mechanism mirrors stock markets: if a contract pays $1 if Event X occurs and $0 if it doesn't, its market price directly reflects the crowd's consensus probability. The **Iowa Electronic Markets (IEM)**, established in 1988 at the University of Iowa, demonstrated that small-scale prediction markets predicted US presidential election outcomes more accurately than major polls 74% of the time. **PredictIt**, a CFTC-regulated US platform, allowed political event trading until 2024. **Polymarket**, operating on blockchain (Polygon), became the dominant platform during 2023–2024, with >$1 billion in trading volume on the 2024 US presidential election alone. The theoretical foundation rests on the **efficient market hypothesis** applied to information: when participants have financial incentives to bet accurately, market prices incorporate available information rapidly and efficiently. Philip **Tetlock's** *Good Judgment Project* (GJP) — the largest forecasting tournament ever conducted — demonstrated that trained "**superforecasters**" (the top ~2% of participants) outperformed intelligence analysts with access to classified information, and that prediction markets composed of superforecasters performed even better. **Calibration** and **Brier scores** provide quantitative measures of forecasting accuracy. Applications extend beyond politics: corporate decision-making (Google, HP, and Ford have used internal prediction markets), public health (pandemic forecasting), climate risk, and Robin Hanson's concept of **futarchy** — governance by prediction markets ("vote on values, bet on beliefs"). Challenges include regulatory restrictions (US CFTC limits), market manipulation, thin markets on niche topics, legal gambling classifications, and ethical concerns about incentivizing bets on harmful events.

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Established)

### 1.1 Mechanism and Theory
- **Arrow-Debreu securities**: theoretical foundation — contracts that pay off contingent on specific states of the world; prediction market contracts are practical implementations
- **Price as probability**: if a binary contract trades at $0.65, the market consensus probability of the event is ~65%
- **Information aggregation**: Hayek's insight that markets aggregate dispersed knowledge — applied to predictions. Each trader contributes their private information through their trades; the market price integrates all contributions
- **Scoring rules**: **Brier score** (mean squared error of probabilistic predictions) and **logarithmic scoring rule** provide rigorous measures of forecast calibration and sharpness

### 1.2 Empirical Track Record
- **Iowa Electronic Markets (IEM)**: Berg, Nelson & Rietz (2008) — IEM election markets outperformed polls in 74% of 964 comparisons across 5 presidential elections:
  - Markets produced lower prediction errors than final pre-election polls despite having only hundreds of participants and small stakes
- **InTrade/TradeSports**: predicted outcomes of elections, Supreme Court decisions, Oscar winners, and economic indicators — market prices consistently well-calibrated
- **Polymarket (2023–2024)**: drew massive attention during 2024 US election cycle; >$1 billion in volume on presidential outcome; market-implied probabilities moved with news events in near-real-time

### 1.3 Superforecasting
- **Tetlock's Good Judgment Project (GJP)** (2011–2015; Tetlock & Gardner, 2015):
  - ~20,000 participants made >1 million predictions on geopolitical events
  - Top 2% ("superforecasters") were ~30% more accurate than intelligence analysts with classified access
  - Superforecaster characteristics: open-minded, numerate, actively seek disconfirming evidence, update beliefs incrementally, use base rates
  - Prediction markets aggregating superforecasters' judgments outperformed both individual superforecasters and large crowd aggregates

---

## 2. CREDIBLE CLAIMS (Tier 2 — Academic / Debated but Supported)

### 2.1 Corporate and Institutional Applications
- **Internal prediction markets**: Google, HP, Ford, Eli Lilly, and the US intelligence community (IARPA ACE program) have deployed internal prediction markets:
  - Google's internal market (2005–): employees traded on product launch dates, quarterly revenue, and strategic decisions — outperforming internal forecasting teams
  - HP: market-based sales forecasts outperformed official forecasts in 6 of 8 quarters tested (Chen & Plott, 2002)
- **Pandemic forecasting**: Metaculus (a forecasting platform using reputation-based scoring rather than money) produced well-calibrated COVID-19 forecasts for case counts, vaccine timelines, and policy decisions

### 2.2 Futarchy — Governance by Prediction Market
- **Robin Hanson (2000)**: proposed "futarchy" — a form of governance where elected officials define national welfare metrics, and prediction markets determine which policies are most likely to achieve those metrics:
  - "Vote on values, bet on beliefs"
  - Never implemented at government scale, but experiments in corporate governance and decentralized autonomous organizations (DAOs) explore market-based decision-making

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Possible but Unverified)

### 3.1 Prediction Markets as Universal Decision Tools
- Enthusiasts argue prediction markets could transform fields from climate policy (betting on warming trajectories) to pandemic response (real-time outbreak probability markets) to corporate strategy. However, markets require sufficient liquidity, motivated informed participants, clearly resolvable questions, and legal frameworks — conditions not easily met for all decision domains. Thin markets on obscure topics can be easily manipulated and produce unreliable prices

---

## 4. DUBIOUS CLAIMS (Tier 4 — No Credible Source / Contradicted by Evidence)

### 4.1 Prediction Markets Are Always Right
- **[MISLEADING]** Prediction markets are probabilistic — a 70% market price means the event should occur ~70% of the time, not that it definitely will. Markets can also be systematically biased: **favorite-longshot bias** (overpricing longshots), **late momentum effects**, thin-market noise, and susceptibility to manipulation. They are the best available aggregation tool, not an infallible oracle

---

## COUNTER-ARGUMENTS

- **Thin markets and manipulation**: prediction markets often suffer from low liquidity, which makes them vulnerable to manipulation by well-funded actors — **Justin Wolfers and Eric Zitzewitz** (2004, *Journal of Economic Perspectives*) found that while prediction markets generally outperform polls, they can exhibit systematic biases when trading volume is low or dominated by a small number of participants
- **Regulation as barrier**: **Cass Sunstein** (Harvard, 2006, *Journal of Political Philosophy*) raised concerns that prediction markets on politically sensitive events (elections, terrorism, policy outcomes) face inherent regulatory obstacles because they resemble gambling, and that public distaste for “profiting from disaster” (as seen in the rapid shutdown of DARPA’s Policy Analysis Market/“terror futures” in 2003) may permanently limit their adoption for the most valuable forecasting domains

---

## IMAGES

| # | Description | Filename | Source | License |
|---|-------------|----------|--------|---------|
*No images assigned yet.*

---

## BIBLIOGRAPHY

1. Tetlock, Philip E., and Dan Gardner. *Superforecasting: The Art and Science of Prediction.* New York: Crown, 2015. DOI: 10.5038/1944-0472.9.1.1519
2. Berg, Joyce E., Robert Forsythe, Forrest Nelson, and Thomas A. Rietz. "Results from a Dozen Years of Election Futures Markets Research." In *Handbook of Experimental Economics Results*, Vol. 1, edited by Charles R. Plott and Vernon L. Smith, 742–751. Amsterdam: North-Holland, 2008. DOI: 10.1016/s1574-0722(07)00080-7
3. Arrow, Kenneth J., et al. "The Promise of Prediction Markets." *Science* 320.5878 (2008): 877–878.
4. Hanson, Robin. "Shall We Vote on Values, But Bet on Beliefs?" *Journal of Political Philosophy* 21.2 (2013): 151–178. DOI: 10.1111/jopp.12008
5. Wolfers, Justin, and Eric Zitzewitz. "Prediction Markets." *Journal of Economic Perspectives* 18.2 (2004): 107–126. DOI: 10.1257/0895330041371321
6. Chen, Kay-Yut, and Charles R. Plott. "Information Aggregation Mechanisms: Concept, Design and Implementation for a Sales Forecasting Problem." Working Paper, California Institute of Technology, 2002.
7. Manski, Charles F. "Interpreting the Predictions of Prediction Markets." *Economics Letters* 91.3 (2006): 425–429. DOI: 10.1016/j.econlet.2006.01.004
8. Servan-Schreiber, Emile, et al. "Prediction Markets: Does Money Matter?" *Electronic Markets* 14.3 (2004): 243–251.
9. Page, Scott E. *The Difference: How the Power of Diversity Creates Better Groups, Firms, Schools, and Societies.* Princeton: Princeton University Press, 2007.
10. Surowiecki, James. *The Wisdom of Crowds.* New York: Doubleday, 2004.

---

## CROSS-REFERENCE INDEX

| Related Doc | Connection |
|-------------|-----------|
| V_4_11 | Game theory |
| [S_1_14](../S1_AI_Computing_Digital/S_1_14_Quantum_Internet.md) | Internet of Things |
| [ZC_4_08](../../ZC_Social_Science/ZC4_Anthropology_Culture/ZC_4_08_Structuralism_Social_Science.md) | Social science |

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
