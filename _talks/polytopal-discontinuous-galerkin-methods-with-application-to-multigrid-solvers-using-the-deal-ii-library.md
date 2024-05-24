---
name: "Polytopal discontinuous Galerkin methods with application to multigrid solvers using the deal.II library"
speakers:
  - "Marco Feder"
  - "Luca Heltai"
  - "Andrea Cangiani"
categories:
  - "Talk"
---

Agglomeration strategies are a key ingredient in polytopal methods for PDEs as they are used to generate (hierarchies of) computational grids from an initial grid. We present a novel approach to perform agglomeration of polygonal and polyhedral grids based on spatial

indices. We show how the construction of the R-tree spatial database of an arbitrary fine grid offers a natural and efficient agglomeration strategy. Our process is fully automated, robust, and automatically produces a balanced and nested hierarchy of agglomerates which allows geometric multigrid methods to be applied also to those cases where a hierarchy of grids is not directly available [1]. We present the new C++ library polyDEAL, based on the deal.II library, which provides building blocks for polytopal Discontinuous Galerkin methods, allowing arbitrarily shaped elements and different agglomeration strategies. Its memory-distributed implementation is based on the MPI communication model. To show the effectiveness of our approach, we present several examples in the context of non-trivial three-dimensional geometries and the design of geometric multigrid preconditioners.

[1] Feder, M., Cangiani, A., Heltai, L. (2024). R3MG: R-tree based agglomeration of

polytopal grids with applications to multilevel methods. https://arxiv.org/pdf/2404.18505