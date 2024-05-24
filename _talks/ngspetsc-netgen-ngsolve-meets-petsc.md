---
name: "ngsPETSc: NETGEN/NGSolve meets PETSc"
speakers:
  - "Umberto Zerbinati"
  - "Patrick E. Farrell"
  - "Stefano Zampini"
categories:
  - "Talks"
session: "10:00 - 11:15"
---

We present ngsPETSc, an interface between the NETGEN mesher, the finite element library

NGSolve and the Portable, Extensible Toolkit for Scientific computation (PETSc). ngsPETSc

interface is written in Python and takes advantage of the Python bindings of Netgen/NGSolve and petsc4py. The key components of ngsPETSc are the interface between NETGEN and PETSc DMPlex and the interface between NGSolve and PETSc PC, KSP and SNES.

In particular, thanks to the first component it is possible to export mesh generated from geometries described via constructive solid geometry (CSG) using OpenCASCADE as PETSc DMPlex objects. Based on this component new features have been added to Firedrake. In particular, now Firedrake supports linear and higher-order meshes that conform to the constructive solid geometry. Furthermore, ngsPETSc allows the construction of mesh hierarchies for multigrid solvers in two dimensions. Lastly, different mesh splits such as Alfeld and Powell-Sabin splits are supported in Firedrake.

The PETSc PC and KSP interface allows the use of PETSc solvers in NGSolve. In particular,

the PETSc PC interface also allows to use of the PETSc preconditioners directly in the linear algebra solvers implemented in NGSolve. Lastly, the PETSc SNES interface gives NGSolve users access to the full range of non-linear solvers present in PETSc. In particular, PETSc SNES can be used to solve complex non-linear problems and to solve the optimisation problems related to the energy of a particular system.
