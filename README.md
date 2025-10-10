# Linear-Depth Multi-Controlled-U in Qiskit

This project implements a linear-depth, no-ancilla construction of an n-controlled unitary (CⁿU) gate based on  
**“Linear-Depth Decomposition of Multi-Controlled Unitary Operations”** ([arXiv:2203.11882](https://arxiv.org/abs/2203.11882)).

---

## Overview
Conventional multi-controlled-U gates scale quadratically in depth.  
This implementation achieves **O(n)** depth using two recursive components:
- **Pₙ(U):** sequence of controlled fractional-power unitaries `U^(1/2ᵏ)`
- **Qₙ:** chain of controlled `Rₓ(π / k)` rotations

Combined, they reproduce the full CⁿU without ancillas.

---
