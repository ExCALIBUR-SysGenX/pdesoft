---
name: "RLST: linear algebra frameworks in Rust for the solution of partial differential equations"
speakers:
  - "Timo Betcke"
  - "Jed Brown"
  - "Srinath Kailasa"
  - "Matthew Scroggs"
categories:
  - "Talks"
session: "15:30 - 17:15"
---

Over the last year we have developed RLST, the Rust Linear Solver Toolbox. It contains a number of data-structures, algorithms, and interfaces to external solvers to support the discretisation and solution of partial differential equations in Rust. Some of its features include heap and stack based n-dimensional array objects, a compile-time lazy expression arithmetic, SIMD acceleration, Lapack interfaces, sparse data structures and linear solves via Umfpack, and a generic operator algebra for iterative solver frameworks.

In this talk we discuss the underlying principles and Rust specific features that were used in the design of this library. Several examples will be shown how RLST is being used in our Rust based boundary element and Fast Multipole Codes.
