# ZD08 — Cryptography: Mathematics of Secrecy and Trust

> **Document ID:** ZD08
> **Section:** Information & Computation
> **Keywords:** cryptography, encryption, RSA, elliptic curve cryptography, ECC, public key, private key, symmetric encryption, AES, hash functions, SHA-256, digital signatures, Diffie-Hellman, zero knowledge proofs, post-quantum cryptography, lattice cryptography, homomorphic encryption, information-theoretic security, one-time pad, Shor algorithm, key exchange, TLS, blockchain
> **Category Tags:** information-computation, information, quantum-physics
> **Cross-References:** [V22 — Number Theory](../V_Mathematics_Information/V22_Number_Theory_Primes_Patterns.md) · V08 — Information Theory · N06 — Codes and Ciphers · [ZA06 — Quantum Entanglement](../ZA_Physics_Quantum/ZA06_Quantum_Entanglement_Nonlocality.md) · S07 — AI/ML
> **Reliability Tier:** Tier 1 (well-documented, peer-reviewed)
> **Last Updated:** Mar 07, 2026 | **Source Count:** 10 | **Weighted Score:** 26 | **Source Confidence:** [3/5] | **Confidence:** High (well-documented, peer-reviewed)

---

## QUICK SUMMARY

Cryptography — the science of secure communication — has evolved from ancient substitution ciphers into one of the deepest applications of pure mathematics. Modern cryptographic systems rest on the computational hardness of mathematical problems: factoring large integers (RSA), computing discrete logarithms (Diffie-Hellman), and finding shortest vectors in lattices (post-quantum). The 1976 Diffie-Hellman key exchange and 1977 RSA algorithm revolutionized secure communication by enabling public-key cryptography — two parties who have never met can establish a shared secret. The rise of quantum computing threatens current systems via Shor's algorithm, driving the development of post-quantum cryptographic standards finalized by NIST in 2024.

---

## 1. VERIFIED CLAIMS (Tier 1 — Peer-Reviewed / Established)

### 1.1 Symmetric Cryptography
- **Symmetric encryption:** Same key encrypts and decrypts — fast (hardware-accelerated); key distribution is the fundamental challenge
- **AES (Advanced Encryption Standard, 2001):** Rijndael cipher selected by NIST; 128/192/256-bit keys; substitution-permutation network; ~50 billion operations per second on modern hardware
- **One-time pad (Vernam, 1917):** Provably unbreakable if key is truly random, at least as long as message, and never reused — Shannon (1949) proved this is information-theoretically secure
- **Block ciphers vs. stream ciphers:** AES operates on 128-bit blocks; ChaCha20 generates a keystream (faster in software); both widely deployed
- **[KEY FINDING]** The one-time pad is the ONLY cryptosystem proven perfectly secure — all other systems rely on computational hardness assumptions that could theoretically be broken

### 1.2 Public-Key Cryptography
- **Diffie-Hellman key exchange (1976):** Two parties agree on shared secret over insecure channel using modular exponentiation — g^a mod p and g^b mod p; shared secret = g^(ab) mod p
- **RSA (Rivest-Shamir-Adleman, 1977):** Public key (N=pq, e); private key (d); encrypt: c = mᵉ mod N; decrypt: m = cᵈ mod N — security relies on difficulty of factoring N
- **Elliptic Curve Cryptography (Koblitz, Miller, 1985):** Uses point addition on elliptic curves over finite fields — 256-bit ECC ≈ 3072-bit RSA security; used in Bitcoin, TLS, Signal Protocol
- **Digital signatures:** RSA, ECDSA, EdDSA — mathematically prove a message was created by the key holder; non-repudiation
- **Key sizes (2025):** RSA-2048 minimum for security; ECC-256 standard; AES-256 for symmetric — NIST recommends transition to larger keys for long-term security

### 1.3 Hash Functions
- **Cryptographic hash:** Maps arbitrary-length input to fixed-length output — requirements: preimage resistance, second-preimage resistance, collision resistance
- **SHA-256 (NSA, 2001):** 256-bit output; used in Bitcoin proof-of-work, TLS certificates, file integrity verification
- **SHA-3 (Keccak, 2015):** Sponge construction by Bertoni, Daemen, Peeters, Van Assche — selected by NIST via public competition; different internal structure from SHA-2
- **MD5, SHA-1:** Both broken (collision attacks found) — MD5 by Wang et al. (2004), SHA-1 by Stevens et al. (2017, SHAttered attack); should not be used for security
- **Applications:** Password storage (with salting/key stretching — bcrypt, Argon2), blockchain, digital signatures, commitment schemes

### 1.4 TLS and Internet Security
- **TLS 1.3 (2018):** Standard protocol securing HTTPS — uses ephemeral Diffie-Hellman for forward secrecy, AES-GCM or ChaCha20-Poly1305 for encryption, ECDSA/EdDSA for authentication
- **Certificate authorities (CA):** Hierarchical trust model — browsers trust ~100-150 root CAs; Let's Encrypt has issued 4+ billion certificates (free, automated)
- **Forward secrecy:** Compromise of long-term key does NOT reveal past session keys — achieved by using ephemeral DH keys for each session
- **Signal Protocol (2013):** Double Ratchet algorithm by Moxlin Marlinspike — provides forward secrecy AND post-compromise security; used by Signal, WhatsApp, Google Messages

---

## 2. CREDIBLE CLAIMS (Tier 2 — Academic / Debated but Supported)

### 2.1 Post-Quantum Cryptography
- **Quantum threat:** Shor's algorithm (1994) breaks RSA, ECC, Diffie-Hellman in polynomial time on a sufficiently large quantum computer — factoring and discrete log become easy
- **NIST PQC standards (August 2024):** Three algorithms standardized: ML-KEM (CRYSTALS-Kyber) for key encapsulation, ML-DSA (CRYSTALS-Dilithium) for digital signatures, SLH-DSA (SPHINCS+) for hash-based signatures
- **Lattice-based cryptography:** Security based on hardness of Learning with Errors (LWE) problem — believed resistant to quantum attacks; Regev (2005) gave worst-case to average-case reduction
- **Timeline:** Large-scale quantum computers may be 10-30 years away — but "harvest now, decrypt later" attacks mean sensitive data encrypted today needs post-quantum protection now
- **Hybrid approach:** Many organizations deploying hybrid classical + post-quantum cryptography during transition period

### 2.2 Zero-Knowledge Proofs
- **Definition (Goldwasser, Micali, Rackoff, 1989):** Prover convinces verifier that a statement is true without revealing ANY information beyond the statement's truth — Turing Award 2012
- **Example:** Prove you know a graph coloring without revealing the coloring — interactive protocol with soundness and zero-knowledge properties
- **zk-SNARKs:** Zero-Knowledge Succinct Non-Interactive Arguments of Knowledge — used in Zcash cryptocurrency for private transactions; trusted setup required
- **zk-STARKs:** Transparent (no trusted setup), post-quantum secure — larger proofs but stronger security assumptions
- **Applications beyond cryptocurrency:** Identity verification, credential systems, supply chain audits, regulatory compliance without data exposure

### 2.3 Homomorphic Encryption
- **Concept:** Compute on encrypted data without decrypting — Enc(a) ⊕ Enc(b) = Enc(a+b); enables cloud computation on private data
- **Gentry (2009):** First fully homomorphic encryption (FHE) scheme — based on lattice problems; groundbreaking but initially ~10⁹ times slower than plaintext computation
- **Current state:** ~1000-10000× overhead for practical FHE (2024) — improving rapidly; used in limited medical/financial applications
- **Partial schemes:** Faster but limited operations — ElGamal (multiplicatively homomorphic), Paillier (additively homomorphic)

---

## 3. SPECULATIVE CLAIMS (Tier 3 — Possible but Unverified)

### 3.1 P = NP and Cryptography
- If P = NP, most public-key cryptography would be broken — factoring, discrete log, and lattice problems would all be polynomial-time solvable
- Most computer scientists believe P ≠ NP — but this is unproven; the most important open problem in computer science ($1 million Millennium Prize)
- Even if P ≠ NP, specific cryptographic assumptions could still fail — the hardness of factoring, for instance, is not known to be NP-complete

### 3.2 Quantum Key Distribution (QKD)
- **BB84 protocol (Bennett, Brassard, 1984):** Uses quantum properties (no-cloning theorem) to distribute keys with information-theoretic security — eavesdropping is detectable
- **Practical challenges:** Distance limitations (~100-300 km fiber), photon loss, side-channel attacks, trusted nodes required for longer distances
- **Quantum internet:** Satellite-based QKD (Micius satellite, 2017) — China demonstrated 1200 km QKD; quantum repeaters needed for global scale

---

## 4. DUBIOUS CLAIMS (Tier 4 — No Credible Source / Contradicted by Evidence)

### 4.1 "Quantum Computers Will Break All Encryption"
- **[MISLEADING]** Shor's algorithm threatens RSA/ECC specifically; symmetric encryption (AES-256) remains secure against known quantum attacks (Grover's algorithm only halves effective key length, so AES-256 → AES-128 equivalent, still secure); post-quantum algorithms are already standardized

### 4.2 "Encryption Backdoors Can Be Made Safe"
- **[REJECTED BY MAINSTREAM]** Cryptographers universally warn that encryption backdoors inevitably weaken security for ALL users — the 2020 Juniper Networks backdoor incident demonstrated this; a backdoor inserted by one entity was exploited by another

---

## IMAGES

| # | Description | Filename | Source | License |
|---|-------------|----------|--------|---------|
| 1 | Diagram of public-key encryption and digital signature flow | — | — | — |

---

## BIBLIOGRAPHY

1. Katz, J. and Lindell, Y. *Introduction to Modern Cryptography.* 3rd ed., CRC Press, 2021.
2. Rivest, R. L., Shamir, A., and Adleman, L. "A Method for Obtaining Digital Signatures and Public-Key Cryptosystems." *Communications of the ACM*, vol. 21, 1978, pp. 120–126.
3. Diffie, W. and Hellman, M. E. "New Directions in Cryptography." *IEEE Transactions on Information Theory*, vol. 22, 1976, pp. 644–654.
4. Shor, P. W. "Polynomial-Time Algorithms for Prime Factorization and Discrete Logarithms on a Quantum Computer." *SIAM Journal on Computing*, vol. 26, 1997, pp. 1484–1509.
5. Gentry, C. "Fully Homomorphic Encryption Using Ideal Lattices." *Proceedings of the 41st ACM Symposium on Theory of Computing*, 2009, pp. 169–178.
6. Goldwasser, S., Micali, S., and Rackoff, C. "The Knowledge Complexity of Interactive Proof Systems." *SIAM Journal on Computing*, vol. 18, 1989, pp. 186–208.
7. Shannon, C. E. "Communication Theory of Secrecy Systems." *Bell System Technical Journal*, vol. 28, 1949, pp. 656–715.
8. Regev, O. "On Lattices, Learning with Errors, Random Linear Codes, and Cryptography." *Journal of the ACM*, vol. 56, 2009, pp. 1–40.
9. NIST. "Module-Lattice-Based Key-Encapsulation Mechanism Standard." FIPS 203, August 2024.
10. Bernstein, D. J. and Lange, T. "Post-Quantum Cryptography." *Nature*, vol. 549, 2017, pp. 188–194.

---

## CROSS-REFERENCE INDEX

| Related Doc | Connection |
|-------------|-----------|
| [V22 — Number Theory](../V_Mathematics_Information/V22_Number_Theory_Primes_Patterns.md) | RSA depends on prime factorization hardness; modular arithmetic underlies all public-key crypto |
| V08 — Information Theory | Shannon proved one-time pad security; entropy measures key quality |
| N06 — Codes and Ciphers | Historical cipher systems — Enigma, Caesar, Vigenère — precursors to modern cryptography |
| [ZA06 — Quantum Entanglement](../ZA_Physics_Quantum/ZA06_Quantum_Entanglement_Nonlocality.md) | QKD uses quantum entanglement for provably secure key distribution |
| S07 — AI/ML | AI-driven cryptanalysis; privacy-preserving ML via homomorphic encryption |

---

*New research document — Phase 9 expansion. Last Updated: Mar 07, 2026*
