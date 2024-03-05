---

title: "On the Resolution of Discrete Variational Equations with Boundary Conditions"
collection: talks
type: "Talk"
permalink: /talks/2023/monteiro
venue: "XVII Congreso Dr. Antonio Monteiro"
date: 2023-06-08
location: "Bahía Blanca, Argentina"
featured_image: "https://www.matematica.uns.edu.ar/xviicm/images/aviso_lma.png"
excerpt: "We present a novel approach to discrete variational equations using parallelization."
---

Sebastián Ferraro from the Department of Mathematics at Universidad Nacional del Sur (UNS) – CONICET, David Martín de Diego from Instituto de Ciencias Matemáticas, Spain, and Rodrigo T. Sato Martín de Almagro from the Institute of Applied Dynamics at Friedrich-Alexander-Universität Erlangen-Nürnberg, Germany, present their joint research on resolving discrete variational equations with boundary conditions.

Given a γ-order Lagrangian system represented by a function \(L : T(γ)Q → R\), where \(T(γ)Q\) denotes the γ-order tangent bundle of the manifold \(Q\), a discretization approach consists of approximating the action in a timestep \(h\) through a discrete Lagrangian \(Ld : T(γ−1)Q × T(γ−1)Q → R\). The objective is to find discrete trajectories \(x0, . . . , xN ∈ T(γ−1)Q\) that optimize the discrete action \(∑N_{k=1} Ld (xk−1, xk)\). This leads to variational integrators, which have proven to be efficient in numerical simulations of mechanical systems.

When boundary conditions \(x0\) and \(xN\) are imposed, a resolution method based on computational parallelization is proposed. Starting from an initial "guess" sequence of points, each \(xk, k = 1, . . . , N − 1\), evolves iteratively, using only the information from the neighboring points. This method converges to a solution of the problem under certain conditions. The analysis of these conditions allows us to discuss the notion of conjugate points for such discrete systems.

The research is funded by the [BBVA Foundation](https://www.fbbva.es/) and [Agencia Estatal de Investigación](https://www.aei.gob.es/).
