---
title: Auxiliary space preconditioners for Virtual Elements
header: 
  teaser: /assets/images/papers/DeRhamDodecaFinal.png
  overlay_image: /assets/images/papers/DeRhamDodecaFinal.png
excerpt: Nodal auxiliary space preconditioners for mixed virtual element methods
authors: W.M. Boon, E. Nilsson
journal: "ESAIM: Mathematical Modelling and Numerical Analysis, 59(1), 363-387"
tags: 
    - auxiliary space
    - differential complexes
    - preconditioners
---

<!-- [Published version](){: .btn .btn--info} -->
[Published version](https://doi.org/10.1051/m2an/2024081){: .btn .btn--success}

In short, we generalized the Hiptmair-Xu auxiliary space preconditioner to the Virtual Element Method on polyhedral grids. 

## Key ideas
- The Virtual Element spaces form a discrete differential complex.
- We derive a regular decomposition of the edge and face Virtual element spaces in terms of the nodal space and high-frequency terms.
- From the regular decomposition, we construct an auxiliary space preconditioner.

## Main findings
- We show theoretically and numerically that the preconditioner is robust with respect to the mesh size $h$.
- Numerical experiments show that the preconditioner is robust with respect to large aspect ratios. It therefore shows potential for problems in which the mesh is naively adapted to conform to interfaces or inclusions.