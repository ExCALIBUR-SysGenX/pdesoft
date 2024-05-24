---
name: "Redefining the finite element"
speakers:
  - "India Marsden"
  - "David A. Ham"
  - "Patrick E. Farrell"
categories:
  - "Talks"
session: "13:30 - 15:00"
---

A core feature of the success of the finite element method, the Ciarlet definition of the components of a finite element has been used for many years. The experience of these decades (and the subsequent implementations) has exposed several key deficiencies. In particular, Ciarlet’s definition is missing information about the global continuity of the mesh and how the degrees of freedom map to each other under the relative orientation of the mesh entities. This information is necessary to implement the finite element method, leaving scope for a new definition. 

We propose a new definition to handle these issues and incorporate the constantly growing landscape of new elements. This new definition also aims to encapsulate more information about the elements, such as the symmetries, incorporating ideas from Group Theory. Through this work, we hope to produce a robust, thorough definition that allows processes such as implementation-independent serialisation of finite element data. 

This talk will present the machinery of the proposed new definition in two dimensions and provide some examples of commonly used elements. 
