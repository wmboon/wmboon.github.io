---
title: Fitted norm preconditioners for the Hodge Laplacian
# header: 
#   teaser: /assets/images/*.png
#   overlay_image: /assets/images/*.png
excerpt: Fitted norm preconditioners for the Hodge Laplacian in mixed form
authors: W.M. Boon, J. Kraus, T. Luber, M. Lymbery
journal: 
tags: 
    - differential complexes
    - preconditioners
---

<!-- [Published version](https://doi.org/10.48550/arXiv.2507.23586){: .btn .btn--info} -->
[ArXiv (open access)](https://doi.org/10.48550/arXiv.2507.23586){: .btn .btn--success}

We consider the Hodge-Laplace problem in mixed form: Find $(u, p) \in H\Lambda^{k - 1} \times H \Lambda^k$ such that

$$
\begin{bmatrix}
    \alpha & -d^* \\
    -d & - d^* d
\end{bmatrix}
\begin{bmatrix}
    u \\ p
\end{bmatrix}
= 
\begin{bmatrix}
    g \\ -f
\end{bmatrix}
$$

in which $d$ is the differential and $\alpha > 0$ a constant. 

We recognize this as a perturbed saddle point problem and use the framework of [Hong et al.](https://doi.org/10.1090/mcom/3795) to derive the parameter-dependent norms in which the problem is well-posed. Two different strategies are adopted, which both lead to the same preconditioner, namely

$$
\mathcal{P} := \begin{bmatrix}
    \alpha I + (1 + \alpha) d^* d \\
    & (1 + \alpha)^{-1} I + d^* d
\end{bmatrix}^{-1}
$$

Numerical experiments in 2D and 3D confirm that the preconditioner is robust with respect to $h$ and $\alpha$. 