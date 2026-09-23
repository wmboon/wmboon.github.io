---
title: Domain Decomposition for Richards' flow in mixed form
header: 
  teaser: assets/images/papers/watertable_T_0.22.png
  overlay_image: assets/images/papers/watertable_T_0.22.png
excerpt: Linear Robin-type Domain Decomposition scheme for Mixed Formulation of Richards' Equation
authors: Å.v.B. Synnevåg, W.M. Boon, F.A. Radu, S.E. Gasda
journal: 
tags: 
    - domain decomposition
    - water table
---

<!-- [Published version](){: .btn .btn--info} -->
[ArXiv (open access)](https://arxiv.org/abs/2609.26478){: .btn .btn--success}

## Summary

- **A new domain-decomposition scheme for heterogeneous Richards' equation flow.** We introduce the mLRDD-scheme, combining non-overlapping domain decomposition, L-scheme linearization, and mixed finite elements to solve Richards' equation across domains with sharply contrasting materials, splitting the problem along material interfaces via a Robin-type coupling condition.

- **Convergence is rigorously proved.** Under mild conditions on the timestep, stabilization parameter, and Robin parameter, we show convergence of flux, saturation, and pressure, with continuity of flux and pressure recovered across interfaces in the limit.

- **Numerical results show robustness and performance gains over monolithic solvers.** 2D and 3D tests (including a realistic multi-material benchmark) confirm first-order convergence and show the mLRDD-scheme is more robust than monolithic Newton/Picard methods, with parallelization giving substantial runtime savings on larger, more heterogeneous problems.