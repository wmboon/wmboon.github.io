---
title: RBM with local mass conservation
header: 
  teaser: /assets/images/midirom_papers/case3_sol.png
  overlay_image: /assets/images/midirom_papers/case3_sol.png
excerpt: A Reduced Basis Method for Darcy flow systems that ensures local mass conservation by using exact discrete complexes.
tags: MiDiROM
---

[Published version (open access)](https://doi.org/10.1007/s10915-023-02119-3){: .btn .btn--success}

## Key ideas
- The difference between two locally conservative flux fields is solenoidal and therefore given by the curl of a potential field.
- We propose a three-step solution procedure:
  1. Given $f$, use a locally conservative scheme such as the TPFA finite volume method to find a $q_f$ that solves the mass balance equation: $\nabla \cdot q_f = f$.
  2. Solve for the potential $r$ by solving a curl-curl problem.
  3. Set $q = q_f + \nabla \times r$ and post-process the pressure $p$.
- The second step can be approximated using a Reduced Basis Method.

{% include figure image_path="/assets/images/midirom_papers/RBM.png" caption="Three test cases solved using the reduced basis method. In each case, mass is conserved locally up to machine precision." %}

## Main findings
- The solution is locally conservative regardless of the accuracy of the reduced basis method. This can be shown as follows:
$$\nabla \cdot q = \nabla \cdot q_f + \nabla \cdot (\nabla \times r) = \nabla \cdot q_f = f.$$
- The original saddle point problem is reduced to three smaller, symmetric positive definite systems.
- The procedure is valid for mixed-dimensional fracture flow by using the mixed-dimensional curl operator.
