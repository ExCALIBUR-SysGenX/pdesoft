---
name: "pyMOR: From model order reduction to numerics in abstract spaces"
speakers:
  - "Stephan Rave"
  - "Linus Balicki"
  - "Hendrik Kleikamp"
  - "Petar Mlinarić"
  - "Jens Saak"
  - "Felix Schindler"
categories:
  - "Talks"
session: "09:15 - 10:45"
---

pyMOR is a free Model Order Reduction library written in the Python programming language. All of pyMOR's algorithms are formulated in terms of operations on abstract VectorArray and Operator objects. This allows to seamlessly integrate pyMOR with various PDE solver libraries by directly utilizing the linear algebra backends of these solvers. Over the past decade, pyMOR has grown to encompass not only a large array of MOR algorithms, it also implements QR decomposition, SVD, eigensolvers, various matrix equation solvers, as well as a Newton algorithm and basic time steppers.

In this talk I will give a brief overview of pyMOR and highlight some of its recent features. I will then introduce our new project, NiAS. Refining the abstractions established in pyMOR, our goal with NiAS is to develop a new foundational library of numerical algorithms operating in abstract spaces, and to make pyMOR part of the NiAS ecosystem. I will discuss how NiAS' approach not only allows to transparently exchange linear algebra libraries and implementation languages, but also allows running the same algorithms in truly infinite-dimensional spaces as appearing in adaptive FEM or meshless approaches.
