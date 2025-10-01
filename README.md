# Awesome Quantum Computing [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Curated resources for mastering quantum computing, from the first qubit intuition to current research horizons. Inspired by the [awesome-*](https://github.com/sindresorhus/awesome) ecosystem.

## Contents

- [Getting Started](#getting-started)
- [Foundational Mathematics](#foundational-mathematics)
- [Textbooks & Reference Books](#textbooks--reference-books)
- [Online Courses & Bootcamps](#online-courses--bootcamps)
- [Hands-on Tutorials & Notebooks](#hands-on-tutorials--notebooks)
- [Software Development Kits (SDKs)](#software-development-kits-sdks)
- [Simulators, IDEs & Tooling](#simulators-ides--tooling)
- [Algorithms & Implementations](#algorithms--implementations)
- [Research Papers & Surveys](#research-papers--surveys)
- [Communities, Events & News](#communities-events--news)
- [Podcasts & Video Series](#podcasts--video-series)
- [Contributing](#contributing)
- [License](#license)

## Getting Started

- [What is Quantum Computing? (IBM Quantum)](https://quantum-computing.ibm.com/composer/docs/iqx/guide/what-is-quantum-computing) – Friendly overview that introduces qubits, superposition, and entanglement.
- [The Qubit by Qiskit Textbook](https://qiskit.org/textbook/ch-states/what-is-a-qubit.html) – Interactive explanation with experiments you can run in the browser.
- [Quantum Computing for the Very Curious](https://quantum.country/qcvc) – Narrative-driven primer with spaced-repetition notes built in.
- [Exploring Quantum Computing (Microsoft Learn)](https://learn.microsoft.com/en-us/training/paths/quantum-computing-fundamentals/) – Free learning path with quizzes using Azure Quantum tooling.
- [Quantum Algorithm Zoo](https://quantumalgorithmzoo.org/) – Catalogue of known quantum algorithms with short descriptions and references.

## Foundational Mathematics

- [Linear Algebra – Gilbert Strang (MIT OCW)](https://ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/) – Gold-standard lecture series covering matrices, eigenvalues, and inner products.
- [Linear Algebra for Quantum Computing (Qiskit YouTube Playlist)](https://www.youtube.com/playlist?list=PLOFEBzvs-VvrmdJ9XQ4kNxTmPyiXBZLUr) – Quantum-focused treatment with code examples.
- [The Mathematics of Quantum Mechanics (Coursera)](https://www.coursera.org/learn/mathematics-for-quantum-mechanics) – Refresher on bras, kets, and operators.
- [Complex Numbers and Probability (Brilliant)](https://brilliant.org/courses/quantum-computing/) – Interactive modules on amplitudes and measurement probabilities.

## Textbooks & Reference Books

- *Quantum Computation and Quantum Information* – Nielsen & Chuang (Cambridge University Press). The definitive reference for theory and algorithms.
- *Quantum Computing: An Applied Approach* – Jack D. Hidary. Blends math, coding examples, and near-term hardware discussion.
- *Programming Quantum Computers* – Eric R. Johnston, Nic Harrigan, and Mercedes Gimeno-Segovia. Hands-on introduction using Quipper-like circuits and Rigetti’s stack.
- *Quantum Computing for Everyone* – Chris Bernhardt. Accessible introduction requiring only high-school algebra.
- *Quantum Information Processing with Cirq* – Oleksandr Kyriienko et al. Practical guide centered on Google’s Cirq ecosystem.

## Online Courses & Bootcamps

- [The Quantum School by Q-CTRL (Black Opal)](https://q-ctrl.com/black-opal) – Interactive lessons with visualizations and spaced repetition.
- [MIT xPRO: Quantum Computing Fundamentals](https://xpro.mit.edu/courses/course-v1:xPRO+QCFx1/) – Instructor-led program with labs on IBM Quantum Experience.
- [University of Toronto: Quantum Machine Learning](https://www.coursera.org/learn/quantum-machine-learning) – Introduces QML concepts with PennyLane exercises.
- [edX Professional Certificate in Quantum Computing (DelftX)](https://www.edx.org/professional-certificate/delftx-quantum-101-quantum-computing-quantum-internet) – Two-course pathway from basics to quantum networks.
- [Quantum Computing Fundamentals (Qiskit Global Summer School archives)](https://www.youtube.com/playlist?list=PLOFEBzvs-Vvq-w0faL8i3Lz7iQus9nIhN) – Lecture recordings and labs from IBM’s annual summer school.

## Hands-on Tutorials & Notebooks

- [Qiskit Textbook](https://qiskit.org/textbook) – Open-source, interactive notebook series covering circuits, algorithms, and error mitigation.
- [PennyLane Tutorials](https://pennylane.ai/qml/demos/) – Differentiable quantum programming demos, including QML and chemistry.
- [Cirq Experiments & Docs](https://quantumai.google/cirq) – Examples for NISQ-friendly circuit design and noise-aware workflows.
- [Amazon Braket Workshop Notebooks](https://github.com/aws/amazon-braket-examples) – End-to-end examples running on AWS-managed hardware and simulators.
- [Quantum Katas (Microsoft)](https://github.com/microsoft/QuantumKatas) – Self-paced coding exercises in Q# with unit tests.

## Software Development Kits (SDKs)

- [Qiskit](https://github.com/Qiskit/qiskit) – IBM’s Python SDK with circuit building, transpilation, and access to real devices.
- [Cirq](https://github.com/quantumlib/Cirq) – Google-backed library optimized for NISQ hardware and custom gate scheduling.
- [PennyLane](https://github.com/PennyLaneAI/pennylane) – Cross-platform, differentiable quantum programming with ML integrations.
- [Braket SDK](https://github.com/amazon-braket/amazon-braket-sdk-python) – Toolkit for Amazon Braket simulators and partner hardware.
- [Q# and the Quantum Development Kit](https://github.com/microsoft/Quantum) – Microsoft’s language and tooling for high-level quantum programs.
- [QuTiP](https://github.com/qutip/qutip) – Quantum optics and open quantum system simulations in Python.

## Simulators, IDEs & Tooling

- [Qiskit Aer](https://qiskit.org/documentation/apidoc/aer.html) – High-performance simulators with noise modeling.
- [Qulacs](https://github.com/qulacs/qulacs) – Fast C++/Python simulator optimized for large circuits.
- [ProjectQ](https://github.com/ProjectQ-Framework/ProjectQ) – Compiler framework with pluggable backends.
- [TensorCircuit](https://github.com/tencent-quantum-lab/tensorcircuit) – Tensor-network-backed differentiable simulator.
- [Quirk](https://algassert.com/quirk) – Browser-based circuit sandbox for quick experimentation.
- [Bloch Sphere Visualizer](https://javafxpert.github.io/grok-bloch/) – Interactive visualization of single-qubit states.

## Algorithms & Implementations

- [Shor’s Algorithm in Qiskit](https://github.com/Qiskit/qiskit-community-tutorials/tree/master/algorithms/shor_algorithm) – Factoring example with modular exponentiation circuits.
- [Grover’s Search Demos](https://github.com/quantumlib/Cirq/tree/master/examples) – Cirq notebooks highlighting amplitude amplification.
- [Quantum Phase Estimation (PennyLane)](https://pennylane.ai/qml/demos/tutorial_qpe) – Walkthrough with gradient-based optimization tips.
- [Variational Quantum Eigensolver (VQE) Tutorials](https://qiskit.org/documentation/partners/qiskit_nature/tutorials/) – Chemistry-focused variational algorithms and problem mappings.
- [Quantum Approximate Optimization Algorithm (QAOA) Examples](https://github.com/hsinyuan-huang/VQE-QAOA-resource-list) – Community-maintained list of combinatorial optimization demos.

## Research Papers & Surveys

**Introductory & Survey Papers**
- ["Quantum Computing for Computer Scientists" (Brown et al.)](https://arxiv.org/abs/2008.06647) – Gentle ramp for CS backgrounds.
- ["A Survey of Quantum Computing" (arXiv:2011.03294)](https://arxiv.org/abs/2011.03294) – Big-picture overview of hardware, algorithms, and applications.
- ["A Comprehensive Review of Quantum Machine Learning" (arXiv:2401.11351)](https://arxiv.org/abs/2401.11351) – State of the art in QML methods and benchmarks.

**Specialized Topics**
- [Quantum Error Correction for Beginners (arXiv:0905.2794)](https://arxiv.org/abs/0905.2794) – Introductory tutorial on stabilizer codes.
- [Post-Quantum Cryptography Status Report (NIST)](https://csrc.nist.gov/projects/post-quantum-cryptography) – Standardization updates and background reading.
- [Quantum Advantage in Cryptography (arXiv:2206.04078)](https://arxiv.org/abs/2206.04078) – Survey of cryptographic protocols leveraging quantum capabilities.
- [Quantum Chemistry with Hybrid Algorithms (Nature Reviews Chemistry, 2023)](https://www.nature.com/articles/s41570-023-00471-5) – Review of VQE-style approaches for molecular simulation.

## Communities, Events & News

- [Quantum Computing Stack Exchange](https://quantumcomputing.stackexchange.com/) – Q&A forum for experts and learners.
- [r/QuantumComputing](https://www.reddit.com/r/QuantumComputing/) – Community discussions, news, and project showcases.
- [IBM Quantum Community](https://www.ibm.com/quantum/community) – Meetups, hackathons, and collaborative challenges.
- [The Quantum Insider](https://thequantuminsider.com/) – Daily industry and research news.
- [Quantum Computing Report](https://quantumcomputingreport.com/) – Market analysis and hardware updates.
- [IEEE International Conference on Quantum Computing and Engineering (QCE)](https://qce.quantum.ieee.org/) – Flagship annual gathering with tutorials and competitions.

## Podcasts & Video Series

- [The Quantum Pod (Q-CTRL)](https://q-ctrl.com/podcast) – Interviews with researchers and industry leaders.
- [Entangled Things](https://entangledthings.com/) – Weekly conversations about quantum technology and theory.
- [Quantum Computing Now](https://feeds.transistor.fm/quantum-computing-now) – Digestible updates on algorithms and hardware milestones.
- [Two Minute Papers: Quantum Playlist](https://www.youtube.com/playlist?list=PLujxSBD-JXgnqkVUvRsm4DtE6tvwFFxaM) – Bite-sized summaries of recent research.
- [Coding with Qiskit](https://www.youtube.com/playlist?list=PLOFEBzvs-VvqHl5YhZP5M2p17fZ5KgLeY) – Tutorials covering algorithms, tools, and best practices.

## Contributing

Have a favorite paper, library, or tutorial that belongs here? Contributions are welcome!

1. Fork the repository and create a feature branch.
2. Add your resource with a short description (max 1–2 sentences) under the most fitting section.
3. Ensure the list remains alphabetized within each subsection where practical.
4. Submit a pull request describing your addition and why it helps learners.

Please follow the [Awesome List guidelines](https://github.com/sindresorhus/awesome/blob/main/contributing.md) and respect the licensing terms of linked materials.

## License

This work is released under the [Creative Commons CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) license. Feel free to reuse, remix, and share.
