---
title: No-slip boundary conditions for H(curl)-based Stokes
header: 
  teaser: /assets/images/papers/nitscheFlowAroundCylinder1.png
  overlay_image: /assets/images/papers/nitscheFlowAroundCylinder1.png
excerpt: H(curl)-based approximation of the Stokes problem with weakly emposed no-slip boundary conditions
authors: W.M. Boon, W. Tonnon, E. Zampa
journal: 
tags: 
    - Stokes
---

<!-- [Published version](){: .btn .btn--info} -->
[ArXiv (open access)](https://arxiv.org/abs/2508.02861){: .btn .btn--success}

We consider a formulation for the Stokes problem in which the velocity is sought in H(curl).
The tangential trace is well-defined in this space, but if we impose zero tangential velocity as an essential boundary condition, then the system is not guaranteed to be well-posed. 

Instead, we propose to impose the no-slip condition weakly using Nitsche's method. Using mesh-dependent norms, we show stability of the resulting discrete system and derive a priori error estimates. These estimates are improved in $L^2$ using duality techniques.

The optimal convergence of the velocity is shown both theoretically and numerically. The pressure, on the other hand, exhibits a half order convergence loss, in agreement with the theoretical estimates.

A closely related study concerning Navier-slip conditions can be found [here](/StokesHcurlSlip).