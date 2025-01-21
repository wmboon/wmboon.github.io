---
title: Preconditioning Stokes-Darcy without fractional operators
# header: 
#   teaser: /assets/images/papers/CechdeRham.png
#   overlay_image: /assets/images/papers/CechdeRham.png
excerpt: Parameter-robust Preconditioners for the Stokes-Darcy Coupled Problem without Fractional Operators
authors: W.M. Boon, X. Hu, X. Wang
journal: 
tags: 
    - Stokes-Darcy
    - preconditioners
---

<!-- [Published version](){: .btn .btn--info} -->
[ArXiv (open access)](https://arxiv.org/abs/2501.06369){: .btn .btn--success}

## Key ideas
- We consider a mixed formulations for the coupled Stokes-Darcy problem, without introducing an interface variable.
- Two finite element discretizations are considered, one based on Raviart-Thomas ($\mathbb{RT}_0$) and one based on Crouzeix-Raviart ($\mathbb{CR}_0$).
- Using weighted norms, we analyze the problem and pay special attention to the cases in which one of the subproblems has solely essential (no-flux) boundary conditions.

## Main findings
- In case of essential boundary conditions in one of the subdomains, the inf-sup constant becomes parameter-dependent. However, this is due to only one parameter-dependent eigenvalue in the system.
- A norm-equivalent preconditioner is proposed and we show that the effective condition number of the preconditioned system is independent of material and discretization parameters.