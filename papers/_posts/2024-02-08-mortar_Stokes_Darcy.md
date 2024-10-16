---
title: A mortar method for Stokes-Darcy problems
header: 
  teaser: /assets/images/papers/heterogeneous.png
  overlay_image: /assets/images/papers/heterogeneous.png
excerpt: A mortar method for the coupled Stokes-Darcy problem using the MAC scheme for Stokes and mixed finite elements for Darcy
authors: W.M. Boon, D. Gläser, R. Helmig, K. Weishaupt, I. Yotov
journal: Computational Geosciences 28, 413–430
tags: 
    - Stokes-Darcy
    - MiDiROM
---

[Published version](https://doi.org/10.1007/s10596-023-10267-6){: .btn .btn--info}
[ArXiv (open access)](https://arxiv.org/abs/2402.10615){: .btn .btn--success}

## Summary
- We discretize the Stokes equations with the Marker-and-Cell (MAC) method and Darcy flow using the Raviart-Thomas pair.
- We analyze the MAC scheme by interpreting it as a conforming mixed finite element method on a staggered grid.
- The two schemes are coupled by introducing a Lagrange multiplier on the Stokes-Darcy interface that enforces flux continuity.
- We show that the discrete system is well-posed and provide a priori error estimates.
- The analytical results are validated by three numerical test cases.