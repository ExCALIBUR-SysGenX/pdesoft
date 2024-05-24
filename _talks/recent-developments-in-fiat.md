---
name: "Recent developments in FIAT"
speakers:
  - "Pablo Brubeck"
  - "Robert C. Kirby"
  - "Fabian Laakmann"
  - "Lawrence Mitchell"
categories:
  - "Talk"
---

FIAT (FInite element Automatic Tabulator) provides a powerful Python library for generation and tabulation of finite elements. We present recent improvements to FIAT aimed at improving its run time and the accuracy and efficiency of code generated using FIAT-provided information. These include an interface to the recursivenodes package for more accurate Lagrange bases at high order, and the addition of simplicial quadrature rules of (Xiao and Gimbutas, 2010), which require many fewer quadrature points than the Stroud conical product rules. We also implemented integral-type degrees of freedom for finite elements in the $L^2$-de Rham complex, which enable more accurate interpolation. FIAT now provides support for fast diagonalization methods, which enable fast solution algorithms at very high order. In each case, we illustrate some of the gains obtained through simple numerical tests.