---
name: "Generic vectorization of parabolic PDEs using parallel in time concepts"
speakers:
  - "Alexander Schell"
  - "Christian Engwer"
categories:
  - "Talks"
session: "09:15 - 10:45"
---

We present a generic approach to increase the performance of PDE solvers for a wide range of instationary problems on modern hardware. In many applications low order methods are still the most common approach to solve PDEs. While they are easy to implement, they are inherently memory bound due to a low arithmetic intensity and thus don't benefit from the high level of concurrency of modern hardware architectures. To increase the arithmetic intensity, it is necessary to increase the work per matrix entry. For applications which require solving different linear systems with the same operator, Block-Krylov methods offer a mathematical tool to increase the arithmetic intensity and in previous work we added corresponding support to our DUNE linear algebra library. Conceptually, a system for multiple time steps of a time stepping method or multiple Runge-Kutta stages can be reformulated to solve a single matrix equation instead of many linear systems which may be solved using Block-Krylov methods. We introduce the general ideas, present first performance results and discuss implementational aspects.
