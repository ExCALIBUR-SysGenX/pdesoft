---
name: "Differentiable programming across the PDE and machine learning barrier"
speakers:
  - "Nacime Bouziani"
  - "David A. Ham"
categories:
  - "Talk"
---

The combination of machine learning and physical laws has shown immense potential for solving scientific problems driven by partial differential equations (PDEs) with the promise of fast inference, zero-shot generalisation, and the ability to discover new physics. Examples include the use of fundamental physical laws as inductive bias to machine learning algorithms, also referred to as physics-informed machine learning, and the application of machine learning to represent features not represented in the differential equations such as closures for unresolved spatiotemporal scales. However, the simulation of complex physical systems by coupling advanced numerics for PDEs with state-of-the-art machine learning demands the composition of specialist PDE solving frameworks with industry-standard machine learning tools. Hand-rolling either the PDE solver or the neural net will not cut it. In this work, we introduce a generic differentiable programming abstraction that provides scientists and engineers with a highly productive way of specifying end-to-end differentiable models coupling machine learning and PDE-based components, while relying on code generation for high performance. Our interface automates the coupling of arbitrary PDE-based systems and machine learning models and unlocks new applications that could not hitherto be tackled, while only requiring trivial changes to existing code. Our framework has been adopted in the Firedrake finite-element library and supports the PyTorch and JAX ecosystems, as well as downstream libraries.