---
title: Mixed finite element methods for linear Cosserat equations
header: 
  teaser: /assets/images/papers/superconvergence_k1_example_1.png
  overlay_image: /assets/images/papers/superconvergence_k1_example_1.png
excerpt: Mixed finite element methods for linear Cosserat equations
authors: W.M. Boon, O. Durán, J.M. Nordbotten
journal: SIAM Journal on Numerical Analysis 63(1), 306-333
tags: 
    - Cosserat
    - differential complexes
---

[Published version (open access)](https://doi.org/10.1137/24M1648387){: .btn .btn--success}
[ArXiv](https://arxiv.org/abs/2403.15136){: .btn .btn--success}

## Key ideas
- Cosserat materials form an extension of linearized elasticity by relaxing the symmetry condition on the stress tensor. 
- With the additional rotation and couple stress variables, the Cosserat equations form a saddle point problem in four variables.
- The Cosserat equations correspond to a well-posed Hodge-Laplace problem on the Cosserat complex.

## Main findings
- Two families of mixed finite element discretizations are proposed:
  * The *strongly coupled* spaces form a subcomplex of the Cosserat complex.
  * The *weakly coupled* spaces can be used if the equations degenerate to linearized elasticity. They utilize tuples of $\mathbb{RT}_0$ for the stress tensors.
- Optimal convergence is shown theoretically and numerically for both families.