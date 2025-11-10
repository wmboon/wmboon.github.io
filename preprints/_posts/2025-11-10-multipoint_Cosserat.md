---
title: Multipoint stress mixed finite element methods for the linear Cosserat equations
header: 
  teaser: /assets/images/papers/cosserat_sigma.jpeg
  overlay_image: /assets/images/papers/cosserat_sigma.jpeg
excerpt: Multipoint stress MFEM for Cosserat
authors: W.M. Boon, A. Fumagalli, J.M. Nordbotten, I. Yotov
journal: 
tags: 
    - multipoint MFEM
    - Cosserat
---

<!-- [Published version](){: .btn .btn--info} -->
<!-- [ArXiv (open access)](https://arxiv.org/abs/2510.23432){: .btn .btn--success} -->

We propose four multipoint stress mixed finite element methods for the linear Cosserat equations that are stable in the limit of linear elasticity. 
- The first two methods employ $BDM_1$ elements for the stress variables, and we propose two higher-order methods using $RT_1$ elements.
- Linear convergence is proven for all methods using a priori error estimates.
- For the methods based on $RT_1$ elements, we show quadratic convergence in some of the variables.
- Numerical experiments in 2D and 3D confirm the theoretical findings and we even observe higher orders of convergence than expected.