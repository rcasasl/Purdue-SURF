# Purdue-SURF – Fibonacci Anyon Quantum Gates

**Rafael Casas Lozano – SURF 2024, Purdue University**  
**Supervisor:** Prof. Shawn X. Cui

This repository contains the code developed during my **Summer Undergraduate Research Fellowship (SURF)** at Purdue University.  
The project studies **leakage-free entangling quantum gates in the Fibonacci anyon model**, using explicit matrix representations of the braid group generators.

## Project overview
**
The code:

- Implements the **F-** and **R-moves** for Fibonacci anyons using the golden ratio `φ`.
- Builds explicit matrix representations of the braid generators  
  \(\sigma_1, \dots, \sigma_5\) on a 5-dimensional fusion space.
- Verifies the **braid relations**  
  \(\sigma_i \sigma_{i+1} \sigma_i = \sigma_{i+1} \sigma_i \sigma_{i+1}\) and  
  \(\sigma_i \sigma_j = \sigma_j \sigma_i\) for \(|i-j| \ge 2\).
- Identifies a 4-dimensional **computational subspace** (two encoded qubits) and a
  leakage level corresponding to the 5th basis state.
- Provides:
  - `Leakagefree(U)`: checks whether a braid word `U` is leakage-free.
  - `Entangling(U)`: checks whether the induced 4×4 gate is genuinely entangling
    (up to local unitaries and SWAP).

At the end of the script, several example braid words are tested and the code
prints whether they are leakage-free and/or entangling.
**
