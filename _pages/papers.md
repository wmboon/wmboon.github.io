---
permalink: /papers/
title: "Scientific Publications"
classes: wide
---

## Journal articles

{% assign paper_posts = site.posts | where_exp:"post", "post.categories contains 'papers'"%}
{% assign years = paper_posts
   | group_by_exp: "post", "post.date | date: '%Y'"
%}
{% for year in years %}
  <h3>{{ year.name }}</h3>

  <ul style="list-style-type:square">
    {% for post in year.items %}
      <li>
        {{ post.authors }}. 
        <a href='{{ post.url }}'>{{ post.excerpt }}.</a>
        <em>{{ post.journal }}.</em>
      </li>
    {% endfor %}
  </ul>
{% endfor %} 

## Journal articles

### 2023



- W.M. Boon, D. Gläser, R. Helmig, I. Yotov. \
    [Flux-mortar mixed finite element methods with multipoint flux approximation.](https://doi.org/10.1016/j.cma.2022.115870)\
	*Computer Methods in Applied Mechanics and Engineering*, 
    405, 115870.

- W.M. Boon, J.M. Nordbotten \
    [Mixed-dimensional poromechanical models of fractured porous media.](https://doi.org/10.1007/s00707-022-03378-1)\
	*Acta Mechanica*, 
    234(3), 1121-1168.

### 2022
- W.M. Boon, T. Koch, M. Kuchta, K.-A. Mardal. \
    [Robust monolithic solvers for the Stokes-Darcy problem with the Darcy equation in primal form.](https://doi.org/10.1137/21M1452974)\
	*SIAM Journal on Scientific Computing*, 
    44(4), B1148-B1174.
- W.M. Boon, M. Hornkjøl, M. Kuchta, K.-A. Mardal, R. Ruiz-Baier. \
    [Parameter-robust methods for the Biot-Stokes interfacial coupling without Lagrange multipliers.](https://doi.org/10.1016/j.jcp.2022.111464)\
	*Journal of Computational Physics*, 
    67, 111464.
- W.M. Boon, D. Gläser, R. Helmig, I. Yotov. \
    [Flux-Mortar Mixed Finite Element Methods on Non-matching Grids.](https://doi.org/10.1137/20M1361407)\
	*SIAM Journal on Numerical Analysis*, 
    60(3), 1193-1225.

### 2021
- W.M. Boon, M. Kuchta, K.-A. Mardal, R. Ruiz-Baier.	 \
    [Robust preconditioners for perturbed saddle-point problems and conservative discretizations of Biot's equations utilizing total pressure.](https://doi.org/10.1137/20M1379708)\
	*SIAM Journal on Scientific Computing*, 
    43(4), B961-B983.
- W.M. Boon, J.M. Nordbotten. \
    [Stable Mixed Finite Elements for Linear Elasticity with Thin Inclusions.](http://dx.doi.org/10.1007/s10596-020-10013-2)\
	*Computational Geosciences*, 
    25(2), 603-620.
- W.M. Boon, J.M. Nordbotten, J.E. Vatne. \
    [Functional Analysis and Exterior Calculus on Mixed-Dimensional Geometries.](https://doi.org/10.1007/s10231-020-01013-1)\
	*Annali di Matematica Pura ed Applicata*,
    200(2), 757-789. 
- I. Berre, W.M. Boon, B. Flemisch, A. Fumagalli, D. Gläser, E. Keilegavlen, A. Scotti, I. Stefansson, A. Tatomir, et al \
    [Verification benchmarks for single-phase flow in three-dimensional fractured porous media.](https://doi.org/10.1016/j.advwatres.2020.103759)\
	*Advances in Water Resources*, 
    147, 103759.
-	W.M. Boon, J.M. Nordbotten. \
	[An Adaptive Penalty Method for Inequality Constrained Minimization Problems.](https://doi.org/10.1007/978-3-030-55874-1_14)\
	*Numerical Mathematics and Advanced Applications ENUMATH 2019*, 
    Springer, Cham, 155-164.

### 2020
- A. Budiša, W.M. Boon, X. Hu. \
    [Mixed-Dimensional Auxiliary Space Preconditioners.](https://doi.org/10.1137/19M1292618)\
	*SIAM Journal on Scientific Computing*, 
    42(5), A3367-A3396.
- W.M. Boon. \
    [A Parameter-Robust Iterative Method for Coupled Stokes-Darcy Models Retaining Local Mass Conservation.](https://doi.org/10.1051/m2an/2020035)\
	*ESAIM: Mathematical Modelling and Numerical Analysis*, 
    54(6), 2045-2067.
- M. Schneider, K. Weishaupt, D. Gläser, W.M. Boon, and R. Helmig. \
    [Coupling staggered-grid and MPFA finite volume methods for free flow/porous-medium flow problems.](https://doi.org/10.1016/j.jcp.2019.109012)\
	*Journal of Computational Physics*, 
    401, 109012. 
-	W.M. Boon, J.M. Nordbotten. \
	[Convergence of a TPFA Finite Volume Scheme for Mixed-Dimensional Flow Problems.](https://doi.org/10.1007/978-3-030-43651-3_40)\
	*Finite Volumes for Complex Applications IX*, 
    435-444.

### 2019
- J.M. Nordbotten, W.M. Boon, A. Fumagalli, E. Keilegavlen. \
    [Unified Approach to Discretization of Flow in Fractured Porous Media.](https://doi.org/10.1007/s10596-018-9778-9)\
	*Computational Geosciences*, 
    23 (1), 225-237.

### 2018
- W.M. Boon, J.M. Nordbotten, I. Yotov. \
    [Robust Discretization of Flow in Fractured Porous Media.](https://doi.org/10.1137/17M1139102)\
	*SIAM Journal on Numerical Analysis*, 
    56 (4), 2203-2233.
- B. Flemisch, I. Berre, W.M. Boon, A. Fumagalli, N. Schwenck, A. Scotti, I. Stefansson, A. Tatomir. \
    [Benchmarks for Single-Phase Flow in Fractured Porous Media.](https://doi.org/10.1016/j.advwatres.2017.10.036)\
	*Adv. in Water Resources*, 
    111, 239-258.
-	J.M. Nordbotten, W.M. Boon. \
    [Modeling, Structure and Discretization of Hierarchical Mixed-Dimensional Partial Differential Equations.](https://doi.org/10.1007/978-3-319-93873-8_7)
	*Int. Conf. on Domain Decomposition Methods*, 
    87-101.

### 2017
- N. Balbarini, W.M. Boon, P.L. Bjerg, J.M. Nordbotten, P.J. Binning. \
    [A 3-D Numerical Model of the Influence of Meanders on Groundwater Discharge to a Gaining Stream in an Unconfined Sandy Aquifer.](https://doi.org/10.1016/j.jhydrol.2017.06.042)\
	*Journal of Hydrology*,
    552, 168-181.
- W.M. Boon, N. Balbarini, P.J. Binning, J.M. Nordbotten. \
    [Efficient Water Table Evolution Discretization using Domain Transformation.](https://doi.org/10.1007/s10596-016-9597-9)\
	*Computational Geosciences*, 
    21 (1), 3-11.

### 2016
- W.M. Boon, D.C. Koppenol, F.J. Vermolen. \
    [A Multi-Agent Cell-Based Model for Wound Contraction.](https://doi.org/10.1016/j.jbiomech.2015.11.058)\
	*Journal of Biomechanics*, 
    49 (8), 1388-1401.

## Theses

- Doctoral thesis. \
    [Conforming Discretizations of Mixed-Dimensional Partial Differential Equations](https://bora.uib.no/bora-xmlui/handle/1956/18159)\
    University of Bergen.
- Master thesis. \
    [Incorporation of Contracture Formation in Dermal Wound Healing: A Mathematical Model](https://repository.tudelft.nl/islandora/object/uuid:fd95b7e1-5509-455b-9bca-febbafba72a0)\
    Delft University of Technology.