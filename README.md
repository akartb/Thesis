# Research Papers in Theoretical Cosmology, Computational Complexity, Analytic Number Theory, and Computational Neuroscience

This repository contains a series of original academic research papers spanning four core fields of theoretical science and engineering: **theoretical cosmology & quantum gravity**, **computational complexity theory**, **analytic number theory & random matrix theory**, and **computational neuroscience & deep learning**.

All works include complete rigorous mathematical proofs, large-scale numerical experiments, standardized academic references, and testable theoretical predictions/conjectures, fully conforming to the normative requirements of professional academic research.

---

## Paper Catalog & Core Contributions

### 1. From Causal Spin Networks to Cyclic Cosmology: A Research Program with a Solvable Phenomenological Core
**Field**: Theoretical Cosmology, Quantum Gravity, Dark Energy Physics

**Core Topic**: Constructs a fully solvable cyclic cosmological model driven by a regular scalar field with an n=4 hilltop potential, and establishes a research roadmap linking the model to underlying causal spin network dynamics.

**Key Results**:
- Derived the complete background dynamics of the universe (expansion, turnaround, contraction, non-singular bounce) with a robust total cycle period of ~192.5 Gyr, and a predicted cosmic turnaround time of 48.6 Gyr from the present epoch.
- Obtained a dark energy equation of state prediction of $w_0=-0.9965$, $w_a \approx -0.002$, which is fully consistent with current cosmological observations and testable by Euclid, Roman, and CMB-S4 experiments.
- Provided quantum gravity physical motivation for the hilltop potential form via marginal stability argument at the loop quantum cosmology (LQC) bounce, effective field theory truncation, and discrete causal set compatibility.
- Diagnosed the primordial perturbation spectrum challenge of the cyclic model, and identified the matter-dominated contraction phase with isocurvature conversion as the most promising resolution path.

---

### 2. Boundary Analysis of the P vs NP Problem: Conditional Equivalence Under the Solution-Verification Complexity (k/z) Model
**Field**: Theoretical Computer Science, Computational Complexity Theory

**Core Topic**: Establishes a rigorous formal framework of solution complexity $k(n)$ and verification complexity $z(n)$ for the P vs NP problem, systematically refutes naive proof fallacies, and formalizes the conditional equivalence principle of P vs NP.

**Key Results**:
- Rigorously formalized the $k(n)/z(n)$ complexity framework without circular presuppositions and implicit assumptions, and defined the precondition consistency principle for valid P vs NP analysis.
- Systematically proved the logical invalidity of naive $k/z$-type $P \neq NP$ proofs, identifying three fatal fallacies: confusion between algorithmic upper bound and problem intrinsic lower bound, circular reasoning, and violation of precondition consistency.
- Restated the three fundamental proof barriers (relativization, natural proofs, algebrization) in the $k/z$ framework, and clarified the absolute proof-theoretic boundaries of intuitive growth-rate analysis methods.
- Formalized the core conditional equivalence principle: the relationship between P and NP is strictly determined by the underlying computational preconditions (computational model, resource constraints, axiomatic system). Rigorous separation and collapse theorems of $k(n)$ and $z(n)$ under different computational models are provided.

---

### 3. On the Spectral Structure of Sinc-Kernel Matrices on the Primes: Effective Rank, Geometric Decay, and Frequency-Box Decomposition
**Field**: Analytic Number Theory, Random Matrix Theory, Mathematical Physics

**Core Topic**: Introduces and analyzes a family of real symmetric matrices determined entirely by prime numbers with a sinc kernel, and establishes a complete spectral theory for this class of arithmetic matrices.

**Key Results**:
- Proved the core main theorem: for any fixed $\epsilon > 0$, the effective rank of the sinc-kernel prime matrix satisfies $\text{rank}_{\epsilon}(G_N) = \Theta(\log N)$, via two independent rigorous arguments (Rayleigh-Ritz lower bound and Slepian-Landau-Pollak upper bound).
- Proved that the eigenvectors corresponding to the top $\Theta(\log N)$ eigenvalues are exponentially localized on the frequency boxes, via diagonal dominance analysis and the Davis-Kahan sin $\Theta$ theorem.
- Developed the frequency-box decomposition method for arithmetic matrices on the primes, which provides a general tool for the spectral analysis of multiplicative arithmetic structures.
- Large-scale numerical experiments (up to $N=5000$) revealed that the full spectrum exhibits geometric decay with a universal ratio $r^* \approx 1.94$, and the nearest-neighbor level-spacing statistics are consistent with the Gaussian Orthogonal Ensemble (GOE).
- Proposed the arithmetic injection barrier conjecture, and verified that multiplicative arithmetic factors systematically destroy the Wigner-Dyson universality of the spectrum.

---

### 4. Non-Convolution Arithmetic Matrices on the Primes: Breaking the Effective-Rank Barrier and Non-Universal Spectral Statistics
**Field**: Analytic Number Theory, Random Matrix Theory, Additive Number Theory

**Core Topic**: Constructs a non-convolution arithmetic matrix based on the von Mangoldt function on prime sums, breaks the $O(\log N)$ effective-rank barrier of convolution kernels, and discovers a novel intermediate spectral statistic beyond standard Wigner-Dyson universality classes. This work is a follow-up and breakthrough of the sinc-kernel matrix research.

**Key Results**:
- Rigorously proved the non-separability and non-convolution property of the $\Lambda$-kernel matrix defined by $K_{ij} = \Lambda(p_i + p_j) / \log(p_i + p_j)$, which fundamentally breaks the bandwidth constraint of convolution-type kernels.
- Numerically verified that the positive eigenvalue count of the $\Lambda$-kernel matrix is $\Theta(N)$, achieving an 18-fold increase in effective rank at $N=2000$ compared to the sinc-kernel matrix, decisively breaking the $O(\log N)$ effective-rank barrier.
- Designed a four-fold control experiment system with an unfolding-free Oganesyan-Huse spacing ratio statistic, and rigorously decomposed the spectral anomaly: non-negativity and sparsity contribute 65% of the total anomaly, while the discrete value set of the von Mangoldt function contributes 35% (95% statistically significant).
- Proved the unitary equivalence barrier theorem: product-type complex phases (e.g., Dirichlet characters) leave all eigenvalues and spacing statistics invariant, precluding such strategies from steering the universality class of the spectrum.
- Discovered a novel "arithmetic intermediate state" spectral statistic, whose small-spacing suppression lies between GOE and GUE, without conforming to any standard Wigner-Dyson universality class, expanding the theoretical boundary of random matrix universality.

---

### 5. H-EVA: A Predictive Coding Architecture with Verified Equivalence to Backpropagation
**Field**: Computational Neuroscience, Deep Learning, Edge AI

**Core Topic**: Implements a rigorous predictive coding (PC) architecture that strictly follows the theoretical mathematical formulation from foundational literature, identifies and corrects five critical implementation bugs in existing PC networks, and empirically verifies the theoretical equivalence between PC learning and backpropagation (BP).

**Key Results**:
- Systematically identified and corrected five fatal implementation bugs in practical PC networks, including incorrect feedback derivative placement, pre-activation staleness in inference loops, and error-value inconsistency after inference convergence, resolving the long-standing divergence and convergence failure problem in real-world PC implementations.
- Provided the first systematic three-mode full-dimensional comparison: BP training + BP inference, BP training + PC inference, and PC learning + PC inference, covering both function regression and digit classification tasks.
- Empirically verified the Whittington & Bogacz (2017) equivalence theorem: PC learning with sufficient inference iterations achieves identical accuracy to BP (97.78% on digit classification), completing the end-to-end practical validation of the theoretical result.
- Rigorously proved that layer-local Adam optimization preserves the spatial locality of PC learning rules, resolving the long-standing academic controversy on whether adaptive optimizers violate the biological plausibility and locality principle of PC.
- Demonstrated that pure SGD-based PC learning fails to converge within 2000 epochs (MSE=0.027 on Sin fitting), establishing that adaptive optimization is essential for practical PC convergence.
- All experiments run natively on CPU without GPU acceleration, verifying the feasibility of PC for resource-constrained edge-device AI deployment.

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
└── 05-heva-predictive-coding
    └── heva_predictive_coding_bp_equivalence.pdf
```

---

## Citation

If you use the methods, results, or code from these works in your research, please cite the corresponding paper via the permanent DOI:

```
[DOI will be updated after Zenodo archive release]
```

---

## Academic Communication

For academic discussions, feedback, or collaboration requests, please open an Issue in this repository, or contact via the email address provided in the papers.
