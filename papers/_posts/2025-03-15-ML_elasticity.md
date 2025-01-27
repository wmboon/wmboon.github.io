---
title: Momentum preserving neural network solvers for elasticity
header: 
  teaser: /assets/images/papers/quiver2j0_splitted_3.png
  overlay_image: /assets/images/papers/quiver2j0_splitted_3.png
excerpt: Neural network solvers for parametrized elasticity problems that conserve linear and angular momentum
authors: W.M. Boon, N.R. Franco, A. Fumagalli
journal: Computer Methods in Applied Mechanics and Engineering, 437, 117759
tags: 
    - neural networks
    - spanning trees
    - weak symmetry
---

[Published version (open access)](https://doi.org/10.1016/j.cma.2025.117759){: .btn .btn--success}
[ArXiv](https://arxiv.org/abs/2410.06975){: .btn .btn--success}

## Summary
- We consider the Arnold-Falk-Winther finite element triplet to discretize the stress, displacement, and rotation variables.
- Using a spanning tree, a *particular* solution $\sigma_f = Sf$ is rapidly constructed that balances body and boundary forces and is weakly symmetric.
- Since $S$ is a right-inverse of $B$, the operator $(I - SB)$ is a projection onto the kernel of $B$.
- Two strategies are proposed to update the particular solution with a *homogeneous* solution
    - A *Split* approach in which a neural network is trained to update the particular solution with $\tilde{\sigma}$, which is then projected onto the kernel of $B$:
    $$ \sigma = \sigma_f + (I - SB) \tilde{\sigma}$$
    - A *Corrected* strategy that trains a neural network to compute the stress directly as $\hat{\sigma}$ and we apply a correction:
    $$ \sigma = \sigma_f + (I - SB) (\hat{\sigma} - \sigma_f)$$
  In both cases, we have $B\sigma = B\sigma_f$ and thus it conserves linear and angular momentum.
- The Corrected approach is found to be more reliable overall.