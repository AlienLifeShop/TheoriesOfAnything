# V52 — Unsolved Problems in Mathematics

> **Document ID:** V52
> **Section:** V_Mathematics_Information
> **Keywords:** unsolved problems, Millennium Prize, Riemann hypothesis, P vs NP, Navier-Stokes, Hodge conjecture, Birch Swinnerton-Dyer, Yang-Mills, Goldbach conjecture, twin primes, Collatz, ABC conjecture, Hilbert problems, Clay Institute, open problems, mathematical conjectures, proof verification
> **Category Tags:** mathematics, information
> **Cross-References:** [V02 — Prime Numbers Riemann Hypothesis](V02_Prime_Numbers_Riemann_Hypothesis.md) · [ZD09 — Computational Complexity](V37_Computational_Complexity_P_NP.md) · [V44 — Analytic Number Theory](V44_Analytic_Number_Theory.md) · [V25 — Topology](V25_Topology_Shape_Continuity_Invariants.md) · [V20 — Mathematical Proof](V20_Mathematical_Proof.md)
> **Reliability Tier:** Tier 1 (well-documented, peer-reviewed)
> **Last Updated:** Mar 07, 2026 | **Source Count:** 10 | **Weighted Score:** 23 | **Source Confidence:** [3/5] | **Confidence:** High (well-documented, peer-reviewed)

---

## QUICK SUMMARY

Mathematics has always been driven by problems that resist solution — conjectures so deep that their resolution reshapes entire fields. The Clay Mathematics Institute's seven Millennium Prize Problems ($1 million each, announced 2000) define the frontier: the Riemann hypothesis (distribution of primes), P vs NP (computational tractability), the Navier-Stokes existence and smoothness problem (fluid dynamics), the Hodge conjecture (algebraic geometry), the Birch and Swinnerton-Dyer conjecture (elliptic curves), and Yang-Mills existence and mass gap (quantum field theory); the seventh, the Poincaré conjecture (topology), was solved by Grigori Perelman (2003, prize declined 2010). Before these, David Hilbert's 23 problems (1900) guided 20th-century mathematics — some solved (continuum hypothesis shown independent), some open (Riemann hypothesis), some reformulated. Beyond the Millennium Problems lie equally tantalizing challenges: the Goldbach conjecture (every even integer > 2 is the sum of two primes, verified to $4 \times 10^{18}$, unproven since 1742), the twin prime conjecture (infinitely many primes differing by 2, with Yitang Zhang's 2013 breakthrough proving bounded gaps), the Collatz conjecture (the simplest-sounding unsolved problem: iterate $n \mapsto n/2$ or $3n+1$ — does every positive integer eventually reach 1?), and the ABC conjecture (relating additive and multiplicative properties of integers, with Shinichi Mochizuki's controversial 2012 claimed proof still debated). These problems reveal the boundaries of mathematical knowledge and the creative tension between what can be computed, conjectured, and proven.

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Established)

### 1.1 The Millennium Prize Problems
- **Clay Mathematics Institute (2000):** Seven problems, $1 million prize each; selected to represent the most important open problems across mathematics; modeled on Hilbert's 1900 problems; announced at Collège de France, Paris, May 24, 2000
- **Riemann Hypothesis (1859):** All non-trivial zeros of the Riemann zeta function $\zeta(s) = \sum_{n=1}^{\infty} n^{-s}$ have real part $\frac{1}{2}$; trivial zeros at $s = -2, -4, -6, ...$; verified computationally for first $10^{13}+$ zeros; implies tightest possible error bound for prime counting function: $|\pi(x) - \text{Li}(x)| = O(\sqrt{x} \log x)$; connections to random matrix theory, quantum chaos, and the distribution of primes; widely considered the most important unsolved problem in mathematics
- **P vs NP (Cook, 1971):** Does every problem whose solution can be verified in polynomial time also admit a polynomial-time algorithm? P = problems solvable efficiently; NP = problems verifiable efficiently; if P = NP, efficient algorithms exist for scheduling, optimization, cryptography-breaking, protein folding; overwhelming consensus: $P \neq NP$ but no proof exists; $1 million Clay prize + central question of theoretical computer science
- **Navier-Stokes Existence and Smoothness:** Do smooth, globally defined solutions exist for the 3D incompressible Navier-Stokes equations for all time, given smooth initial data? Or do solutions develop singularities (blow up) in finite time? Fundamental for fluid dynamics; 2D case solved (Ladyzhenskaya, 1958); 3D case remains open; Tao (2016) showed blow-up possible for averaged versions of the equations
- **Hodge Conjecture:** On a non-singular complex projective algebraic variety, certain cohomology classes (Hodge classes) are rational linear combinations of classes of algebraic subvarieties; connects topology, complex analysis, and algebraic geometry; known in special cases (divisors, codimension 1); wide open in general
- **Birch and Swinnerton-Dyer Conjecture (1965):** The rank of the group of rational points on an elliptic curve $E$ equals the order of vanishing of $L(E,s)$ at $s=1$; experimentally verified for many curves; partial results (Gross-Zagier, Kolyvagin — proved for analytic rank 0 and 1); full conjecture remains open; deep connections to Langlands program
- **Yang-Mills Existence and Mass Gap:** Prove that quantum Yang-Mills theory (non-abelian gauge theory) on $\mathbb{R}^4$ exists mathematically and has a positive mass gap (lowest energy excitation has positive mass); foundational for the Standard Model of particle physics (QCD); constructive quantum field theory approach; no rigorous mathematical construction yet exists despite physical theories working spectacularly in practice

### 1.2 Poincaré Conjecture — SOLVED
- **Conjecture (1904):** Every simply connected, closed 3-manifold is homeomorphic to the 3-sphere $S^3$; generalization to higher dimensions proved by Smale ($n \geq 5$, 1961, Fields Medal 1966) and Freedman ($n = 4$, 1982, Fields Medal 1986); the $n = 3$ case was hardest
- **Perelman's proof (2002–2003):** Grigori Perelman posted three preprints on arXiv proving the Poincaré conjecture using Hamilton's Ricci flow with surgery; verified by multiple groups (Kleiner-Lott, Morgan-Tian, Cao-Zhu) over several years; actually proved the stronger Thurston geometrization conjecture
- **Perelman declined all prizes:** Declined the 2006 Fields Medal and the 2010 Clay Millennium Prize ($1 million), saying "the main reason is my disagreement with the organized mathematical community"; reclusive since; one of the most dramatic episodes in mathematical history

### 1.3 Hilbert's Problems (1900)
- **David Hilbert's address (Paris, ICM, 1900):** Presented 23 problems spanning all major areas; shaped 20th-century mathematical research; status as of 2026:
  - **Solved:** Problem 1 partially (continuum hypothesis independent — Gödel 1940, Cohen 1963); Problem 2 (consistency of arithmetic — negatively by Gödel's incompleteness theorems, 1931); Problem 3 (scissors congruence — Dehn, 1901); Problem 7 (Gelfond-Schneider theorem, 1934); Problem 10 (no algorithm for Diophantine equations — Davis, Putnam, Robinson, Matiyasevich, 1970); Problem 13 (resolved by Kolmogorov-Arnold, 1957); Problem 18 (partially — Bieberbach groups, Hales's Kepler conjecture proof, 1998/2014)
  - **Unsolved:** Problem 8 (Riemann hypothesis); Problem 12 (Kronecker's Jugendtraum generalization); Problem 16 (topology of algebraic curves)
  - **Too vague to resolve definitively:** Problem 6 (axiomatize physics); Problem 15 (Schubert calculus rigor — largely done)

---

## 2. CREDIBLE CLAIMS (Tier 2 — Strong Evidence, Active Research)

### 2.1 Number Theory Conjectures
- **Goldbach's Conjecture (1742):** Every even integer greater than 2 is the sum of two primes; verified computationally to $4 \times 10^{18}$ (Oliveira e Silva et al., 2013); weak Goldbach conjecture (every odd integer > 5 is sum of three primes) proved by Helfgott (2013); strong conjecture remains open; heuristic arguments strongly support it but no proof technique is in sight
- **Twin Prime Conjecture:** Infinitely many pairs of primes $(p, p+2)$; Yitang Zhang (2013) proved bounded gaps — infinitely many prime pairs $(p, p+H)$ with $H \leq 70,000,000$; Polymath8 project reduced $H$ to 246 (Maynard, 2014); gap of 2 still unproven; sieve theory limitations may prevent reaching 2 without fundamentally new ideas
- **Collatz Conjecture (3n+1 Problem):** Starting from any positive integer $n$, iterate: if even, $n \to n/2$; if odd, $n \to 3n+1$; conjecture: always eventually reaches 1; verified for all $n < 2^{68}$ (~$2.95 \times 10^{20}$); Tao (2019) proved "almost all" orbits achieve bounded values; Erdős: "Mathematics is not yet ready for such problems"
- **ABC Conjecture (Masser-Oesterlé, 1985):** For coprime positive integers $a + b = c$, the radical $\text{rad}(abc) = \prod_{p|abc} p$ is "usually" not much smaller than $c$; precisely: for every $\epsilon > 0$, there are finitely many triples with $c > \text{rad}(abc)^{1+\epsilon}$; would have profound implications for Diophantine equations, including a new approach to Fermat's Last Theorem

### 2.2 Algebraic and Geometric Conjectures
- **Langlands Program:** Robert Langlands's conjectures (1967 onwards) connecting number theory, algebraic geometry, and representation theory; "grand unified theory of mathematics"; functoriality conjecture, reciprocity conjecture; local Langlands proved for GL(n) over p-adic fields (Harris-Taylor, 2001; Henniart, 2000); geometric Langlands actively researched; Fields Medals: Lafforgue (2002), Scholze (2018) for related work
- **Invariant Subspace Problem:** Does every bounded linear operator on an infinite-dimensional separable Hilbert space have a non-trivial closed invariant subspace? Open since 1930s; resolved negatively for Banach spaces (Enflo, 1987; Read, 1985) but open for Hilbert spaces
- **Jacobian Conjecture (Keller, 1939):** If a polynomial map $F: \mathbb{C}^n \to \mathbb{C}^n$ has constant nonzero Jacobian determinant, is $F$ invertible (with polynomial inverse)? Open for $n \geq 2$; simple to state, extremely resistant to proof; many false proofs published

### 2.3 Combinatorics and Discrete Mathematics
- **Hadwiger Conjecture (1943):** If a graph has no $K_t$ minor, then it is $(t-1)$-colorable; proved for $t \leq 6$ (Robertson, Seymour, Thomas, 1993 for $t=6$; uses four-color theorem); open for $t \geq 7$; considered one of the most important open problems in graph theory
- **Erdős-Straus Conjecture (1948):** For every integer $n \geq 2$, the fraction $4/n$ can be written as a sum of three unit fractions: $\frac{4}{n} = \frac{1}{x} + \frac{1}{y} + \frac{1}{z}$; verified for all $n < 10^{17}$; no general proof known

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Emerging / Theoretical)

### 3.1 Mochizuki's Claimed Proof of ABC Conjecture
- Shinichi Mochizuki posted a ~500-page proof using his "inter-universal Teichmüller theory" (IUT) in August 2012; published in PRIMS (2021), journal where Mochizuki serves as editor-in-chief; many leading number theorists (Scholze, Stix) identified a specific gap they consider fatal (Corollary 3.12); Mochizuki disputes their critique; unprecedented situation: a claimed proof published in a peer-reviewed journal but rejected by significant portions of the mathematical community; resolution unclear as of 2026

### 3.2 Machine-Assisted Proof Discovery
- AI and automated theorem proving showing promise for attacking open problems — DeepMind's AlphaProof (2024) solved IMO-level problems; large language models assisting in conjecture formation; Lean/Coq formal verification ensuring proof correctness; speculation that AI might contribute to resolving Millennium Problems within decades; current capabilities far from proving deep conjectures autonomously but trajectory is encouraging

---

## 4. DUBIOUS CLAIMS (Tier 4 — Fringe / Unsubstantiated)

### 4.1 Simple Short Proofs Exist for Major Conjectures [UNLIKELY]
- Amateur mathematicians regularly submit claimed short proofs of the Riemann hypothesis, Goldbach conjecture, or P ≠ NP; virtually all contain fundamental errors; the depth of these problems suggests any proof will require either deep new techniques or very long arguments; Wiles's proof of Fermat's Last Theorem was ~130 pages using sophisticated modern machinery — and that was considered a "simpler" problem

### 4.2 Unsolved Problems Are Undecidable [SPECULATIVE]
- Some problems (like the continuum hypothesis) are indeed independent of standard axioms (ZFC); but most major conjectures (Riemann, Goldbach, P vs NP) are expected to be provable or disprovable within standard mathematics; Paris-Harrington theorem and Goodstein's theorem show some mathematical truths require axioms beyond Peano arithmetic — but this does not mean every hard problem is undecidable; claiming undecidability without evidence is often a retreat from mathematical engagement

---

## IMAGES

| # | Description | Source |
|---|-------------|--------|
| 1 | Riemann zeta function critical strip with zeros on the line | Standard analytic number theory texts |
| 2 | Collatz conjecture iteration tree for small numbers | Standard recreational mathematics |
| 3 | Perelman's Ricci flow surgery on a 3-manifold | Morgan & Tian (2007) |
| 4 | Twin prime gap results timeline (Zhang to Maynard) | Polymath8 project documentation |

---

## BIBLIOGRAPHY

1. Devlin, K. (2002). *The Millennium Problems: The Seven Greatest Unsolved Mathematical Puzzles of Our Time*. Basic Books.
2. Riemann, B. (1859). "Über die Anzahl der Primzahlen unter einer gegebenen Grösse." *Monatsberichte der Berliner Akademie*, 671–680.
3. Cook, S. A. (1971). "The Complexity of Theorem-Proving Procedures." *Proceedings of the 3rd ACM Symposium on Theory of Computing*, 151–158.
4. Perelman, G. (2002). "The Entropy Formula for the Ricci Flow and Its Geometric Applications." arXiv:math/0211159.
5. Zhang, Y. (2014). "Bounded Gaps Between Primes." *Annals of Mathematics*, 179(3), 1121–1174.
6. Tao, T. (2019). "Almost All Orbits of the Collatz Map Attain Almost Bounded Values." arXiv:1909.03562.
7. Wiles, A. (1995). "Modular Elliptic Curves and Fermat's Last Theorem." *Annals of Mathematics*, 141(3), 443–551.
8. Clay Mathematics Institute. (2000). *The Millennium Prize Problems*. Retrieved from claymath.org.
9. Gray, J. (2000). *The Hilbert Challenge*. Oxford University Press.
10. Bombieri, E. (2000). "The Riemann Hypothesis." In *The Millennium Prize Problems* (pp. 107–124). Clay Mathematics Institute.

---

## CROSS-REFERENCE INDEX

- **[V02 — Prime Numbers Riemann Hypothesis](V02_Prime_Numbers_Riemann_Hypothesis.md):** Riemann hypothesis and prime distribution
- **[ZD09 — Computational Complexity](V37_Computational_Complexity_P_NP.md):** P vs NP and complexity theory
- **[V44 — Analytic Number Theory](V44_Analytic_Number_Theory.md):** Zeta function, prime gaps, and number-theoretic conjectures
- **[V25 — Topology](V25_Topology_Shape_Continuity_Invariants.md):** Poincaré conjecture and topological classification
- **[V20 — Mathematical Proof](V20_Mathematical_Proof.md):** Nature of proof, verification, and the social process of mathematics
- **[V24 — Differential Equations](V24_Differential_Equations_Modeling_Change.md):** Navier-Stokes equations and PDE existence theory

---

*Last verified: Mar 07, 2026 — All sources peer-reviewed or from established mathematical literature*
