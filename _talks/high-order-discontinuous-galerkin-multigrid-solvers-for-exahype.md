---
name: "High-order discontinuous Galerkin multigrid solvers for ExaHyPE"
speakers:
  - "Alexander Belozerov"
  - "Sean Baccas"
  - "Advanced Research Computing"
  - "Alexander Belozerov"
  - "Department of Mathematical Sciences)"
  - "Eike Mueller"
  - "Department of Mathematical Sciences)"
  - "Dmitry Nikolaenko"
  - "Advanced Research Computing"
  - "Tobias Weinzierl"
  - "Department of Computer Science)"
categories:
  - "Talk"
---

ExaHyPE is an open-source solver engine for hyperbolic PDEs with a successful track record in diverse applications from seismology to astrophysics. We extend ExaHyPE to a wider class of problems by developing elliptic solvers using high-order discretisation and multigrid techniques.

While ExaHyPE focuses on hyperbolic equations, many applications require the solution of problems that combine properties of hyperbolic and elliptic types: these arise, for example, from constraints equations in computational astrophysics and fluid dynamics. This development will allow the combination of hyperbolic and elliptic solvers in a uniform computational framework naturally designed to operate on hierarchical meshes and HPC infrastructure, leveraging the advantages of the multigrid approach.

Mathematically, the goal is to use the hybridisable Discontinuous Galerkin method for high-order space-time discretisation of problems with elliptic constraints. Multigrid is the elliptic solver of choice since it is the only method that scales algorithmically (computational cost grows linearly with the number of unknowns) to large problems on exascale machines.

We designed an abstraction that separates the mathematical details of the (local) discretisation from the (global) problem assembly. This separation of concerns is crucial to guarantee the productivity of mathematicians and software engineers developing highly sophisticated algorithms.