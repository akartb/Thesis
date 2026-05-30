# Research Papers in Theoretical Cosmology, Computational Complexity, Analytic Number Theory, and Computational Neuroscience

**Permanent DOI for Originality Proof (v1.7 Latest)**: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.20020716.svg)](https://doi.org/10.5281/zenodo.20020716)

This repository contains a series of original academic research papers spanning four core fields of theoretical science: **theoretical cosmology & quantum gravity**, **computational complexity theory**, **analytic number theory & random matrix theory**, and **computational neuroscience & deep learning**.

All works include complete rigorous mathematical proofs, large-scale numerical experiments, standardized academic references, and testable theoretical predictions/conjectures, fully conforming to the normative requirements of professional academic research.

---

## Version Update Note (v1.7)

This is the v1.7 update. Changes from v1.6:
- **Paper 3 revised**: geometric decay of sinc-kernel eigenvalues is now rigorously proved as Theorem 4.2 (previously a conjecture), with expanded exposition.
- **Paper 10 added**: a new paper on negation-limited monotone circuit lower bounds for the CLIQUE function, extending Razborov's framework to circuits with up to c log n NOT gates.
- All papers remain fully anonymized with cleaned metadata.

- v1.0 Permanent DOI: 10.5281/zenodo.20020716
- v1.7 Full Archive: https://doi.org/10.5281/zenodo.20020716

---

## Paper Catalog & Core Contributions

### 1. From Causal Spin Networks to Cyclic Cosmology: A Research Program with a Solvable Phenomenological Core
**Field**: Theoretical Cosmology, Quantum Gravity, Dark Energy Physics

**Core Topic**: Constructs a fully solvable cyclic cosmological model driven by a regular scalar field with an n=4 hilltop potential, and establishes a research roadmap linking the model to underlying causal spin network dynamics.

**Key Results**:
- Derived the complete background dynamics of the universe (expansion, turnaround, contraction, non-singular bounce) with a robust total cycle period of ~192.5 Gyr, and a predicted cosmic turnaround time of 48.6 Gyr from the present epoch.
- Obtained a dark energy equation of state prediction of w₀ = −0.9965, wₐ ≈ −0.002, which is fully consistent with current cosmological observations and testable by Euclid, Roman, and CMB-S4 experiments.
- Provided quantum gravity physical motivation for the hilltop potential form via marginal stability argument at the loop quantum cosmology (LQC) bounce, effective field theory truncation, and discrete causal set compatibility.
- Diagnosed the primordial perturbation spectrum challenge of the cyclic model, and identified the matter-dominated contraction phase with isocurvature conversion as the most promising resolution path.

---

### 2. Boundary Analysis of the P vs NP Problem: Conditional Equivalence Under the Solution-Verification Complexity (k/z) Model
**Field**: Theoretical Computer Science, Computational Complexity Theory

**Core Topic**: Establishes a rigorous formal framework of solution complexity k(n) and verification complexity z(n) for the P vs NP problem, systematically refutes naive proof fallacies, and formalizes the conditional equivalence principle.

**Key Results**:
- Rigorously formalized the k(n)/z(n) complexity framework without circular presuppositions, and defined the precondition consistency principle for valid P vs NP analysis.
- Systematically proved the logical invalidity of naive k/z-type P ≠ NP proofs, identifying three fatal fallacies: confusion between algorithmic upper bound and problem intrinsic lower bound, circular reasoning, and violation of precondition consistency.
- Restated the three fundamental proof barriers (relativization, natural proofs, algebrization) in the k/z framework, clarifying the absolute proof-theoretic boundaries of intuitive growth-rate analysis.
- Formalized the core conditional equivalence principle: the relationship between P and NP is strictly determined by the underlying computational preconditions (computational model, resource constraints, axiomatic system). Rigorous separation and collapse theorems under different computational models are provided.

---

### 3. On the Spectral Structure of Sinc-Kernel Matrices on the Primes: Effective Rank, Geometric Decay, and Frequency-Box Decomposition *(Revised)*
**Field**: Analytic Number Theory, Random Matrix Theory, Mathematical Physics

**Core Topic**: Introduces and analyzes a family of real symmetric matrices determined entirely by prime numbers with a sinc kernel, and establishes a complete spectral theory for this class of arithmetic matrices. This revision upgrades the geometric decay from a numerical observation to a rigorous theorem.

**Key Results**:
- Proved the core main theorem: for any fixed ε > 0, the effective rank of the sinc-kernel prime matrix satisfies rank_ε(G_N) = Θ(log N), via two independent rigorous arguments (Rayleigh-Ritz lower bound and Slepian-Landau-Pollak upper bound).
- Proved that the eigenvectors corresponding to the top Θ(log N) eigenvalues are exponentially localized on the frequency boxes, via diagonal dominance analysis and the Davis-Kahan sin Θ theorem.
- **New**: Rigorously proved geometric decay of the leading Θ(log N) eigenvalues (Theorem 4.2): there exists an absolute constant r > 1 such that λ_k/λ_{k+1} ≥ r for all k = 1, ..., K−1. Numerical experiments (up to N=5000) confirm the universal ratio r* ≈ 1.94.
- Developed the frequency-box decomposition method for arithmetic matrices on the primes, providing a general tool for spectral analysis of multiplicative arithmetic structures.
- Large-scale numerical experiments show the nearest-neighbor level-spacing statistics are consistent with the Gaussian Orthogonal Ensemble (GOE).
- Proposed the arithmetic injection barrier conjecture, and verified that multiplicative arithmetic factors systematically destroy the Wigner-Dyson universality of the spectrum.

---

### 4. Non-Convolution Arithmetic Matrices on the Primes: Breaking the Effective-Rank Barrier and Non-Universal Spectral Statistics
**Field**: Analytic Number Theory, Random Matrix Theory, Additive Number Theory

**Core Topic**: Constructs a non-convolution arithmetic matrix based on the von Mangoldt function on prime sums, breaks the O(log N) effective-rank barrier of convolution kernels, and discovers a novel intermediate spectral statistic beyond standard Wigner-Dyson universality classes.

**Key Results**:
- Rigorously proved the non-separability and non-convolution property of the Λ-kernel matrix, fundamentally breaking the bandwidth constraint of convolution-type kernels.
- Numerically verified that the positive eigenvalue count is Θ(N), achieving an 18-fold increase in effective rank at N=2000 compared to the sinc-kernel matrix.
- Designed a four-fold control experiment system with the unfolding-free Oganesyan-Huse spacing ratio statistic, and rigorously decomposed the spectral anomaly: non-negativity and sparsity contribute 65% of the total anomaly, while the discrete value set of the von Mangoldt function contributes 35% (95% statistically significant).
- Proved the unitary equivalence barrier theorem: product-type complex phases leave all eigenvalues and spacing statistics invariant, precluding such strategies from steering the universality class.
- Discovered a novel "arithmetic intermediate state" spectral statistic, whose small-spacing suppression lies between GOE and GUE, expanding the theoretical boundary of random matrix universality.

---

### 5. H-EVA: A Predictive Coding Architecture with Verified Equivalence to Backpropagation
**Field**: Computational Neuroscience, Deep Learning, Edge AI

**Core Topic**: Implements a rigorous predictive coding (PC) architecture that strictly follows the theoretical mathematical formulation from foundational literature, identifies and corrects five critical implementation bugs, and empirically verifies the theoretical equivalence between PC learning and backpropagation (BP).

**Key Results**:
- Systematically identified and corrected five fatal implementation bugs in practical PC networks, including incorrect feedback derivative placement, pre-activation staleness in inference loops, and error-value inconsistency after inference convergence.
- Provided the first systematic three-mode full-dimensional comparison: BP training + BP inference, BP training + PC inference, and PC learning + PC inference, covering both function regression and digit classification tasks.
- Empirically verified the Whittington & Bogacz (2017) equivalence theorem: PC learning with sufficient inference iterations achieves identical accuracy to BP (97.78% on digit classification).
- Rigorously proved that layer-local Adam optimization preserves the spatial locality of PC learning rules, resolving the long-standing academic controversy on whether adaptive optimizers violate the biological plausibility and locality principle of PC.
- Demonstrated that pure SGD-based PC learning fails to converge within 2000 epochs (MSE=0.027 on Sin fitting), establishing that adaptive optimization is essential for practical PC convergence.
- All experiments run natively on CPU without GPU acceleration, verifying the feasibility of PC for resource-constrained edge-device AI deployment.

---

### 6. Spectral Statistics of Deterministic Arithmetic Prime Matrices: A Phase Diagram from GOE to Poisson
**Field**: Analytic Number Theory, Random Matrix Theory, Additive Number Theory

**Core Topic**: Systematically studies five core arithmetic kernels (sinc, divisor d, Liouville λ, Möbius μ, von Mangoldt Λ) in the three-dimensional parameter space of density, sign structure, and value discreteness, and maps the first complete phase diagram of spectral statistics for deterministic arithmetic prime matrices.

**Key Results**:
- Discovered that sparsity is the dominant tuning parameter for spectral universality classes: ⟨r̃⟩ decreases monotonically from GOE (ρ=1) to a compressed state (ρ≈0.0008).
- Provided strong new numerical evidence for an additive version of the Chowla conjecture: the Liouville λ matrix on prime sums is the only tested construction that simultaneously passes both local (GOE spacing statistics) and global (semicircle moment ratio κ→2) GOE tests.
- Verified through full control experiments that none of the tested deterministic arithmetic constructions achieve GUE statistics, proposing an empirical boundary conjecture for the inaccessibility of GUE within this framework.
- Perfected the complete spectral analysis methodology for deterministic arithmetic prime matrices, providing a new research perspective for the Hilbert-Pólya conjecture.

---

### 7. From Semicircle to Sato-Tate: Moment Convergence, Hecke Angle Statistics, and the Dimension of S₂₄(SL₂(Z))
**Field**: Analytic Number Theory, Random Matrix Theory, Automorphic Forms

**Core Topic**: Extends the asymptotic arithmetic spectral geometry program from finite-dimensional matrix ensembles toward the automorphic world via three complementary results: the semicircle law, Sato-Tate statistics, and the dimension of S₂₄.

**Key Results**:
- Proved that the standardized moments of the Liouville kernel on prime sums converge to the Catalan numbers for all even orders up to m₁₂ (κ₄=1.990, κ₆=4.963, κ₈=13.323 at N=4000), and formulated a conditional theorem linking this convergence to the additive Chowla conjecture.
- Verified that Hecke eigenvalues of the Ramanujan Δ function for all 109 primes p≤599 confirm the Sato-Tate law (KS p=0.64) and reject uniformity (p=0.0003), with zero Ramanujan bound violations.
- Proved that S₂₄(SL₂(Z)) has dimension 3 (not 2 as given by the standard formula), establishing linear independence of the three forms Δ·E₄³, Δ·E₄·E₆, Δ·E₆² via SVD rank verification.

---

### 8. From Sato-Tate to Wigner-Dyson: Emergent Level Repulsion in Families of Hecke Operators
**Field**: Analytic Number Theory, Random Matrix Theory, Automorphic Forms

**Core Topic**: Reports the first numerical observation of a monotonic transition in the spectral statistics of Hecke operator families across increasing dimensions of cusp form spaces, from Sato-Tate toward GOE universality.

**Key Results**:
- Discovered a monotonic evolution of the angle spacing ratio ⟨r̃⟩ from 0.326 (Sato-Tate, k=12, d=1) through 0.384 (Poisson, k=28, d=3) to 0.467 (GOE transition, k=36, d=4), a +0.14 increase consistent with the Katz-Sarnak prediction of emergent level repulsion.
- Formulated a conditional theorem reducing the convergence to GUE to a decorrelation hypothesis on Hecke eigenvalues in high-dimensional spaces.
- Provided the first systematic numerical evidence for the dimensional emergence of random matrix universality in automorphic spectral statistics, bridging the Sato-Tate and Wigner-Dyson regimes.

---

### 9. Direct Spacing Ratio Computation for Zeros of the Riemann Zeta and Ramanujan τ L-Functions
**Field**: Analytic Number Theory, Random Matrix Theory, Computational Number Theory

**Core Topic**: Computes nearest-neighbor spacing ratios for zeros of the Riemann zeta function and the Ramanujan τ L-function using the lcalc engine within SageMath, providing a fully reproducible benchmark with complete uncertainty quantification.

**Key Results**:
- For the first 200 zeros of the Riemann zeta function, the spacing ratio is r̃ = 0.615 ± 0.012, consistent with the GUE theoretical value 0.602 given finite-size effects.
- For the first 500 zeros of the Ramanujan τ L-function, obtained r̃ = 0.646 ± 0.008, which is 5.8 standard errors above GUE — a preliminary observation requiring independent verification.
- Provided the complete code, the first 10 zeros for cross-validation, and a detailed uncertainty analysis.
- Cautioned that the elevated τ L-function result may reflect computational limitations, finite-size effects, or systematic bias in the lcalc implementation.
- Established a transparent, reproducible pipeline for spacing ratio computation that facilitates independent cross-validation with PARI/GP, Mathematica, or custom high-precision tools.

---

### 10. Negation-Limited Monotone Circuits for CLIQUE: A Simple Proof of Strong Lower Bounds
**Field**: Theoretical Computer Science, Circuit Complexity, Computational Complexity Theory

**Core Topic**: Revisits the monotone circuit complexity of the CLIQUE function, proving that Razborov's exponential lower bound remains valid even when the circuit is allowed up to c·log n negation (NOT) gates — a simpler proof handling a strictly larger range than prior work.

**Key Results**:
- Proved that any circuit for CLIQUE(n, k) containing at most c·log n NOT gates requires at least n^{Ω(√k)} AND/OR gates, via a direct extension of Razborov's approximation framework.
- The key insight: each NOT gate introduces an error of at most O(|X| + |Y|), while Razborov's threshold is Q = |X| · |Y|; the exponential gap between Q and |X| + |Y| allows logarithmically many negations without affecting the asymptotic bound.
- Improved upon the prior result of Amano and Maruoka (2005), which handled only (1/6)·log log n NOT gates via a delicate layer-by-layer induction, by a simpler, cruder — but asymptotically sufficient — error analysis.
- Provided a step-by-step manual verification of Razborov's approximator construction on a minimal CLIQUE instance (n = 5, k = 3) as a pedagogical illustration.
- Provided an explicit Karchmer-Wigderson game for the same parameters, demonstrating the communication-complexity perspective on monotone depth lower bounds.

---

## Repository Structure

```
.
├── README.md
├── 01-cyclic-cosmology
│   └── cyclic_hilltop_quintessence.pdf
├── 02-p-vs-np-boundary-analysis
│   └── p_vs_np_kz_model_analysis.pdf
├── 03-sinc-kernel-prime-matrices
│   └── sinc_kernel_primes_spectral_structure.pdf
├── 04-non-convolution-prime-arithmetic-matrices
│   └── non_convolution_lambda_kernel_primes.pdf
├── 05-heva-predictive-coding
│   └── heva_predictive_coding_bp_equivalence.pdf
├── 06-arithmetic-matrix-phase-diagram
│   └── spectral_statistics_prime_matrices_phase_diagram.pdf
├── 07-semicircle-to-sato-tate
│   └── semicircle_sato_tate_moment_convergence_hecke.pdf
├── 08-sato-tate-to-wigner-dyson
│   └── sato_tate_wigner_dyson_hecke_repulsion.pdf
├── 09-zeta-tau-spacing-ratios
│   └── zeta_tau_spacing_ratios.pdf
└── 10-negation-limited-clique
    └── negation_limited_clique.pdf
```

---

## Thematic Map

| Theme | Papers |
|-------|--------|
| Theoretical Cosmology & Quantum Gravity | 1 |
| Computational Complexity Theory | 2, 10 |
| Analytic Number Theory & Random Matrix Theory | 3, 4, 6, 7, 8, 9 |
| Computational Neuroscience & Deep Learning | 5 |

Papers 3–4 and 6–9 form a coherent research arc in analytic number theory: Papers 3–4 establish the spectral theory of deterministic arithmetic matrices; Paper 6 maps the full phase diagram across five kernels; Papers 7–8 extend the program to automorphic forms and Hecke operators; and Paper 9 provides a direct spacing-ratio benchmark for classical L-function zeros. Papers 2 and 10 are complementary works in computational complexity: Paper 2 addresses the P vs NP problem through the k/z framework, while Paper 10 provides concrete circuit lower bounds for the CLIQUE function under limited negation.

---

## Citation

If you use the methods, results, or code from these works in your research, please cite the original collection via the permanent DOI:

```
Anonymous Author. (2026). Research Papers in Theoretical Cosmology, Computational Complexity,
Analytic Number Theory, and Computational Neuroscience (v1.7). Zenodo.
https://doi.org/10.5281/zenodo.20020716
```

---

## Academic Communication

For academic discussions, feedback, or collaboration requests, please open an Issue in this repository.
