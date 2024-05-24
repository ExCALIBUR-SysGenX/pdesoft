---
name: "p-multigrid on LUMI GPU HPC"
speakers:
  - "Chris Richardson"
  - "Igor Baratta"
  - "Joseph P. Dean"
  - "Garth N. Wells"
categories:
  - "Talks"
session: "15:30 - 17:15"
---

Solving very large elliptic problems in a scalable way requires a scalable preconditioner, such as multigrid. For arbitrary problems on unstructured meshes, algebraic multigrid (AMG) offers a neat solution. However, AMG needs assembled matrices, and therefore a large storage requirement. For a GPU-based code, where memory is at a premium, it is neater to use a matrix-free method, especially if we can use higher-order elements (which are inimical to AMG). In this presentation, we will explore the options for hooking up matrix-free multigrid at higher order to AMG on a coarse representation, and present some results from the EuroHPC machine LUMI using AMD MI-250X GPUs with GPU-aware MPI and FEniCSx.
