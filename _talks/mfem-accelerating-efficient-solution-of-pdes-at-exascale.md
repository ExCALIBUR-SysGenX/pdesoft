---
name: "MFEM: accelerating efficient solution of PDEs at exascale"
speakers:
  - "Tzanio Kolev"
categories:
  - "Talk"
session: "13:30 - 15:00"
---

Exascale architectures require rethinking of the numerical algorithms used in large-scale PDE-based applications. These architectures favor algorithms, such as high-order finite elements, that expose fine-grain parallelism and maximize the ratio of floating point operations to energy intensive data movement. In this talk we present an overview of MFEM, a scalable library for high-order finite element discretization of PDEs on general unstructured grids. We also report on the work in the Center for Efficient Exascale Discretizations, a co-design center in the US Exascale Computing Project focused on next-generation discretization software and algorithms. We will describe recent research on performance optimizations for GPU architectures, scalable meshing and discretization algorithms, and matrix-free preconditioning.
