---
name: "Contact formulation for mixed finite element"
speakers:
  - "Lukasz Kaczmarczyk"
  - "Chris Pearce University of Glasgow"
  - "Andrei Shvarts University of Glasgow"
categories:
  - "Talk"
---

I present an application of research code to solve industrial structural integrity problems. The finite element framework for the analysis of fracture and contact problems using mixed finite element elements is developed with the support of EDF for the analysis of fractured nuclear graphite bricks. 

During the talk, I will focus on extending the mixed finite element for small strain elasticity to large strain problems. The finite element formulation includes four independently approximated fields, i.e. stresses, logarithm stretches, rotation vectors, and displacements. The first two are associated with conserving linear and angular momentum, respectively. The other two fields are associated with the constitutive equation and the consistency between displacements and deformation. An exponential map establishes the relationship between the rotation vectors and rotation tensor. The stresses are approximated in H(div) space, and the remaining three fields are in L2 space.

This formulation results in a very sparse system of equations that can be efficiently solved in parallel using a block solver, thereby enabling highly scalable and robust solvers. The FE formulation is implemented in the open-source software MoFEM, developed by the Glasgow Computational Engineering Centre.