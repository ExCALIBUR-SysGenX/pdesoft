---
name: "ExaHyPE 2: an engine for hyperbolic PDEs solver with numerical relativity application as a case study"
speakers:
  - "Han Zhang"
  - "Tobias Weinzierl"
  - "Baojiu Li"
categories:
  - "Talk"
---

We present ExaHyPE 2, the second generation of the Exascale Hyperbolic PDE Solver Engine. It is a tool to implement solvers for hyperbolic PDEs given in first-order formulation, while also providing support to second-order formulation via additional mesh sweep. ExaHyPE 2 features a modular design, allowing users to easily compose their simulation systems by only specifying the evolving quantities and terms of their PDEs. Once specified, ExaHyPE assembles the simulation code hiding parallelisation, data structures, I/O, and so forth. Based upon Peano 4, the code supports dynamically adaptive meshes. The resulting application created by ExaHyPE 2 can be executed on various platforms, ranging from laptops to supercomputers, with support for MPI, OpenMP, TBB, and offloading to GPUs via OpenMP, C++ and SYCL.

In this talk, we will use our numerical relativity application as case study to demonstrate the workflow behind ExaHyPE 2, which is now completely Python-based, as opposed to a mixture of C++ and parameter files in ExaHyPE 1. We also showcase which ingredients (such as numerical schemes) had to be changed due to the application, and how ExaHyPE 2 supports this via the composition of various solvers and their tailoring. 