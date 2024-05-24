---
name: "Non-intrusive multirate time-integration for high-order accurate compressible fluid dynamics with Trixi.jl"
speakers:
  - "Daniel Doehring"
  - "Michael Schlottke-Lakemper"
  - "Gregor Gassner"
  - "Manuel Torrilhon"
categories:
  - "Talk"
---

In this talk, we are going to discuss the implementation of multirate time-integration schemes in the Discontinuous Galerkin Code Trixi.jl.

Trixi.jl targets the adaptive simulation of purely hyperbolic and hyperbolic-parabolic compressible flows and is written in native Julia.

Unsteady flow computations typically rely on time integration schemes which employ an identical global timestep thoughout the domain.

However, in cases with strong variations of wave speeds and/or spatial resolution, local stability criteria allow for much larger time steps in some parts of the domain.

By extending the paired-explicit Runge-Kutta schemes by Vermeire et al., high-order, conservative, and consistent multirate time integration

of convection-dominated PDEs in method-of-lines form can be performed.

We demonstrate that by implementing these methods as partitioned Runge-Kutta schemes, we may leave the entire spatial discretization process untouched.

In particular, the semidiscretization of our scheme remains compatible to the OrdinaryDiffEq.jl time integration package and the SciML interface, which allows us to use features from the SciML ecosystem such as algorithmic differentiation and to immediately benchmark our approach against alternative methods.

We demonstrate significant savings in terms of flux evaluations resulting in speedup compared to a range of state-of-the-art optimized Runge-Kutta schemes while maintaining temporal accuracy.

The presented application examples cover aerodynamics and coupled acoustic-inviscid flow simulations.