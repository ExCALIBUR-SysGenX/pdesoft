---
name: "A framework for implementing virtual element spaces"
speakers:
  - "Andreas Dedner"
  - "Alice Hodson"
categories:
  - "Talk"
session: "13:30 - 15:00"
---

The Virtual Element Method (VEM) is a recent approach to define a wide range of finite element type spaces on general element shapes. We will discuss the construction of these methods within existing finite element software packages requiring little overhaul of the existing code base. Our approach is an extension of the well known FEM constructing based on finite element triples (K, B, L). Here K is a grid element, B is the basis of a finite dimensional space, and L is a set of functionals with |L| = |B|. To construct spaces with desirable properties (approximation order and conformity for example) the choice for L is often known but defining a suitable B can be challenging. We introduce the concept of a VEM tuple using a fixed B depending on the approximation order but not on L thus avoiding the problem described above. The similarity with the FEM construction simplifies the implementation of VEM schemes within existing FEM codes. Our proof of concept implementation is based on the DUNE software framework and is publicly available. The code currently includes a range of spaces suitable for forth order problems and some unusual vector valued spaces, e.g., curl-free and divergence conforming spaces. The latter for example is especially of interest for simulating fluid flow since it provides a stable, higher order approximations with a low number of degrees of freedom.
