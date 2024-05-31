---
title: Mixed finite element methods for linear Cosserat equations
header: 
  teaser: /assets/images/papers/superconvergence_k1_example_1.png
  overlay_image: /assets/images/papers/superconvergence_k1_example_1.png
excerpt: Mixed finite element methods for linear Cosserat equations
authors: W.M. Boon, O. Durán, J.M. Nordbotten
journal: 
tags: 
    - Cosserat
    - differential complexes
---

<!-- [Published version](){: .btn .btn--info} -->
[ArXiv (open access)](https://arxiv.org/abs/2403.15136){: .btn .btn--success}

## Key ideas
- Cosserat materials form an extension of linearized elasticity by relaxing the symmetry condition on the stress tensor. 
- With the additional rotation and couple stress variables, the Cosserat equations form a saddle point problem in four variables.

## Main findings
- The operators in the Cosserat equations can be placed in a differential complex that is isomorphic to six copies of the de Rham complex.
- The Cosserat equations correspond to a well-posed Hodge-Laplace problem.
- Two families of mixed finite element discretizations are proposed:
  * The *strongly coupled* spaces form a subcomplex.
  * The *weakly coupled* spaces can be used if the equations degenerate to linearized elasticity.
- Optimal convergence is shown theoretically and numerically for both families.