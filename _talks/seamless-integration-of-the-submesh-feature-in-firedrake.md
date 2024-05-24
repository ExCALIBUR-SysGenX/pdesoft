---
name: "Seamless integration of the submesh feature in Firedrake"
speakers:
  - "Koki Sagiyama"
  - "Lawrence Mitchell"
  - "David A. Ham"
categories:
  - "Talk"
session: "13:30 - 14:45"
---

We talk about integration of the submesh feature in Firedrake that enables one to extract parts of an existing mesh and make them work together to solve finite element problems.

The user interface is made intuitive, respecting the current interface of Firedrake. We discuss required changes in the DMPlex component of the Portable, Extensible Toolkit for Scientific Computation (PETSc), which manages parallel unstructured meshes in Firedrake, and the Unified Form Language (UFL), which allows for representing the finite element problems symbolically at high-level. We talk about interesting corner cases to consider in the parallel settings. We present numerical examples to demonstrate our implementations.
