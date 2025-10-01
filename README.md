# Awesome Quantum Computing [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Curated resources for mastering quantum computing, from the first qubit intuition to current research horizons. Inspired by the [awesome-*](https://github.com/sindresorhus/awesome) ecosystem.

## Contents

- Explore: [Books](#books), [Getting Started](#getting-started), [Mathematics & Prerequisites](#mathematics--prerequisites)
- Learn: [Courses & Bootcamps](#courses--bootcamps), [Hands-on Tutorials & Notebooks](#hands-on-tutorials--notebooks), [Podcasts & Video Series](#podcasts--video-series)
- Build: [Libraries & SDKs](#libraries--sdks), [Developer Tools](#developer-tools), [Hardware Access & Cloud Platforms](#hardware-access--cloud-platforms)
- Research: [Datasets & Benchmarks](#datasets--benchmarks), [Research Papers & Surveys](#research-papers--surveys), [Journals & Magazines](#journals--magazines)
- Connect: [Communities & Events](#communities--events), [Newsletters & Blogs](#newsletters--blogs), [Talks & Conferences](#talks--conferences), [Use Cases & Case Studies](#use-cases--case-studies)
- Stewardship: [Contributing](#contributing), [License](#license)

Entries are alphabetical inside each section. Prefer concise descriptions (≤2 sentences) and trusted, up-to-date sources.

## Books

- *Programming Quantum Computers* – Eric R. Johnston, Nic Harrigan, and Mercedes Gimeno-Segovia. Hands-on introduction using circuit diagrams and Rigetti’s stack.
- *Quantum Computation and Quantum Information* – Michael A. Nielsen and Isaac L. Chuang. The canonical reference covering core theory and algorithms.
- *Quantum Computing: An Applied Approach* – Jack D. Hidary. Bridges foundational math with near-term applications and hardware considerations.
- *Quantum Computing for Everyone* – Chris Bernhardt. Accessible overview requiring only high-school algebra.
- *Quantum Information Processing with Cirq* – Oleksandr Kyriienko et al. Practical guide centered on Google’s Cirq ecosystem.

## Getting Started

- [Exploring Quantum Computing (Microsoft Learn)](https://learn.microsoft.com/en-us/training/paths/quantum-computing-fundamentals/) – Free learning path with self-check quizzes that introduce Azure Quantum tooling.
- [Quantum Algorithm Zoo](https://quantumalgorithmzoo.org/) – Catalogue of known quantum algorithms with one-paragraph summaries and citations.
- [Quantum Computing for the Very Curious](https://quantum.country/qcvc) – Narrative-driven primer with spaced-repetition flashcards built in.
- [The Qubit by Qiskit Textbook](https://qiskit.org/textbook/ch-states/what-is-a-qubit.html) – Interactive chapter exploring the anatomy of a qubit via executable code.
- [What is Quantum Computing? (IBM Quantum)](https://quantum-computing.ibm.com/composer/docs/iqx/guide/what-is-quantum-computing) – High-level orientation to qubits, superposition, and entanglement.

## Mathematics & Prerequisites

- [Complex Numbers and Probability (Brilliant)](https://brilliant.org/courses/quantum-computing/) – Interactive modules on amplitudes, phases, and measurement probabilities.
- [Linear Algebra – Gilbert Strang (MIT OCW)](https://ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/) – Definitive lecture series on matrices, eigenvalues, and vector spaces.
- [Linear Algebra for Quantum Computing (Qiskit YouTube Playlist)](https://www.youtube.com/playlist?list=PLOFEBzvs-VvrmdJ9XQ4kNxTmPyiXBZLUr) – Quantum-focused recaps with coding exercises.
- [Mathematics for Quantum Mechanics (Coursera)](https://www.coursera.org/learn/mathematics-for-quantum-mechanics) – Refresher on bras, kets, and operators for physics newcomers.
- [Quantum Computation Lecture Notes (University of Waterloo)](https://cs.uwaterloo.ca/~watrous/quantum-information/) – Graduate-level notes emphasizing linear algebra foundations.

## Courses & Bootcamps

- [edX Professional Certificate in Quantum Computing (DelftX)](https://www.edx.org/professional-certificate/delftx-quantum-101-quantum-computing-quantum-internet) – Two-course pathway from basics to quantum networking concepts.
- [MIT xPRO: Quantum Computing Fundamentals](https://xpro.mit.edu/courses/course-v1:xPRO+QCFx1/) – Instructor-led program with labs on IBM Quantum hardware.
- [Quantum Computing Fundamentals (Qiskit Global Summer School archives)](https://www.youtube.com/playlist?list=PLOFEBzvs-Vvq-w0faL8i3Lz7iQus9nIhN) – Recorded lectures and guided labs covering circuits and algorithms.
- [The Quantum School by Q-CTRL (Black Opal)](https://q-ctrl.com/black-opal) – Interactive lessons with visualizations and spaced repetition.
- [University of Toronto: Quantum Machine Learning](https://www.coursera.org/learn/quantum-machine-learning) – Applies PennyLane to introduce hybrid ML workflows.

## Hands-on Tutorials & Notebooks

- [Amazon Braket Workshop Notebooks](https://github.com/aws/amazon-braket-examples) – End-to-end examples for Braket simulators and partner hardware.
- [Cirq Experiments & Docs](https://quantumai.google/cirq) – NISQ-friendly circuit design patterns and realistic noise modeling.
- [PennyLane Tutorials](https://pennylane.ai/qml/demos/) – Differentiable quantum programming demos spanning QML and chemistry.
- [Qiskit Textbook](https://qiskit.org/textbook) – Open-source notebook series covering algorithms, error mitigation, and applications.
- [Quantum Katas (Microsoft)](https://github.com/microsoft/QuantumKatas) – Self-paced Q# coding exercises with unit tests.

## Podcasts & Video Series

- [Coding with Qiskit](https://www.youtube.com/playlist?list=PLOFEBzvs-VvqHl5YhZP5M2p17fZ5KgLeY) – Tutorials on algorithms, tooling, and best practices.
- [Entangled Things](https://entangledthings.com/) – Weekly conversations about quantum technologies and theory.
- [Quantum Computing Now](https://feeds.transistor.fm/quantum-computing-now) – Digestible updates on algorithms and hardware milestones.
- [The Quantum Pod (Q-CTRL)](https://q-ctrl.com/podcast) – Interviews with researchers and industry leaders.
- [Two Minute Papers: Quantum Playlist](https://www.youtube.com/playlist?list=PLujxSBD-JXgnqkVUvRsm4DtE6tvwFFxaM) – Bite-sized summaries of recent research developments.

## Libraries & SDKs

- [Braket SDK](https://github.com/amazon-braket/amazon-braket-sdk-python) – Toolkit for Amazon Braket simulators and third-party hardware.
- [Cirq](https://github.com/quantumlib/Cirq) – Google-backed Python framework optimized for NISQ devices.
- [PennyLane](https://github.com/PennyLaneAI/pennylane) – Differentiable quantum programming with ML integrations.
- [Q# and the Quantum Development Kit](https://github.com/microsoft/Quantum) – Microsoft’s language, libraries, and simulators for hybrid quantum programs.
- [Qiskit](https://github.com/Qiskit/qiskit) – IBM’s open-source SDK for circuit design, transpilation, and execution.
- [QuTiP](https://github.com/qutip/qutip) – Python toolbox for open quantum system dynamics and control.

## Developer Tools

**Circuit simulators**
- [Intel Quantum Simulator](https://github.com/intel/qpp) – High-performance state-vector simulator with distributed execution support.
- [ProjectQ](https://github.com/ProjectQ-Framework/ProjectQ) – Compiler framework with pluggable classical and quantum backends.
- [Qiskit Aer](https://qiskit.org/documentation/apidoc/aer.html) – Noise-aware simulators that integrate directly with Qiskit circuits.
- [Qulacs](https://github.com/qulacs/qulacs) – Fast C++/Python simulator tailored for large-scale circuits.
- [TensorCircuit](https://github.com/tencent-quantum-lab/tensorcircuit) – Tensor-network backed simulator with automatic differentiation.

**IDEs & visual builders**
- [IBM Quantum Composer](https://quantum.ibm.com/composer) – Drag-and-drop circuit editor backed by live calibration data.
- [IBM Quantum Lab](https://quantum.ibm.com/lab) – Managed Jupyter environment with pre-installed quantum SDKs.
- [Microsoft Quantum Development Kit for VS Code](https://marketplace.visualstudio.com/items?itemName=quantum.QDK) – Extension providing Q# syntax highlighting, debugging, and templates.
- [Quirk](https://algassert.com/quirk) – Browser-based circuit playground for rapid intuition building.

**Workflow & orchestration**
- [Classiq Designer](https://www.classiq.io/) – Model-based synthesis platform for complex quantum circuits.
- [Covalent](https://github.com/AgnostiqHQ/covalent) – Python orchestrator for hybrid classical-quantum workloads.
- [Mitiq](https://github.com/unitaryfund/mitiq) – Open-source toolkit for error mitigation techniques.
- [QURI Parts](https://github.com/QunaSys/quri-parts) – Modular Python components for variational algorithm pipelines.

## Hardware Access & Cloud Platforms

- [Amazon Braket](https://aws.amazon.com/braket/) – Managed access to multiple trapped-ion, superconducting, and neutral-atom providers plus simulators.
- [IBM Quantum Platform](https://quantum.ibm.com/) – Fleet of superconducting devices with free and premium plans and Qiskit integration.
- [IonQ Cloud](https://cloud.ionq.com/) – Native trapped-ion hardware access with detailed calibration metrics.
- [Microsoft Azure Quantum](https://azure.microsoft.com/en-us/products/quantum/) – Unified access to hardware partners and classical solvers inside Azure.
- [Xanadu Borealis via Strawberry Fields](https://strawberryfields.ai/) – Photonic quantum computing access with Gaussian boson sampling demos.

## Datasets & Benchmarks

- [MQT Bench](https://github.com/cda-tum/mqt-bench) – Suite of reversible and quantum circuits for benchmarking compilers and simulators.
- [QASMBench](https://github.com/pnnl/QASMBench/) – Open-source benchmark set for fair comparison of quantum software stacks.
- [SupermarQ](https://superstaq.readthedocs.io/en/latest/apps/supermarq/supermarq.html/) – Application-centric metrics for comparing quantum hardware performance.
- [Unitary Fund Metriq](https://metriq.info/) – Community database tracking quantum algorithm benchmark results across platforms.

## Research Papers & Surveys

**Introductory & survey papers**
- [A Survey of Quantum Computing](https://www.sciencedirect.com/science/article/abs/pii/S1574013718301709) – Broad overview of hardware, algorithms, and software stacks.
- [National Academies: Quantum Computing – Progress and Prospects (2019)](https://nap.nationalacademies.org/catalog/25196/quantum-computing-progress-and-prospects) – Policy-focused assessment of timelines and challenges.
- [Quantum Algorithms: An Overview (arXiv:0808.0369)](https://arxiv.org/abs/0808.0369) – Classic survey summarizing the main algorithmic primitives.
- [Quantum Computing for Computer Scientists (Noson et al.)](https://ccpd.ciens.ucv.ve/wp-content/uploads/2025/03/Noson-S.-Yanofsky-Mirco-A.-Mannucci-Quantum-Computing-for-Computer-Scientists.pdf) – Gentle ramp aimed at CS backgrounds.

**Specialized topics**
- [Post-Quantum Cryptography Status Report (NIST)](https://csrc.nist.gov/projects/post-quantum-cryptography) – Standardization updates and background references.
- [Quantum Advantage in Cryptography (arXiv:2206.04078)](https://arxiv.org/abs/2206.04078) – Survey of cryptographic protocols leveraging quantum capabilities.
- [Quantum Chemistry with Hybrid Algorithms (Nature Reviews Chemistry, 2023)](https://www.nature.com/articles/s41598-024-67897-8) – Review of VQE-style methods for molecular simulation.
- [Quantum Error Correction for Beginners (arXiv:0905.2794)](https://arxiv.org/abs/0905.2794) – Introductory tutorial on stabilizer codes and fault tolerance.

## Journals & Magazines

- [ACM Transactions on Quantum Computing](https://dl.acm.org/journal/tqc) – Peer-reviewed venue for theoretical and applied quantum research.
- [npj Quantum Information](https://www.nature.com/npjqi/) – Nature portfolio journal covering information theory, communication, and computation.
- [PRX Quantum](https://journals.aps.org/prxquantum/) – American Physical Society journal spotlighting high-impact quantum research.
- [Quantum Journal](https://quantum-journal.org/) – Community-run open-access journal for quantum science.
- [Quantum Science and Technology](https://iopscience.iop.org/journal/2058-9565) – IOP journal spanning theory, hardware, and applications.

## Communities & Events

- [IBM Quantum Community](https://www.ibm.com/quantum/community) – Global meetups, hackathons, and collaborative challenges.
- [Quantum Computing Stack Exchange](https://quantumcomputing.stackexchange.com/) – Expert Q&A forum covering theory and practice.
- [Quantum Open Source Foundation (QOSF) Mentorship](https://qosf.org/) – Cohort-based mentorship advancing open quantum projects.
- [Quantum.Tech Community](https://www.quantumtechcongress.com/) – Industry-focused events and regional meetups.
- [r/QuantumComputing](https://www.reddit.com/r/QuantumComputing/) – Community discussions, news, and project showcases.

## Newsletters & Blogs

- [AWS Quantum Technologies Blog](https://aws.amazon.com/blogs/quantum-computing/) – Announcements, tutorials, and case studies from AWS.
- [IBM Quantum Blog](https://research.ibm.com/topics/quantum) – Engineering deep dives and roadmap updates.
- [Quantum Computing Report](https://quantumcomputingreport.com/) – Weekly newsletter on hardware, funding, and corporate moves.
- [Quantum Zeitgeist](https://quantumzeitgeist.com/) – Daily news and analysis on industry trends.
- [Shtetl-Optimized](https://scottaaronson.blog/) – Scott Aaronson’s research commentary on quantum complexity.
- [The Quantum Insider](https://thequantuminsider.com/) – Aggregated market intelligence and funding news.

## Talks & Conferences

- [APS March Meeting – Quantum Information Track](https://march.aps.org/) – Extensive technical program spanning hardware and algorithms.
- [IEEE International Conference on Quantum Computing and Engineering (QCE)](https://qce.quantum.ieee.org/) – Flagship annual event with tutorials and competitions.
- [Q2B Conference](https://q2b.qcware.com/) – Industry summit highlighting commercialization progress.
- [Quantum.Tech](https://www.alphaevents.com/events-quantumtech/) – Global series focused on enterprise adoption and standards.
- [SciRate Quantum Talks](https://scirate.com/search?utf8=%E2%9C%93&q=Quantum+Computing/) – Community-curated talk announcements and paper discussions.

## Use Cases & Case Studies

- [Bain & Company: Quantum Computing Moves from Theoretical to Inevitable (2025)](https://www.bain.com/insights/quantum-computing-moves-from-theoretical-to-inevitable-technology-report-2025/) – Market analysis on near-term business value.
- [BCG: Where Will Quantum Computers Create Value—and When?](https://www.bcg.com/publications/2019/quantum-computers-create-value-when/) – Framework for prioritizing initiatives across industries.
- [Deloitte: Quantum Computing Services](https://www.deloitte.com/us/en/what-we-do/capabilities/quantum/services/quantum-computing-services.html/) – Practical assessment of risk management and optimization use cases.
- [IBM Quantum Industry Case Studies](https://www.ibm.com/quantum/resources/industry/) – Collection of cross-sector pilots and proof-of-concept results.

## Contributing

Have a favorite paper, library, or tutorial that belongs here? Contributions are welcome!

1. Fork the repository and create a feature branch.
2. Add your resource with a short description (max two sentences) under the most fitting section.
3. Keep entries alphabetized within their section and avoid duplicates.
4. Submit a pull request describing your addition and why it helps learners.

Please follow the [Awesome List guidelines](https://github.com/sindresorhus/awesome/blob/main/contributing.md) and respect the licensing terms of linked materials.

## License

This work is released under the [Creative Commons CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) license. Feel free to reuse, remix, and share.
