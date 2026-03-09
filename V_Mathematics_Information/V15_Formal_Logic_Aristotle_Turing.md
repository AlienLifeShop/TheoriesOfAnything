# V15 — Formal Logic: Aristotle to Turing

> **Document ID:** V15
> **Section:** V_Mathematics_Information
> **Keywords:** logic, formal logic, Aristotle, syllogism, Boolean algebra, Frege, Begriffsschrift, Russell, Whitehead, Principia Mathematica, Gödel, Turing, computability, decidability, predicate logic, propositional logic
> **Category Tags:** mathematics, information
> **Cross-References:** P30 · [ZD01](V03_Algorithms_Computation_Limits.md) · P08 · S01
> **Reliability Tier:** Tier 1 (mathematical proofs and established historical scholarship)
> **Last Updated:** Mar 07, 2026 | **Source Count:** 20 | **Weighted Score:** 37 | **Source Confidence:** [4/5] | **Confidence:** High

---

## QUICK SUMMARY

Formal logic — the systematic study of valid inference — spans 2,400 years from **Aristotle's syllogistic** (c. 350 BCE) to **Turing's computation theory** (1936). Aristotle's *Organon* established the syllogism as the fundamental unit of deductive reasoning and dominated Western logic for nearly two millennia. The 19th century saw an explosion of innovation: **George Boole** (1854) algebraized logic, **Gottlob Frege** (1879) created modern predicate logic with quantifiers in his *Begriffsschrift*, and **Giuseppe Peano** developed symbolic notation for arithmetic. **Russell and Whitehead's** *Principia Mathematica* (1910–1913) attempted to derive all of mathematics from logic (logicism), but **Gödel's incompleteness theorems** (1931) showed that any consistent formal system powerful enough for arithmetic contains truths it cannot prove. **Alan Turing** (1936) resolved the *Entscheidungsproblem* (decision problem) by defining the **Turing machine** and proving that no algorithm can decide the truth of all mathematical statements — simultaneously founding theoretical computer science. The history of formal logic is the story of humanity's attempt to mechanize reasoning, its remarkable successes, and the discovery of its inherent limitations.

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Established Scholarship)

### 1.1 Aristotle's syllogistic logic (c. 350 BCE)

- **Aristotle** (384–322 BCE) developed the **syllogism** — a deductive argument with two premises and a conclusion — in the *Prior Analytics* (part of the *Organon*).
- Example: "All men are mortal; Socrates is a man; therefore Socrates is mortal."
- Classified 256 possible syllogistic forms into 24 valid moods (later refined to 15 unconditionally valid moods in three figures, later four).
- **Square of opposition**: systematic relationships (contradiction, contrariety, subalternation) between categorical propositions (All S are P / No S are P / Some S are P / Some S are not P).
- **Dominance**: Aristotelian logic was the core of Western education (the trivium: grammar, logic, rhetoric) for roughly 2,000 years — Kant (1787) declared that logic "has not had to retrace a single step" since Aristotle.
- **Limitations**: Aristotelian logic cannot handle relations (e.g., "A is taller than B"), multiple quantifiers, or mathematical induction — these required the 19th-century revolution.

### 1.2 Stoic and medieval contributions

- **Stoic logic** (Chrysippus, c. 279–206 BCE): developed **propositional logic** — inference rules governing "if…then," "or," "and" — complementing Aristotle's term logic. Five basic inference schemas (indemonstrables).
- **Medieval logicians**: Peter Abelard (12th c., modal logic), William of Ockham (14th c., nominalism and supposition theory), Jean Buridan (14th c., consequences and self-reference paradoxes).
- **Indian logic**: Nyāya school (Gautama's *Nyāya Sūtras*, c. 2nd c. CE) independently developed a five-membered syllogism and sophisticated theories of inference (*anumāna*), perception, and debate rules.
- **Buddhist logic**: Dignāga (5th–6th c. CE) and Dharmakīrti (7th c. CE) developed formal theories of inference remarkably parallel to Western developments.

### 1.3 Boole, De Morgan, and the algebraization of logic (1847–1854)

- **George Boole** (1815–1864), *The Laws of Thought* (1854): reformulated logic as algebra — propositions as variables (0 or 1), conjunction as multiplication, disjunction as addition, negation as complement.
- **Boolean algebra** became the mathematical foundation of digital circuit design (Shannon's master's thesis, 1938, showed that switching circuits implement Boolean algebra).
- **Augustus De Morgan** (1806–1871): De Morgan's laws ($\neg(A \wedge B) = \neg A \vee \neg B$), formalized the logic of relations.
- Together, Boole and De Morgan liberated logic from Aristotelian term structure and opened it to mathematical treatment.

### 1.4 Frege's *Begriffsschrift* and modern predicate logic (1879)

**Gottlob Frege** (1848–1925):
- ***Begriffsschrift*** ("Concept-Script," 1879): invented modern **predicate logic** with quantifiers (∀, "for all"; ∃, "there exists"), variables, functions, and a formal proof system — the single most important advance in logic since Aristotle.
- Distinguished **sense** (*Sinn*) from **reference** (*Bedeutung*) — foundational for philosophy of language.
- ***Die Grundlagen der Arithmetik*** (1884): attempted to reduce arithmetic to logic (logicism) — defining numbers as equivalence classes of concepts.
- ***Grundgesetze der Arithmetik*** (vol. 1, 1893; vol. 2, 1903): the full formal derivation — but just before vol. 2's publication, Bertrand Russell informed Frege that his system was **inconsistent** (Russell's Paradox: the set of all sets that don't contain themselves).
- Frege's notation was two-dimensional and never adopted, but his logical system — translated into modern notation by Peano and Russell — remains the foundation of mathematical logic.

### 1.5 Russell, Whitehead, and *Principia Mathematica* (1910–1913)

- **Bertrand Russell** (1872–1970) and **Alfred North Whitehead** (1861–1947): *Principia Mathematica* (3 volumes, 1910–1913) — the most ambitious attempt to derive all of mathematics from purely logical axioms.
- To avoid Russell's Paradox, they introduced the **theory of types** — a hierarchy forbidding self-referential set membership.
- The proof that $1 + 1 = 2$ appears on page 379 of Volume I (proposition *54.43), with the note "the above proposition is occasionally useful."
- **Logicism** — the thesis that mathematics is reducible to logic — was the driving philosophical program. While *Principia* demonstrated the power of formal systems, Gödel's theorems (1931) showed that the logicist program cannot be fully completed.

### 1.6 Gödel's incompleteness theorems (1931)

**Kurt Gödel** (1906–1978):
- **First Incompleteness Theorem**: any consistent formal system $F$ capable of expressing basic arithmetic contains a statement $G$ that is true but unprovable within $F$. (Gödel constructed $G$ to say, in effect, "this statement is not provable in $F$.")
- **Second Incompleteness Theorem**: such a system $F$ cannot prove its own consistency (unless it is inconsistent).
- **Method**: Gödel numbering — encoding logical formulas as natural numbers, allowing the system to "talk about itself."
- **Impact**: destroyed Hilbert's program to prove mathematics consistent and complete from finitary methods. (See also V12.)
- Gödel's theorems do not imply that mathematics is unreliable — they show that no single formal system can capture all mathematical truth.

### 1.7 Turing and the *Entscheidungsproblem* (1936)

**Alan Turing** (1912–1954):
- **Hilbert's *Entscheidungsproblem*** (1928): is there an algorithm that can determine the truth or falsity of any mathematical statement?
- **Turing (1936)**, "On Computable Numbers": defined the **Turing machine** — a theoretical device with an infinite tape, a read/write head, and a finite set of states — capable of computing anything that is computable by any mechanical process.
- Proved the **halting problem** is undecidable: no algorithm can determine, for all programs and inputs, whether the program halts or runs forever.
- **Consequence**: the *Entscheidungsproblem* has no solution — there are mathematical questions that no algorithm can answer. (Alonzo Church proved this independently using lambda calculus in 1936.)
- The Turing machine became the foundational model of theoretical computer science and the basis for the Church-Turing thesis.

---

## 2. CREDIBLE BUT DEBATED CLAIMS (Tier 2 — Academic / Debated)

### 2.1 The Church-Turing thesis

- **Claim**: any function computable by any physically realizable device is computable by a Turing machine.
- **Status**: widely accepted but unprovable (it is a thesis about the physical world, not a mathematical theorem).
- **Challenges**: quantum computing does not violate the thesis (quantum computers compute the same functions, just faster for some problems), but hypercomputation proposals (super-Turing machines, oracle machines) remain speculative and controversial.

### 2.2 Whether logic captures all valid reasoning

- **Formal logic** captures deductive reasoning but may not capture all forms of valid inference — abductive reasoning (inference to the best explanation), analogical reasoning, and practical reasoning are not fully formalized.
- Some philosophers (e.g., Toulmin, 1958) argue that formal logic is too narrow to model real-world argumentation.

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Possible but Unverified)

### 3.1 Ancient precursors to formal logic beyond Greece and India

Claims that ancient Egyptians, Chinese (Mohist logic), or Mesoamericans had formal logical systems comparable to Aristotelian or Nyāya logic are largely unsubstantiated. The **Mohist** *Canons* (c. 400 BCE) contain interesting logical insights but do not constitute a formal system. Egyptian wisdom literature contains reasoned argument but not systematic logic.

---

## 4. DUBIOUS OR FRINGE CLAIMS (Tier 4 — No Credible Source / Contradicted by Evidence)

### 4.1 Gödel proved that truth is unknowable

A common misinterpretation: Gödel proved that *specific formal systems* cannot prove all truths expressible within them — not that mathematical truth is unknowable. The unprovable statement $G$ *is* known to be true (by the meta-mathematical argument). The theorems concern the limitations of formal proof systems, not of human knowledge.

---

## COUNTER-ARGUMENTS & CRITICISMS

| Claim | Counter-Argument | Source |
|-------|------------------|--------|
| Formal logic is the foundation of all reasoning | Natural language reasoning often uses informal, context-dependent inference | Toulmin, 1958 |
| Logicism (math = logic) | Gödel showed arithmetic cannot be completely derived from any consistent logical system | Gödel, 1931 |
| Aristotelian logic was complete | It could not handle relations, multiple quantifiers, or mathematical induction | Frege, 1879 |
| The Church-Turing thesis is proven | It is an empirical claim about physical computability, not a mathematical theorem | Copeland, 2004 |
| Gödel's theorems undermine mathematical knowledge | They limit formal systems, not mathematical understanding; mathematicians routinely prove results Gödel-type sentences concern | Franzén, 2005 |

---

## IMAGES

| Description | Source | Type |
|-------------|--------|------|
| Aristotle's Square of Opposition | Various logic textbooks | Logical diagram |
| Page from Frege's *Begriffsschrift* (1879) | Frege, 1879 | Historical reproduction |
| *Principia Mathematica* proof of 1+1=2 | Russell & Whitehead, 1910 | Historical reproduction |
| Turing machine schematic | Turing, 1936 / various | Conceptual diagram |
| Gödel numbering example | Various | Mathematical diagram |

---

## BIBLIOGRAPHY

1. Aristotle. *Prior Analytics*. Translated by Robin Smith. Indianapolis: Hackett, 1989.
2. Boole, George. *An Investigation of the Laws of Thought*. London: Walton and Maberly, 1854.
3. Frege, Gottlob. *Begriffsschrift, eine der arithmetischen nachgebildete Formelsprache des reinen Denkens*. Halle: Louis Nebert, 1879.
4. Russell, Bertrand, and Alfred North Whitehead. *Principia Mathematica*. 3 vols. Cambridge: Cambridge University Press, 1910–1913.
5. Gödel, Kurt. "Über formal unentscheidbare Sätze der *Principia Mathematica* und verwandter Systeme I." *Monatshefte für Mathematik und Physik* 38 (1931): 173–198.
6. Turing, Alan M. "On Computable Numbers, with an Application to the Entscheidungsproblem." *Proceedings of the London Mathematical Society* 42 (1936): 230–265.
7. Church, Alonzo. "An Unsolvable Problem of Elementary Number Theory." *American Journal of Mathematics* 58 (1936): 345–363.
8. Kneale, William, and Martha Kneale. *The Development of Logic*. Oxford: Clarendon Press, 1962.
9. van Heijenoort, Jean, ed. *From Frege to Gödel: A Source Book in Mathematical Logic, 1879–1931*. Cambridge, MA: Harvard University Press, 1967.
10. Hodges, Andrew. *Alan Turing: The Enigma*. London: Burnett Books, 1983.
11. Matilal, Bimal Krishna. *The Character of Logic in India*. Albany: SUNY Press, 1998.
12. Shannon, Claude E. "A Symbolic Analysis of Relay and Switching Circuits." *Transactions of the AIEE* 57 (1938): 713–723.
13. Toulmin, Stephen. *The Uses of Argument*. Cambridge: Cambridge University Press, 1958.
14. Copeland, B. Jack, ed. *The Essential Turing*. Oxford: Oxford University Press, 2004.
15. Franzén, Torkel. *Gödel's Theorem: An Incomplete Guide to Its Use and Abuse*. Wellesley: A K Peters, 2005.
16. Stillwell, John. *Roads to Infinity: The Mathematics of Truth and Proof*. Natick: A K Peters, 2010.
17. Davis, Martin. *The Universal Computer: The Road from Leibniz to Turing*. New York: W.W. Norton, 2000.
18. Ganeri, Jonardon. "Indian Logic." In *Handbook of the History of Logic*, vol. 1, edited by Dov M. Gabbay and John Woods, 309–395. Amsterdam: Elsevier, 2004.
19. Smith, Peter. *An Introduction to Gödel's Theorems*. 2nd ed. Cambridge: Cambridge University Press, 2013.
20. Mancosu, Paolo, Richard Zach, and Calixto Badesa. "The Development of Mathematical Logic from Russell to Tarski, 1900–1935." In *The Development of Modern Logic*, edited by Leila Haaparanta, 318–470. Oxford: Oxford University Press, 2009.

---

## CROSS-REFERENCE INDEX

| Topic | Section | Document |
|-------|---------|----------|
| Logic and reasoning (philosophy) | P | P30 — Logic & Reasoning |
| Algorithms and computation | V | [ZD01 — Algorithms Computation](V03_Algorithms_Computation_Limits.md) |
| Ancient Greek philosophy | P | P08 — Ancient Greek Philosophy |
| Artificial intelligence | S | S01 — Artificial Intelligence |

---

*Document V15 · Created Mar 07, 2026 · TheoriesOfAnything Knowledge Base*
