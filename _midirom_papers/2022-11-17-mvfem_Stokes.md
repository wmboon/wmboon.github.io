---
title: Multipoint MFEM for Stokes flow
header: 
  teaser: /assets/images/midirom_papers/Picture2.png
  overlay_image: /assets/images/midirom_papers/Picture2.png
excerpt: A multipoint vorticity mixed finite element method for incompressible Stokes flow.
---

[Published version (open access)](https://doi.org/10.1016/j.aml.2022.108498){: .btn .btn--success}

## Key ideas

- We rewrite the Stokes equations as a vector Laplacian and reformulate the equations in terms of vorticity, velocity, and pressure.
- The equations are discretized using low-order finite element spaces that conform to the de Rham complex.
- Using a low-order quadrature rule, the vorticity is eliminated and we are left with the Raviart-Thomas finite element pair of lowest order.

{% include figure image_path="/assets/images/midirom_papers/deRham_Stokes.png" caption="The three finite elements used for the vorticity, velocity, and pressure in 3D. The vorticity space (yellow) is eliminated through a structure-preserving quadrature rule." %}


## Main findings

- First order (optimal) convergence is shown in $H(curl) \times H(div) \times L^2$.
- The pressure is invariant to the use of the quadrature rule.
- In 2D, the vorticity variable is invariant and converges quadratically
- The flow field is pointwise solenoidal and the method is pressure robust.

{% include figure image_path="/assets/images/midirom_papers/Picture3.png" caption="Stokes flow calculated using the multipoint vorticity method with a rotational forcing term. The velocity is superimposed on the vorticity on the left and the right shows the pressure." %}

