---
name: "Solving mixed-domain problems in FEniCSx"
speakers:
  - "Joseph P. Dean"
  - "Jørgen Schartum Dokken"
  - "Garth N. Wells"
categories:
  - "Talks"
session: "13:30 - 15:00"
---

Problems involving fields defined over different domains arise in many areas of science and engineering. The fields may be coupled in regions where domains overlap or domain boundaries intersect. Examples include multiphysics problems, where coupling may occur in the bulk or at interfaces, and Lagrange multiplier problems, where the unknown fields may be defined over domains of different topological dimensions. Solving such problems for real-world applications typically requires large-scale simulations to provide sufficient accuracy.

We present recent developments in the FEniCSx core libraries, inspired by some previous work in FEniCS [1], that allows mixed-domain problems to be solved in an efficient manner. Subdomains (of possibly different topological dimensions) can be created by specifying a subset of mesh entities, yielding a submesh. Forms can then be assembled involving functions defined over different meshes. The relationships between the meshes can be nested, and high-order geometry is supported. Parallelism and scalability are at the heart of the design philosophy, and code prototyped on a laptop can be deployed on an HPC system without modification.

We show several examples with application to magnetohydrodynamics, hybridised discontinuous Galerkin methods, and problems with Neumann boundary conditions. Performance results are also presented.

[1] Cécile Daversin-Catty, Chris N. Richardson, Ada J. Ellingsrud, and Marie E. Rognes. 2021. Abstractions and Automated Algorithms for Mixed Domain Finite Element Methods. ACM Trans. Math. Softw. 47, 4, Article 31 (December 2021). [doi.org/10.1145/3471138](https://doi.org/10.1145/3471138)
