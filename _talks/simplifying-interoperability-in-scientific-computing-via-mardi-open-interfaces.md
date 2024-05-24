---
name: "Simplifying interoperability in scientific computing via MaRDI open interfaces"
speakers:
  - "Dmitry Kabanov"
  - "Stephan Rave"
  - "Mario Ohlberger"
categories:
  - "Talk"
---

The scientific-computing community uses several different programming languages for implementing numerical solvers. Moreover, these solvers often have significantly different programming interfaces. Both of these factors impede interoperability, as switching from, say, a Python solver for time integration to another solver implemented in C requires writing bindings and adapting the calling code to different function names and the order of arguments.

We present our work on simplifying interoperability in scientific computing by alleviating these difficulties. To this aim, we develop a mediator library that automates data marshalling between programming languages so that writing explicit bindings is not required. Additionally, we develop a set of generic interfaces for typical numerical problems. Therefore, users could switch more easily from one implementation to another, while working through the same programming interface.

We describe the architecture and technical details of the library, such as the implementation of data marshalling. We also demonstrate examples of the usage of the library and provide performance analysis by comparison with direct use of numerical solvers.

Our work is part of the German-wide project Mathematical Research Data Initiative (MaRDI). 