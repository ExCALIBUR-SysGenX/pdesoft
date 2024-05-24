---
name: "A Programming Language for coordinate free linear algebra"
speakers:
  - "Teodoro Fields Collin"
  - "Teodoro F. Collin"
  - "Oded Stein"
  - "Gilbert Bernstein"
  - "Saman Amarasinghe"
categories:
  - "Talk"
---

In this talk, we propose a new programming language and compiler for deducing implementations of linear algebra operations from a high level specification. We will show how we can use these tools to generate code for pullbacks & permutation management of finite elements such as the Morley & Argyris elements. The core idea of our language and compiler is "coordinate free" linear algebra. Our language features separate specifications of vectors, vector spaces, and bases, but our compiler combines a vector and a basis to generate code that builds an array representing the vector in the given basis. Our system is conceptually similar to computer algebra systems for differential geometry, but also heavily builds on the ideas in earlier UFL compilers (pre quadrature representation) as well as FIAT/FINAT. However, our language is minimal, focusing on certain universal features of linear algebra; the finite element applications are achieved as corollaries to the existing features. Our system also provides a convenient system for managing the linear algebra details that occur when dealing with manifolds and exterior calculus. We will describe a preliminary specification of our language, a compilation algorithm, and how we use the language to fully specify finite elements. 