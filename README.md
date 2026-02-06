# Asymptotic Convergence Bounds for Geometric Theorem Discovery Under Resource Constraints

[![Download PDF](https://img.shields.io/badge/Download-PDF-blue?logo=adobe-acrobat-reader)](https://github.com/ChicagoHAI/geom-theorem-bounds-29bf/releases/download/latest/paper.pdf) [![Build Status](https://github.com/ChicagoHAI/geom-theorem-bounds-29bf/actions/workflows/build-paper.yml/badge.svg)](https://github.com/ChicagoHAI/geom-theorem-bounds-29bf/actions)

> Proves that automated geometric theorem discovery requires O(n^3 log n) computational resources to find theorems of length n with high probability, establishing the first rigorous complexity bounds for this problem.

## Abstract

We establish fundamental complexity bounds for automated theorem discovery in geometric reasoning systems. Our main result proves that for any geometric theorem discovery system G operating in first-order logic with equality, there exists a complexity threshold T(n) = O(n^3 log n) such that allocating computational resources exceeding T(n) yields probability 1 - e^(-n) of discovering a novel theorem of statement length n as n → ∞. The proof introduces a measure-theoretic framework for analyzing the space of geometric statements and shows that heuristic search trajectories with algebraic verification form martingale sequences. By applying the Azuma-Hoeffding inequality and the method of moments, we demonstrate convergence to the claimed asymptotic behavior. We further prove this threshold is tight through explicit construction of adversarial statement spaces. Our results provide the first rigorous complexity bounds for automated geometric theorem discovery and establish fundamental limits on the computational resources required for reliable theorem generation. The techniques developed here extend to broader classes of formal reasoning systems and suggest a general framework for analyzing the complexity of automated mathematical discovery.

## Key Contributions

1. Existence of complexity threshold T(n) = O(n^3 log n) for geometric theorem discovery
2. Probability of theorem discovery approaches 1 - e^(-n) when resources exceed threshold
3. The complexity bound is tight through adversarial construction

## Key Results

| Result | Statement | Status |
|--------|-----------|--------|
| Theorem 1 | For any geometric theorem discovery system G using first-order logic with equality, there exists a complexity threshold ... | Complete |

## Methodology

**Main Claim:** For any geometric theorem discovery system G using first-order logic with equality, there exists a complexity threshold function T(n) = O(n^3 log n) such that if the computational resources allocated exceed T(n), the probability of discovering a novel theorem of statement length n approaches 1 - e^(-n) asymptotically

**Approach:** 1) Establish a measure-theoretic framework for the space of geometric statements
2) Prove that heuristic search with algebraic verification creates a martingale sequence
3) Apply the Azuma-Hoeffding inequality to bound deviation probabilities
4) Use the method of moments to show convergence to the claimed asymptotic behavior
5) Demonstrate that the threshold function T(n) is tight via adversarial construction

## Experiments

| # | Description | Status |
|---|-------------|--------|
| 1 | This experiment tests the theorem discovery complexity threshold by simulating g... | Simulated |



## Limitations

- Here are 4 specific limitations of this mathematical work:
- Scope Limitation: The result only applies to first-order logic with equality, excluding higher-order geometric reasoning systems that might use modal logic, temporal logic, or other formalisms necessa
- Computational Assumption: The proof assumes that algebraic verification of geometric statements can be performed within polynomial time, which may not hold for complex geometric constructions involvin
- Measure-Theoretic Restriction: The framework requires a well-defined measure over the space of geometric statements, but this may break down for statements involving arbitrary precision or continuous 
- Practical Resource Bounds: While the O(n^3 log n) complexity bound is polynomial, for real-world geometric theorems where n could be large (hundreds or thousands of logical symbols), the actual comput

## Topics

`computational-complexity` `automated-reasoning` `geometric-reasoning` `probability-theory` `measure-theory`

## Download PDF

The paper is automatically compiled on every push. Download the latest version:

**[Download paper.pdf](https://github.com/ChicagoHAI/geom-theorem-bounds-29bf/releases/download/latest/paper.pdf)**

Or build it locally:

```bash
cd paper_draft
make          # Builds main.pdf
```

## Research Artifacts

- [`REPORT.md`](REPORT.md) - Detailed findings and results analysis
- [`planning.md`](planning.md) - Research plan and proof strategy
- [`literature_review.md`](literature_review.md) - Literature survey and background
- [`experiments/`](experiments/) - Experiment code and results

## Repository Structure

```
.
├── paper_draft/
│   ├── main.tex          # Main LaTeX file
│   ├── references.bib    # Bibliography
│   ├── sections/         # Paper sections
│   │   ├── abstract.tex      # Problem, approach, results summary
│   │   ├── introduction.tex      # Motivation, hypotheses, contributions
│   │   ├── background.tex      # Related work and preliminaries
│   │   ├── methodology.tex      # Approach, algorithms, analysis setup
│   │   ├── results.tex      # Theorems, proofs, experiments
│   │   ├── discussion.tex      # Interpretation and implications
│   │   ├── limitations.tex      # Limitations and future work
│   │   └── conclusion.tex      # Summary and takeaways
│   └── commands/         # LaTeX macros
│       ├── math.tex
│       └── macros.tex
├── REPORT.md             # Key findings and results
├── planning.md           # Research plan
├── literature_review.md  # Literature survey
├── experiments/          # Experiment code and results
├── .github/workflows/    # Automatic PDF compilation
├── README.md
└── .math-agent/          # Generation metadata
```

## Reproducing Results

```bash
# Build the paper
cd paper_draft
make

# Run experiments (requires Python 3)
cd ../experiments
python experiment_1.py
```

## Generated by

This paper was autonomously generated by the [Scibook Math Agent](https://scibook.ai).



---

*Generated on 2026-02-06*
