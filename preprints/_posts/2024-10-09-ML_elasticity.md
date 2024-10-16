---
title: Momentum preserving neural network solvers for elasticity
header: 
  teaser: /assets/images/papers/quiver2j0_splitted_3.png
  overlay_image: /assets/images/papers/quiver2j0_splitted_3.png
excerpt: Neural network solvers for parametrized elasticity problems that conserve linear and angular momentum
authors: W.M. Boon, N.R. Franco, A. Fumagalli
journal: 
tags: 
    - neural networks
    - spanning trees
---

<!-- [Published version](){: .btn .btn--info} -->
[ArXiv (open access)](https://arxiv.org/abs/2410.06975){: .btn .btn--success}

## Highlights
- We consider the Arnold-Falk-Winther finite element triplet to discretize the stress, displacement, and rotation variables.
- Using a spanning tree, a *particular* solution $\sigma_f = Sf$ is rapidly constructed that balances body and boundary forces and is weakly symmetric.
- Two strategies are proposed that guarantee conservation of linear and angular momentum:
    - A *Split* approach in which a neural network is trained to update the particular solution.
    $$ \sigma = \sigma_f + (I - SB) \tilde{\sigma}$$
    - A *Corrected* strategy that trains a neural network to compute the stress 
    $$ \sigma = \sigma_f + (I - SB) (\hat{\sigma} - \sigma_f)$$
- The corrected approach is found to be more reliable overall.