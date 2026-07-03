
# Flavor Attractor Dynamics & Fermion Mass Convergence

This repository contains the rigorous numerical validation suite for our proposed theoretical framework, analyzing the emergence of fermion mass hierarchies through fixed-point attractor dynamics at the Higgs vacuum expectation value ($v^* = 246.22$ GeV).

## Overview
The code tracks the dynamic relaxation and structural stability of Yukawa matrices under optimized flavor-misalignment fields. It transitions from analytical formulations to concrete numerical proofs across a multi-generation field space.

## Key Components in `toust.ipynb`
* **Fermion Mass Convergence:** Computes first-principles Yukawa eigenvalues $Y_f^*$ to derive Standard Model quark and lepton masses, evaluating precise relative errors against experimental observables.
* **Spectral Certificate Engine:** Constructs a complete parameter Jacobian matrix system to evaluate eigenvalues ($\lambda_i$) and explicitly verify Lyapunov stability criteria ($\max(\text{Re}(\lambda_i)) < 0$).
* **Dynamical Relaxation Testing:** Implements a high-precision 4th-order Runge-Kutta integration loop (`rk4_step`) to track out-of-equilibrium trajectory decay and ensure basin robustness against non-equilibrium perturbations.
* **Geometric Stiffness Alignment:** Isolates stationary geometric phases, optimizing effective structural stiffness against target scales ($S^* \approx 1.6002$).

## Prerequisites
To run the notebook locally, ensure you have a standard Python environment with the following dependencies:
* `numpy`
* `scipy`
* `pandas`
