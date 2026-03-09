# K22 — Predictive Processing and Consciousness

> **Document ID:** K22
> **Section:** K_Consciousness
> **Keywords:** predictive processing, predictive coding, Bayesian brain, Karl Friston, Andy Clark, Jakob Hohwy, free energy principle, prediction error, generative model, prior, posterior, top-down prediction, bottom-up error, hierarchical processing, precision weighting, active inference, controlled hallucination, Anil Seth, interoception, allostasis, embodied prediction
> **Category Tags:** consciousness, neuroscience
> **Cross-References:** [K04 — Free Energy Principle](K04_Free_Energy_Principle.md) · [K16 — Neural Correlates](K16_Neural_Correlates_Consciousness.md) · [K20 — Global Workspace Theory](K20_Global_Workspace_Theory.md) · [Y02 — Altered States Psychedelics](K02_Altered_States_Psychedelics.md) · [K15 — Phantom Limb](K15_Phantom_Limb_Body_Schema.md)
> **Reliability Tier:** Tier 2 (credible, scholarly debate ongoing)
> **Last Updated:** Mar 07, 2026 | **Source Count:** 10 | **Weighted Score:** 25 | **Source Confidence:** [3/5] | **Confidence:** Moderate-High (credible, scholarly debate ongoing)

---

## QUICK SUMMARY

Predictive processing (PP) is a unifying framework in cognitive neuroscience proposing that the brain is fundamentally a prediction machine — it continuously generates top-down predictions of incoming sensory input and updates its internal model based on bottom-up prediction errors (the mismatch between predictions and actual input). Rooted in Helmholtz's "unconscious inference" (1867) and formalized through Bayesian probability, predictive coding models (Rao and Ballard, 1999), and Karl Friston's free energy principle (2006–present), PP offers a comprehensive account of perception, action, attention, learning, and — increasingly — consciousness. In this framework, perception is not a passive reception of sensory data but an active construction: what we experience is the brain's "best guess" (posterior inference) about the causes of sensory signals. Anil Seth has called conscious experience a "controlled hallucination" — the brain's predictions constrained by sensory evidence. Precision weighting (the brain's estimate of the reliability of prediction errors) functions as attention: increasing the gain on reliable signals and suppressing unreliable ones. Psychedelic states, meditation, and psychosis can all be understood as alterations in the precision weighting of the predictive hierarchy. While PP provides an elegant computational framework for many aspects of consciousness, whether it can address the "hard problem" (why prediction processing feels like anything) remains debated.

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Established Neuroscience)

### 1.1 Foundations of Predictive Coding
- **[KEY FINDING]** The brain implements a hierarchical generative model that predicts sensory input at every level — higher cortical areas generate predictions (top-down signals transmitted via feedback connections); lower areas compute prediction errors (mismatch between prediction and input, transmitted via feedforward connections); only prediction errors propagate upward; when predictions are accurate, error signals are minimized and processing is efficient; this is "predictive coding" (Rao and Ballard, 1999)
- **Bayesian inference in the brain:** Perception = Bayesian posterior inference: $P(\text{cause}|\text{sensory data}) \propto P(\text{sensory data}|\text{cause}) \times P(\text{cause})$ — prior beliefs (learned expectations) combine with likelihood (sensory evidence) to form the percept; explains perceptual illusions as strong priors overriding weak sensory evidence; explains perceptual learning as updating priors; Doya et al. (2007): neural circuits implement approximate Bayesian computation
- **Neural implementation evidence:** Montague (2006), Keller and Mrsic-Flogel (2018): visual cortex responses are best explained as prediction errors rather than feature detections — V1 neurons respond more to unexpected stimuli than predicted ones (mismatch responses); oddball paradigms in auditory cortex (MMN: mismatch negativity) reflect prediction error signals; feedforward and feedback connections have distinct laminar profiles consistent with error vs. prediction signals (layer 2/3 vs. layer 5/6)
- **Repetition suppression and expectation suppression:** Repeated stimuli produce reduced neural responses (repetition suppression) — PP explains this as more accurate predictions reducing prediction errors; expectation suppression (predicted stimuli produce reduced responses even without repetition) has been demonstrated in fMRI (Summerfield et al., 2008); both phenomena are natural consequences of predictive coding

### 1.2 Precision Weighting as Attention
- **[KEY FINDING]** Precision = the inverse variance of a probability distribution — in PP, the brain estimates the precision (reliability) of prediction errors at each level; high-precision errors receive greater weight and drive stronger model updating; low-precision errors are suppressed; precision weighting IS attention: increasing precision on a signal channel is equivalent to attending to it; this provides a computational account of both top-down (voluntary) and bottom-up (salience-driven) attention
- **Neuromodulatory implementation:** Precision weighting is hypothesized to be implemented by neuromodulatory systems — acetylcholine modulates sensory precision (cholinergic input to cortex, Yu and Dayan, 2005); dopamine modulates reward prediction precision; serotonin modulates prior precision (Carhart-Harris and Friston, 2019: REBUS model of psychedelics — reduced serotonin-2A mediated precision of high-level priors); norepinephrine modulates the gain of prediction error processing (unexpected uncertainty, Dayan and Yu, 2006)

### 1.3 Active Inference and Action
- **Action as prediction fulfillment:** In PP, action is the motor system's way of fulfilling predictions — proprioceptive predictions of limb position are fulfilled by moving the limb to match the predicted state; this is "active inference" (Friston, 2010); eliminates the traditional perception-action divide: both perception and action serve the same goal of minimizing prediction error (free energy); oculomotor behavior (saccades) selects sensory samples that reduce uncertainty about the environment ("epistemic foraging")

---

## 2. CREDIBLE CLAIMS (Tier 2 — Academic / Debated but Supported)

### 2.1 Consciousness as Controlled Hallucination
- **Anil Seth's "beast machine" framework (2021):** Consciousness = the brain's best prediction of the causes of sensory signals — "we don't passively perceive the world, we actively generate it"; perceptual experience is a controlled hallucination constrained (but not determined) by sensory input; when the model becomes decoupled from sensory evidence (dreams, psychedelics, psychosis), the hallucination becomes "uncontrolled"
- **Interoceptive predictive processing:** Seth extends PP to interoception (the sense of the body's internal state) — the experience of emotion, mood, and self is the brain's prediction of the physiological causes of interoceptive signals; allostatic predictions (predicting and regulating body budget) underlie mood, motivation, and homeostasis; Lisa Feldman Barrett's "constructed emotion" theory is compatible: emotions are predictions about the body's internal state, not readouts of fixed circuits
- **REBUS model of psychedelics (Carhart-Harris and Friston, 2019):** Psychedelics (psilocybin, LSD, DMT) reduce the precision weighting of high-level priors via serotonin 5-HT2A receptor agonism — this "relaxes" the brain's prior model, allowing prediction errors to propagate more freely, leading to: vivid perception, ego dissolution, synesthesia, emotional lability, creative insights; explains both the therapeutic potential and the phenomenology of psychedelic experience within the PP framework

### 2.2 Clinical Applications
- **Autism as precision imbalance (Pellicano and Burr, 2012):** Proposed that autism involves weakened priors (reduced influence of contextual predictions) — leading to heightened sensory precision, overwhelming detail perception, difficulty with social prediction (social cognition requires strong prior models), and need for routine (reduced ability to form flexible predictions); some experimental support but controversial — alternative accounts emphasize different precision imbalances
- **Psychosis as false inference:** Delusions and hallucinations = failures of predictive processing — aberrant precision signals cause prediction errors to be given excessive weight (Fletcher and Frith, 2009); the brain constructs a "best explanation" for internally generated noise, producing hallucinations and delusional interpretations; dopaminergic dysfunction disrupts precision estimation; antipsychotics work by modulating precision signals

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Possible but Unverified)

### 3.1 PP and the Hard Problem
- **Can PP explain phenomenal consciousness?** PP elegantly accounts for the structure and content of experience but faces the same challenge as other computational theories: why does information processing feel like anything? — Hohwy (2013) argues that PP's self-modeling (the brain predicting its own states) creates the conditions for phenomenal consciousness; Seth proposes that the "realness" of perception correlates with the richness of the generative model; critics argue these are descriptions of the correlates of consciousness, not explanations of experience itself
- **"Dark room problem":** If the brain minimizes prediction error, why doesn't it seek a dark, featureless room where all predictions are trivially confirmed? — Friston resolves this by noting that biological agents have evolved priors that predict certain states (eating, exploring, socializing) as probable, creating "prior preferences" that drive adaptive behavior; the free energy framework thus encompasses homeostasis, motivation, and curiosity through precision-weighted prior preferences

---

## 4. DUBIOUS CLAIMS (Tier 4 — No Credible Source / Contradicted by Evidence)

### 4.1 "The Brain Is Just a Passive Bayesian Calculator"
- **[MISLEADING]** PP does not imply passive computation — active inference (action as prediction fulfillment) and precision weighting (selective attention as gain control) make the system fundamentally active and embodied; nor does PP claim exact Bayesian inference: the brain uses approximations (variational inference, sampling); the "Bayesian brain" is a computational-level theory, not a claim about the algorithmic implementation

---

## IMAGES

| # | Description | Filename | Source | License |
|---|-------------|----------|--------|---------|
| 1 | Diagram of hierarchical predictive coding with top-down predictions and bottom-up prediction errors | — | — | — |

---

## BIBLIOGRAPHY

1. Rao, R. P. N. and Ballard, D. H. "Predictive Coding in the Visual Cortex: A Functional Interpretation of Some Extra-Classical Receptive-Field Effects." *Nature Neuroscience*, vol. 2, 1999, pp. 79–87.
2. Friston, K. "The Free-Energy Principle: A Unified Brain Theory?" *Nature Reviews Neuroscience*, vol. 11, 2010, pp. 127–138.
3. Clark, A. "Whatever Next? Predictive Brains, Situated Agents, and the Future of Cognitive Science." *Behavioral and Brain Sciences*, vol. 36, 2013, pp. 181–204.
4. Seth, A. K. *Being You: A New Science of Consciousness*. Dutton, 2021.
5. Carhart-Harris, R. L. and Friston, K. J. "REBUS and the Anarchic Brain: Toward a Unified Model of the Brain Action of Psychedelics." *Pharmacological Reviews*, vol. 71, 2019, pp. 316–344.
6. Hohwy, J. *The Predictive Mind*. Oxford University Press, 2013.
7. Keller, G. B. and Mrsic-Flogel, T. D. "Predictive Processing: A Canonical Cortical Computation." *Neuron*, vol. 100, 2018, pp. 424–435.
8. Pellicano, E. and Burr, D. "When the World Becomes 'Too Real': A Bayesian Explanation of Autistic Perception." *Trends in Cognitive Sciences*, vol. 16, 2012, pp. 504–510.
9. Barrett, L. F. *How Emotions Are Made: The Secret Life of the Brain*. Houghton Mifflin Harcourt, 2017.
10. Fletcher, P. C. and Frith, C. D. "Perceiving Is Believing: A Bayesian Approach to Explaining the Positive Symptoms of Schizophrenia." *Nature Reviews Neuroscience*, vol. 10, 2009, pp. 48–58.

---

## CROSS-REFERENCE INDEX

| Related Doc | Connection |
|-------------|-----------|
| [K04 — Free Energy Principle](K04_Free_Energy_Principle.md) | Predictive processing is the neural implementation of Friston's free energy principle |
| [K16 — Neural Correlates](K16_Neural_Correlates_Consciousness.md) | PP proposes that the NCC is the brain's generative model and its precision-weighted prediction errors |
| [K20 — Global Workspace Theory](K20_Global_Workspace_Theory.md) | GWT's "ignition" may correspond to prediction errors surpassing a precision-weighted threshold for global broadcasting |
| [Y02 — Altered States Psychedelics](K02_Altered_States_Psychedelics.md) | REBUS model explains psychedelic phenomenology as relaxation of high-level predictive priors |
| [K15 — Phantom Limb](K15_Phantom_Limb_Body_Schema.md) | Phantom limb experiences are maintained by persistent proprioceptive predictions for absent limbs |

---

*New research document — Phase 9 expansion. Last Updated: Mar 07, 2026*
