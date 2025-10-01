

# **Awesome Quantum Computing: A Curated Learning Path**

This document provides a definitive, structured guide to learning quantum computing, progressing from foundational concepts to the frontiers of research. It is designed as a comprehensive roadmap for students, developers, researchers, and enthusiasts at all levels of expertise.

## **Introduction to the Quantum Realm**

This section provides a high-level, conceptual entry point into the world of quantum computing, establishing the fundamental "what" and "why" before diving into the technical "how".

### **What is Quantum Computing?**

Quantum computing represents a new paradigm in computation that leverages the principles of quantum mechanics to process information in a fundamentally different manner than classical computers.1 While classical computers, from desktops to smartphones, store and manipulate information using bits, which can only exist in one of two definite states (0 or 1), quantum computers use quantum bits, or

**qubits**.3

A qubit is the fundamental unit of quantum information. Unlike a classical bit, a qubit can exist in a state of 0, a state of 1, or a **superposition** of both states simultaneously.5 This ability to exist in multiple states at once allows quantum computers to explore a vast computational space. The computational power grows exponentially with the number of qubits; for instance, while two classical bits can represent one of four possible combinations (00, 01, 10, 11\) at any given time, two qubits can represent all four combinations simultaneously in a complex superposition.5 With 100 qubits, the range of possibilities becomes astronomically large, far exceeding the capacity of any conceivable classical supercomputer.5

A helpful analogy for understanding superposition is to think of a spinning coin. While it is in the air, it is neither heads nor tails but exists in an undefined state that is a combination of both. Only when it lands—or, in the quantum case, when it is measured—does it collapse into a single, definite outcome.6 This inherent parallelism is a cornerstone of quantum computing's potential power.

### **Why is Quantum Computing Important?**

The significance of quantum computing lies in its potential to solve certain classes of problems that are currently intractable for even the most powerful classical supercomputers.1 This capability could trigger revolutionary advancements across numerous fields.8

Key potential application areas include:

* **Drug Discovery and Materials Science:** Classical computers struggle to accurately simulate the complex quantum mechanical interactions within molecules. Quantum computers could model these systems with high fidelity, enabling the design of novel drugs, catalysts, and materials with desired properties, dramatically accelerating research and development in medicine and engineering.2  
* **Cryptography and Security:** Quantum computers pose a significant threat to modern cybersecurity. Algorithms like Shor's algorithm can efficiently factor large numbers, which would break many widely used encryption schemes such as RSA.1 This has spurred the development of new cryptographic methods, known as quantum-resistant or post-quantum cryptography, to secure data in the future.4  
* **Complex Optimization Problems:** Many critical problems in finance, logistics, and manufacturing are optimization problems that become exponentially more difficult as variables are added. The classic "Traveling Salesman Problem" is a prime example. Quantum computers, by evaluating a vast number of possibilities simultaneously, could find optimal solutions to these problems far more efficiently than classical methods.4  
* **Artificial Intelligence and Machine Learning:** Quantum computing may supercharge artificial intelligence by accelerating complex calculations in machine learning models, potentially leading to more powerful AI systems and new algorithmic approaches.8

### **The Four Pillars of Quantum Mechanics**

The power of quantum computing is derived from harnessing several counterintuitive principles of quantum mechanics. Four of these are central to its operation.5

* **Superposition:** As previously mentioned, this is the ability of a quantum system, such as a qubit, to exist in a combination of multiple distinct states at the same time. A group of qubits in superposition can represent a complex, multidimensional computational space, allowing for a massive degree of parallelism in computations.3  
* **Entanglement:** This phenomenon occurs when two or more qubits become linked in such a way that their fates are intertwined, regardless of the physical distance separating them. The state of one entangled qubit is intrinsically correlated with the state of the other(s). Measuring one qubit instantly provides information about the other, a property Albert Einstein famously described as "spooky action at a distance".5 Entanglement is a critical resource for amplifying the computational power of quantum systems.  
* **Interference:** Often described as the "engine" of quantum computing, interference is the mechanism by which quantum algorithms arrive at the correct answer. By manipulating the wave-like nature of qubits in superposition, algorithms are designed to cause the probability amplitudes of incorrect solutions to cancel each other out (destructive interference) while the amplitudes of correct solutions reinforce each other (constructive interference). This process significantly increases the probability of measuring the desired outcome when the computation concludes.4  
* **Decoherence:** This is the process through which a quantum system loses its quantum properties—its superposition and entanglement—due to interactions with its environment (e.g., thermal fluctuations, electromagnetic fields). Decoherence causes the system to collapse into a classical state, destroying the information being processed.2 It is the primary obstacle in building large-scale, fault-tolerant quantum computers. Consequently, quantum computations must be performed in highly isolated environments, often at temperatures near absolute zero, and completed before decoherence corrupts the result. This duality between the immense power derived from delicate quantum states and the extreme fragility of those same states is the central narrative of the current era of quantum computing. Understanding this tension is crucial, as it motivates the entire field of quantum error correction.

### **The Qubit: A Deeper Look**

The qubit, or quantum bit, is a two-state quantum-mechanical system that serves as the fundamental building block of quantum computers. While theoretically abstract, a qubit must be realized physically. Researchers have developed various physical implementations, including superconducting circuits, trapped ions, photons, and topological qubits, each with its own set of advantages and challenges.

To visualize the state of a single qubit, the **Bloch Sphere** is an invaluable geometric tool. In this representation, the North Pole of the sphere corresponds to the classical state '![][image1]' and the South Pole corresponds to the state '![][image1]'. A classical bit can only be at one of these two poles. A qubit, however, can exist at any point on the surface of the sphere. Each point represents a unique superposition of '![][image1]' and '![][image1]', defined by two angles. Quantum operations, or gates, applied to the qubit correspond to rotations of its state vector on the surface of the Bloch Sphere.1

## **Mathematical Foundations: The Language of Quantum**

While it is possible to grasp the high-level implications of quantum computing conceptually, any practical or deep understanding requires fluency in its native language: mathematics. This section outlines the essential mathematical prerequisites and provides resources for the practitioner's learning track, which begins with these formal tools. A solid foundation in linear algebra, complex numbers, and probability theory is non-negotiable for anyone aspiring to develop or analyze quantum algorithms.2 Additionally, familiarity with programming, particularly Python, is crucial, as it is the lingua franca of the leading quantum software development kits (SDKs).2

### **Linear Algebra for Quantum Computing**

Linear algebra is the fundamental mathematical framework for quantum computing.12 It provides the tools to describe quantum states, the operations that transform them, and the process of measurement.

* **Key Concepts:**  
  * **Vectors and Vector Spaces:** The state of a quantum system is represented by a vector in a complex vector space known as a Hilbert space. A single qubit's state is a vector in a two-dimensional space (![][image1]), a two-qubit system is described by a vector in a four-dimensional space (![][image1]), and an n-qubit system resides in a ![][image1]\-dimensional space (![][image1]).16  
  * **Matrices and Operators:** Quantum gates, which are the operations that manipulate qubits, are represented by unitary matrices. Applying a gate to a quantum state is mathematically equivalent to multiplying the state's vector by the gate's matrix.13  
  * **Inner Product:** The inner product is a mathematical operation that takes two vectors and produces a scalar. In quantum mechanics, it is used to project a quantum state onto another, which is fundamental for calculating the probability of a measurement outcome. Two states are considered orthogonal (distinguishable) if their inner product is zero.16  
  * **Tensor Product:** To describe a system of multiple qubits, the vector spaces of the individual qubits are combined using the tensor product. For example, the state of a two-qubit system is the tensor product of the states of the two individual qubits.13  
* **Curated Resources for Linear Algebra:**  
  * **Textbook Standard:** The canonical textbook *Quantum Computation and Quantum Information* by Nielsen and Chuang begins with a thorough treatment of the required linear algebra, making it a definitive reference.12  
  * **Interactive Courses:** The Singularity Research's "Linear Algebra for Quantum Computing" offers a series of Jupyter notebooks that teach the concepts from the ground up with executable Python code, providing a hands-on learning experience.12  
  * **University Courses:** MIT OpenCourseWare provides a complete "Linear Algebra" course taught by Professor Gilbert Strang. This course is highly recommended as preparation for formal quantum computing studies.18  
  * **Video Lectures:** The Qiskit YouTube channel features a dedicated lecture series on "Introduction to Linear Algebra" tailored for quantum computation, complete with lecture notes.19 For a more visual and introductory approach, the "Quantum Computing Course – Math and Theory for Beginners" on YouTube is also a valuable resource.20

### **Dirac (Bra-Ket) Notation**

To simplify the complex mathematical manipulations of linear algebra in quantum mechanics, Paul Dirac introduced a powerful and concise notation known as bra-ket notation, which is now the standard in the field.16

* **Ket |ψ⟩**: A ket represents a quantum state as a column vector in a complex Hilbert space.13 For example, the computational basis states of a single qubit are written as  
  ![][image1] and ![][image1].  
* **Bra ⟨ψ|**: A bra represents the Hermitian conjugate (conjugate transpose) of a ket, which is a row vector.13  
* **Inner Product ⟨ϕ|ψ⟩**: The product of a bra ⟨ϕ| and a ket |ψ⟩ is their inner product, which results in a scalar complex number. This is used to calculate probability amplitudes.13

## **The Quantum Toolkit: Gates and Circuits**

Moving from abstract mathematics, this section details the concrete building blocks of quantum algorithms: quantum gates and the circuits constructed from them. These are the fundamental tools for manipulating quantum information.

### **From Classical to Quantum Gates**

In classical computing, information is processed by a series of logic gates, such as AND, OR, and NOT, which operate on bits.6 Quantum computing has an analogous set of operations, known as quantum gates, which manipulate the states of qubits.3 A crucial distinction is that all quantum operations (excluding measurement) must be

**reversible**. This means that from the output of a gate, one can always determine its input. This requirement stems from the unitary nature of quantum mechanical evolution. Mathematically, this reversibility is captured by the fact that every quantum gate is represented by a unitary matrix, whose inverse is its own conjugate transpose.

### **A Zoo of Quantum Gates**

A small set of universal quantum gates can be combined to approximate any possible quantum computation. Below are some of the most fundamental gates.

* **Single-Qubit Gates:** These gates operate on a single qubit and are visualized as rotations of the state vector on the Bloch sphere.1  
  * **Pauli Gates (X, Y, Z):** These are foundational. The **Pauli-X gate** is the quantum equivalent of a classical NOT gate, flipping ![][image1] to ![][image1] and vice versa. The **Pauli-Z gate** is a phase-flip gate, leaving ![][image1] unchanged and mapping ![][image1] to ![][image1]. The **Pauli-Y gate** performs both a bit-flip and a phase-flip.13  
  * **Hadamard Gate (H):** This is one of the most important gates in quantum computing. It is the primary tool for creating superposition. When applied to a qubit in the ![][image1] or ![][image1] state, it transforms it into an equal superposition of both, allowing the qubit to explore both possibilities simultaneously.13  
* **Multi-Qubit Gates:** These gates operate on two or more qubits and are essential for creating entanglement.  
  * **Controlled-NOT (CNOT) Gate:** This is a two-qubit gate that acts as a conditional bit-flip. It has a "control" qubit and a "target" qubit. It flips the state of the target qubit if and only if the control qubit is in the state ![][image1]. The CNOT gate is a fundamental building block for creating entangled Bell states and is a key component in many quantum algorithms.3  
  * **Other Gates:** Other important multi-qubit gates include the **SWAP gate**, which swaps the states of two qubits, and various other controlled gates (like the Controlled-Z) that apply an operation conditionally.

### **Constructing Quantum Circuits**

A quantum algorithm is implemented as a **quantum circuit**, which is a timed sequence of quantum gates applied to a register of qubits.3 The standard model of a quantum circuit consists of three distinct stages:

1. **Initialization:** The circuit begins by preparing all qubits into a known, simple initial state. Most commonly, this is the state where all qubits are set to ![][image1].  
2. **Operation:** A sequence of quantum gates is applied to the qubits. These gates manipulate the qubits' states, creating complex superpositions and entanglement patterns designed to produce constructive and destructive interference. This stage is where the core of the quantum algorithm is executed.  
3. **Measurement:** At the end of the computation, the state of one or more qubits is measured. This process extracts a classical outcome—a string of 0s and 1s—from the quantum system. The act of measurement is irreversible and collapses the qubit's superposition into a single definite state. The probability of measuring a particular outcome is determined by the final quantum state's amplitudes.

Quantum circuits are typically visualized using a standard diagrammatic notation. Each qubit is represented by a horizontal line, and time flows from left to right. Gates are represented by boxes or symbols placed on the qubit lines, showing the sequence of operations.

## **Getting Started: A Curated Path for Beginners**

This section serves as the primary entry point for newcomers, offering a structured pathway with resources tailored for different learning styles. The journey into quantum computing can begin either through high-level conceptual understanding or through hands-on, code-free experimentation, both of which build the necessary intuition for more advanced topics.

### **Conceptual First Steps**

For those who wish to understand the "what" and "why" of quantum computing without immediately delving into complex mathematics, these resources provide an accessible introduction. They are ideal for business leaders, students from non-technical backgrounds, or anyone who is simply "quantum-curious."

* **Introductory Articles:**  
  * "Quantum Computing for Dummies – A Simple Guide": An essential guide for beginners to understand the complex world of quantum technology.  
  * "Demystifying Quantum Computing: A Beginner's Guide": A guide aimed at developers that explains quantum concepts without heavy physics or equations.  
* **Introductory Books:**  
  * *Quantum Computing For Dummies* by whurley and Floyd Earl Smith: This book provides a primer on the inner workings and practical applications of quantum computers, explaining the differences between classical and quantum computation and covering its impact on AI and cryptography.10  
  * *Quantum Computing for Everyone* by Chris Bernhardt: Praised for its gentle approach, this book introduces core quantum computing concepts without requiring a background in advanced mathematics, making it highly accessible.15

### **Interactive Learning Platforms**

Before writing a single line of code, it is invaluable to build an intuition for how quantum circuits behave. The following platforms offer visual, hands-on environments to experiment with qubits, gates, and quantum phenomena. Starting with one of these tools is strongly recommended for all beginners, as it provides a tangible feel for abstract concepts like superposition and entanglement.

| Platform | Provider | Description | Key Features | Target Audience |
| :---- | :---- | :---- | :---- | :---- |
| **IBM Quantum Composer** | IBM | A graphical interface for building quantum circuits by dragging and dropping gates. Circuits can be run on both simulators and real IBM quantum hardware.22 | Visual circuit builder, real-time feedback on quantum states, free access to real quantum computers. | Absolute beginners, educators, visual learners. |
| **Black Opal** | Q-CTRL | An interactive online platform that teaches quantum computing through hands-on tasks, gamified modules, and a unique visual coding environment.24 | Interactive activities, skill-based learning paths from beginner to advanced, certification upon completion. | Students, developers, corporate training. |
| **SpinQ Educational Solutions** | SpinQ | A comprehensive suite of educational tools including software, courses, and portable desktop NMR quantum computers for hands-on experiments.25 | Access to real, albeit small, quantum hardware; graphical circuit design; tailored courses. | Educational institutions, hands-on learners. |
| **Amazon Braket Quantum Lab** | Amazon | An integrated development environment within AWS that includes visualization tools for building and analyzing quantum circuits and their states.15 | Integration with the broader AWS ecosystem, circuit visualization, algorithm analysis tools. | Developers and researchers using AWS. |

### **Introductory Online Courses**

For those who prefer a structured learning path with guided instruction, numerous online courses offer a solid foundation in quantum computing.

| Course Name | Provider/Platform | Description | Target Audience |
| :---- | :---- | :---- | :---- |
| **Quantum Computing For Everyone** | UChicagoX (edX) | A two-course professional certificate program that introduces the fundamental principles of quantum computing and its potential applications.26 | General audience, professionals seeking a foundational understanding. |
| **The Complete Quantum Computing Course for Beginners** | Packt (Coursera) | A three-course specialization covering essential mathematics, programming with Qiskit, and core quantum algorithms like Grover's and Shor's.27 | Beginners with a high school math background; no prior programming or quantum knowledge required. |
| **Introduction to Quantum Computing** | MIT xPRO | A four-week professional course covering foundational concepts, engineering challenges, and business implications, including hands-on labs using the IBM Quantum Experience.18 | Professionals, business leaders, and technologists. |
| **Quantum information and computation I** | IBM Quantum Learning | The first course in IBM's foundational series, covering quantum states, measurements, circuits, and the principles of entanglement.22 | Students and professionals with a background in linear algebra and complex numbers. |
| **Quantum 101: Quantum Computing & Quantum Internet** | DelftX (edX) | A professional certificate program that introduces the core concepts of quantum computing and the future quantum internet.26 | General audience, individuals interested in future communication technologies. |

## **Programming the Quantum Future: SDKs and Cloud Platforms**

After building a conceptual and intuitive foundation, the next step is to learn how to program quantum computers. This is primarily done through Python-based Software Development Kits (SDKs) that allow users to design, simulate, and execute quantum algorithms on both simulators and real hardware accessible via the cloud.

### **The Quantum Software Ecosystem**

The modern quantum software stack is a layered ecosystem designed to bridge the gap between high-level algorithmic ideas and low-level hardware control.15

* **Circuit Simulators:** These are classical software programs that simulate the behavior of a quantum computer. They are indispensable for developing, testing, and debugging quantum algorithms before running them on costly and limited quantum hardware. Simulators can provide full access to the quantum state vector, which is impossible on real hardware, making them powerful tools for learning and verification.3  
* **Programming Frameworks:** These are libraries, typically in Python, that provide the functions and abstractions needed to build quantum circuits, define quantum operations, and manage execution. The leading frameworks are open-source and form the backbone of the quantum development community.15  
* **Cloud Platforms:** Quantum computers are expensive, sensitive machines that require specialized environments. Companies like IBM, Google, and Amazon provide access to their quantum hardware and advanced simulators through the cloud, allowing anyone to run quantum programs from their own computer.15

### **Leading Quantum SDKs**

While numerous SDKs exist, three have emerged as the most prominent in the field. The choice of SDK often depends on the user's goals, such as a focus on machine learning or a preference for a particular hardware provider. However, the fundamental skills of circuit construction are largely transferable, and the open-source nature of the ecosystem promotes interoperability; for example, some frameworks can execute code on hardware from multiple different providers.31

| SDK Name | Primary Backer | Core Philosophy & Focus | Key Features | Official Website/Repo |
| :---- | :---- | :---- | :---- | :---- |
| **Qiskit** | IBM | A comprehensive, full-stack SDK for exploring everything from foundational research to utility-scale quantum computing. It is tightly integrated with IBM's hardware and has a strong focus on performance and education.15 | High-performance transpiler for circuit optimization, extensive libraries for algorithms and applications, Qiskit Runtime for hybrid jobs, and the world's largest quantum developer community.33 | [qiskit.org](https://www.ibm.com/quantum/qiskit) |
| **Cirq** | Google | A Python framework designed for writing, manipulating, and optimizing quantum circuits specifically for Noisy Intermediate-Scale Quantum (NISQ) devices. It emphasizes hardware-aware programming to get the most out of today's processors.15 | Detailed control over gate placement and timing, realistic noise modeling, integration with Google Quantum Engine and the Quantum Virtual Machine (QVM) for hardware-realistic simulation.35 | [quantumai.google/cirq](https://quantumai.google/cirq) |
| **PennyLane** | Xanadu | A cross-platform Python library for quantum differentiable programming. Its core focus is the seamless integration of quantum computing with classical machine learning frameworks like PyTorch, TensorFlow, and JAX.31 | Automatic differentiation of quantum circuits on both simulators and hardware, a rich set of tools for quantum machine learning (QML), and broad support for devices from multiple hardware providers through a plugin system.31 | [pennylane.ai](https://pennylane.ai/) |

### **Accessing Real Quantum Computers**

The ability to run algorithms on actual quantum hardware is no longer restricted to a select few. Through cloud platforms, anyone can access and experiment with this cutting-edge technology.

* **IBM Quantum:** Offers the most extensive free-tier access, allowing users to run jobs on a diverse fleet of simulators and real superconducting quantum computers. It is fully integrated with the Qiskit SDK.15  
* **Amazon Braket:** A fully managed service on AWS that provides a single interface to access quantum hardware from multiple providers, including IonQ (trapped ions), Rigetti (superconducting), and others, alongside various high-performance simulators.15  
* **Microsoft Azure Quantum:** An open cloud ecosystem that offers a diverse set of quantum solutions, software, and hardware from Microsoft and its partners.30

## **Core Quantum Algorithms: The Engines of Quantum Power**

Quantum algorithms are the recipes that instruct a quantum computer how to solve a problem. They are carefully designed sequences of quantum gates that leverage principles like superposition and interference to achieve a computational advantage over their classical counterparts.3 While hundreds of quantum algorithms have been proposed, a handful of them form the foundational canon of the field.

Understanding these core algorithms is essential, not only because of their direct applications but also because they introduce fundamental techniques and subroutines that are used to build more complex algorithms. For instance, the Quantum Fourier Transform (QFT) and Quantum Phase Estimation (QPE) are not just standalone algorithms; they are crucial building blocks for landmark algorithms like Shor's for factoring and HHL for solving linear systems.9 The learning path should therefore be structured according to these dependencies, mastering the subroutines before tackling the more complex applications.

The following table provides a comprehensive resource matrix for studying and implementing these key algorithms.

| Algorithm | Description & Significance | Seminal Paper (Link) | Explanatory Articles/Tutorials | Qiskit Implementation | Cirq Implementation | PennyLane Implementation |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| **Quantum Fourier Transform (QFT)** | The quantum analogue of the Discrete Fourier Transform. A critical subroutine for many algorithms, it efficiently finds periodicities in quantum states.9 | ([https://arxiv.org/abs/quant-ph/0201067](https://arxiv.org/abs/quant-ph/0201067)) 42 | ([https://milvus.io/ai-quick-reference/what-is-the-quantum-fourier-transform-and-how-does-it-speed-up-quantum-algorithms](https://milvus.io/ai-quick-reference/what-is-the-quantum-fourier-transform-and-how-does-it-speed-up-quantum-algorithms)), ([https://courses.edx.org/c4x/BerkeleyX/CS191x/asset/chap5.pdf](https://courses.edx.org/c4x/BerkeleyX/CS191x/asset/chap5.pdf)), ([https://courses.physics.illinois.edu/phys498cmp/sp2022/QC/QFT.html](https://courses.physics.illinois.edu/phys498cmp/sp2022/QC/QFT.html)) 43 | ([https://quantumpedia.uk/quantum-algorithm-1-shors-algorithm-for-factorization-part-1-cffcb4f0d0c1](https://quantumpedia.uk/quantum-algorithm-1-shors-algorithm-for-factorization-part-1-cffcb4f0d0c1)) 46 | ([https://learn.microsoft.com/en-us/azure/quantum/tutorial-qdk-qubit-level-program](https://learn.microsoft.com/en-us/azure/quantum/tutorial-qdk-qubit-level-program)) 47 | ([https://pennylane.ai/qml/demos/tutorial\_qft/](https://pennylane.ai/qml/demos/tutorial_qft/)) 48 |
| **Quantum Phase Estimation (QPE)** | Estimates the eigenvalue (or phase) of an eigenvector of a unitary operator. A key building block for Shor's and HHL algorithms.38 | [A. Kitaev, 1995](https://arxiv.org/abs/quant-ph/9511026) 49 | ([https://pennylane.ai/qml/demos/tutorial\_qpe](https://pennylane.ai/qml/demos/tutorial_qpe)), ([https://www.classiq.io/insights/quantum-phase-estimation-qpe](https://www.classiq.io/insights/quantum-phase-estimation-qpe)), ([https://dojo.qulacs.org/en/latest/notebooks/2.4\_phase\_estimation\_beginner.html](https://dojo.qulacs.org/en/latest/notebooks/2.4_phase_estimation_beginner.html)) 50 | ([https://quantumcomputinguk.org/tutorials/quantum-phase-estimation-with-code](https://quantumcomputinguk.org/tutorials/quantum-phase-estimation-with-code)) 53 | ([https://quantumai.google/cirq/experiments/textbook\_algorithms](https://quantumai.google/cirq/experiments/textbook_algorithms)) 54 | ([https://pennylane.ai/qml/demos/tutorial\_qpe](https://pennylane.ai/qml/demos/tutorial_qpe)) 50 |
| **Shor's Algorithm** | Factors large integers into their primes exponentially faster than the best-known classical algorithms. Its discovery launched the field by proving quantum computers could break modern cryptography.1 | ([https://math.mit.edu/\~shor/elecpubs.html](https://math.mit.edu/~shor/elecpubs.html)) 56 | ([https://en.wikipedia.org/wiki/Shor%27s\_algorithm](https://en.wikipedia.org/wiki/Shor%27s_algorithm)), ([https://qrisp.eu/general/tutorial/Shor.html](https://qrisp.eu/general/tutorial/Shor.html)), ([https://www.spinquanta.com/news-detail/shors-algorithm](https://www.spinquanta.com/news-detail/shors-algorithm)) 55 | ([https://quantum.cloud.ibm.com/docs/en/tutorials/shors-algorithm](https://quantum.cloud.ibm.com/docs/en/tutorials/shors-algorithm)) 60 | ([https://quantumai.google/cirq/experiments/shor](https://quantumai.google/cirq/experiments/shor)) 61 | (Community tutorials may exist) |
| **Grover's Algorithm** | Provides a quadratic speedup for searching an unstructured database. While less dramatic than Shor's exponential speedup, it has broad applicability as a subroutine for optimization and search problems.9 | [L. Grover, 1996](https://arxiv.org/pdf/quant-ph/9605034) 62 | ([https://learn.microsoft.com/en-us/azure/quantum/concepts-grovers](https://learn.microsoft.com/en-us/azure/quantum/concepts-grovers)), ([https://www.geeksforgeeks.org/dsa/introduction-to-grovers-algorithm/](https://www.geeksforgeeks.org/dsa/introduction-to-grovers-algorithm/)), ([https://quantum.cloud.ibm.com/learning/courses/fundamentals-of-quantum-algorithms/grover-algorithm/introduction](https://quantum.cloud.ibm.com/learning/courses/fundamentals-of-quantum-algorithms/grover-algorithm/introduction)) 64 | ([https://quantum.cloud.ibm.com/docs/tutorials/grovers-algorithm](https://quantum.cloud.ibm.com/docs/tutorials/grovers-algorithm)) 67 | ([https://www.kaggle.com/code/viratkothari/quantum-computing-grover-s-algorithm-cirq](https://www.kaggle.com/code/viratkothari/quantum-computing-grover-s-algorithm-cirq)) 68 | ([https://pennylane.ai/qml/demos/tutorial\_grovers\_algorithm](https://pennylane.ai/qml/demos/tutorial_grovers_algorithm)) 69 |
| **HHL Algorithm** | Solves systems of linear equations with the potential for exponential speedup over classical methods. It is a foundational algorithm for many quantum machine learning proposals.70 | [Harrow, Hassidim, Lloyd, 2009](https://link.aps.org/doi/10.1103/PhysRevLett.103.150502) 72 | ([https://physlab.org/wp-content/uploads/2023/05/HHL\_22120009\_Fin.pdf](https://physlab.org/wp-content/uploads/2023/05/HHL_22120009_Fin.pdf)), ([https://www.quantumgrad.com/article/462](https://www.quantumgrad.com/article/462)), ([https://www.arclightquantum.com/isq-docs/latest/examples/hhl/](https://www.arclightquantum.com/isq-docs/latest/examples/hhl/)) 40 | (Community tutorials exist) | ([https://qtedu.eu/material/cirq-quantum-algorithms-and-tutorials](https://qtedu.eu/material/cirq-quantum-algorithms-and-tutorials)) 75 | ([https://qrisp.eu/general/tutorial/HHL.html](https://qrisp.eu/general/tutorial/HHL.html)) 76 |
| **Variational Quantum Eigensolver (VQE)** | A hybrid quantum-classical algorithm designed to find the ground state energy (lowest eigenvalue) of a physical system, such as a molecule. It is a flagship algorithm for the NISQ era.9 | [A. Peruzzo et al., 2014](https://arxiv.org/abs/1304.3061) 78 | ([https://en.wikipedia.org/wiki/Variational\_quantum\_eigensolver](https://en.wikipedia.org/wiki/Variational_quantum_eigensolver)), ([https://link.aps.org/doi/10.1103/PhysRevLett.126.220501](https://link.aps.org/doi/10.1103/PhysRevLett.126.220501)) 77 | ([https://quantum.cloud.ibm.com/learning](https://quantum.cloud.ibm.com/learning)) 22 | ([https://quantumai.google/cirq/experiments](https://quantumai.google/cirq/experiments)) 80 | ([https://pennylane.ai/qml/demos/tutorial\_vqe/](https://pennylane.ai/qml/demos/tutorial_vqe/)) 81 |
| **Quantum Approximate Optimization Algorithm (QAOA)** | A hybrid algorithm used to find approximate solutions to combinatorial optimization problems, such as Max-Cut. Like VQE, it is well-suited for near-term quantum devices.38 | [E. Farhi et al., 2014](https://arxiv.org/abs/1411.4028) 83 | ([https://discuss.pennylane.ai/t/qaoa-and-optimization/5188](https://discuss.pennylane.ai/t/qaoa-and-optimization/5188)), ([https://www.semanticscholar.org/paper/A-Quantum-Approximate-Optimization-Algorithm-Farhi-Goldstone/ea238b034c2042fc0ce4efcff288725e5e74f462](https://www.semanticscholar.org/paper/A-Quantum-Approximate-Optimization-Algorithm-Farhi-Goldstone/ea238b034c2042fc0ce4efcff288725e5e74f462)) 84 | ([https://quantum.cloud.ibm.com/learning/tutorials](https://quantum.cloud.ibm.com/learning/tutorials)) 29 | ([https://quantumai.google/cirq](https://quantumai.google/cirq)) 35 | ([https://pennylane.ai/qml/demos/tutorial\_qaoa\_intro/](https://pennylane.ai/qml/demos/tutorial_qaoa_intro/)) 86 |

## **The Intermediate & Advanced Learner's Bookshelf**

While online resources provide dynamic and practical learning experiences, textbooks offer a structured, deep, and cohesive understanding of the field. The journey for a serious practitioner can be seen as a path toward mastering the canonical texts of quantum information science. Beginner books build conceptual foundations, intermediate books develop the necessary mathematical and algorithmic skills, and advanced texts serve as comprehensive references for research and deep study.

The textbook *Quantum Computation and Quantum Information* by Michael Nielsen and Isaac Chuang, often affectionately called "Mike and Ike," stands as the universally acknowledged "bible" of the field.15 Many intermediate textbooks are explicitly positioned as introductions to this comprehensive work.89 Therefore, the learning path can be framed as the journey to fully comprehending Nielsen and Chuang, with other texts serving as essential preparation and companions.

| Title | Author(s) | Description & Focus | Target Audience | Difficulty |
| :---- | :---- | :---- | :---- | :---- |
| *Quantum Computing for Everyone* | Chris Bernhardt | A gentle, conceptual introduction requiring no advanced mathematics. Focuses on building intuition.15 | Absolute beginners, non-technical readers. | **Beginner** |
| *Quantum Computing for Dummies* | whurley & Floyd Smith | A primer on the inner workings and practical applications. Explains the "what" and "how" in an easy-to-understand way.10 | The "quantum-curious", IT professionals. | **Beginner** |
| *Introduction to Classical and Quantum Computing* | Thomas Wong | An excellent introductory textbook, particularly for those with a computer science or math background. Praised for its clarity and logical progression.15 | Undergraduates in CS/Math. | **Intermediate** |
| *Quantum Computing: An Applied Approach* | Jack D. Hidary | Integrates foundational principles with a hands-on coding approach. Suitable for academic courses and corporate training.15 | Students and professionals looking for practical application. | **Intermediate** |
| *Quantum Computing for Computer Scientists* | Yanofsky & Mannucci | An undergraduate textbook that starts from first principles (complex numbers), making it accessible for CS students. Strong section on algorithms.88 | Undergraduates in STEM fields. | **Intermediate** |
| *Dancing with Qubits* | Robert S. Sutor | A comprehensive textbook that covers both the mathematical underpinnings and industry use cases, bridging theory and practice.92 | Those with interest in math, physics, or CS. | **Intermediate/Advanced** |
| *Quantum Computation and Quantum Information* | Nielsen & Chuang | The definitive, canonical reference text. This comprehensive, 700-page book covers the entire field in depth, from foundational physics to advanced algorithms and information theory.12 | Graduate students, researchers, serious practitioners. | **Advanced** |

## **University-Level Learning & Deeper Dives**

For learners seeking a rigorous, academic approach, many of the world's leading universities and researchers have made their course materials and lectures available for free online. These resources provide a university-level education in quantum computation and information theory.

* **MIT OpenCourseWare (OCW):**  
  * **Quantum Computation (18.435J):** Taught by Professor Peter Shor, the inventor of the factoring algorithm. This graduate-level course covers quantum logic, algorithms (including detailed analyses of Shor's and Grover's), quantum error correction, and cryptography.94  
  * **Quantum Complexity Theory (6.845):** An advanced course that delves into the fundamental capabilities and limitations of quantum computers, exploring the boundaries of what is computable in the quantum world.95  
  * **Information and Entropy (6.050J):** Features a comprehensive unit on Quantum Information, including lecture notes and an extensive reading list with seminal papers by Feynman, Bennett, and others.96  
  * **Quantum Physics III (8.06):** Includes a dedicated chapter of lecture notes on Quantum Computing, providing a physicist's perspective on the subject.97  
* **Other University Courses & Lecture Series:**  
  * **Stanford Online:** Offers a suite of courses including "Quantum Mechanics for Scientists and Engineers," which provides the necessary physics background, and a dedicated "Quantum Computing" course.15  
  * **UC Berkeley (via YouTube):** The lectures from Professor Umesh Vazirani's course, "Quantum Mechanics and Quantum Computation," are available online, offering insights from another pioneer in the field.99  
  * **Caltech:** Professor John Preskill's highly influential and comprehensive lecture notes on quantum information and computation are an essential resource for any serious student. They are widely recommended and used in university courses globally.96  
* **Renowned Lecture Series:**  
  * **Quantum Computing for the Determined:** A video lecture series by Michael Nielsen (co-author of the field's standard textbook). It is designed for learners who are comfortable with basic linear algebra and want a deep, principled understanding of quantum computing.15  
  * **IonQ Lecture Series:** Taught by the scientists and engineers at IonQ, this series provides a practical look at the fundamentals of trapped-ion quantum computers and how to program them.101

## **Frontiers of Quantum Research**

For advanced learners and professionals, staying abreast of the latest research is crucial. This section provides an overview of three key frontiers in quantum computing—Quantum Machine Learning, Quantum Error Correction, and Quantum Cryptography—along with links to important review articles and recent breakthrough papers.

### **Quantum Machine Learning (QML)**

QML is an emerging interdisciplinary field that seeks to leverage quantum computers to enhance machine learning tasks. This can involve using quantum algorithms to accelerate classical ML computations or designing entirely new models that process quantum data.22

* **Key Review Papers:**  
  * "A comprehensive review of Quantum Machine Learning: from NISQ to Fault Tolerance" (arXiv:2401.11351): A thorough review covering techniques for both near-term (NISQ) and future fault-tolerant quantum computers.102  
  * "Quantum Machine Learning: A Hands-on Tutorial for Machine Learning Practitioners and Researchers" (arXiv:2502.01146): A 260-page tutorial designed to bridge the gap between classical AI and quantum computing.104  
* **Recent Breakthroughs (2023-2024):**  
  * **Demonstration of a Logical Qubit Prototype (2023):** Researchers at Google AI demonstrated that it is possible to reduce computational errors by increasing the number of qubits, a key milestone for quantum error correction, which is foundational for scalable QML.105  
  * **Quantum Gaussian Processes (2025):** A team at Los Alamos National Laboratory developed a new QML approach using quantum Gaussian processes. This method avoids the "barren plateau" problem—a major obstacle in training quantum neural networks—by using a non-parametric statistical method natively suited to quantum systems.106

### **Quantum Error Correction (QEC)**

The greatest challenge facing practical quantum computing is decoherence—the tendency of qubits to lose their quantum properties due to environmental noise. QEC is a collection of techniques designed to protect quantum information from such errors, making it possible to perform long, complex computations reliably. It is the bedrock upon which fault-tolerant quantum computing will be built.2

* **Introductory Guides:**  
  * "Quantum Error Correction for Beginners" (arXiv:0905.2794): A review that explains the basic aspects of QEC and fault-tolerance through detailed examples rather than rigorous formalism.107  
  * "Quantum Error Correction: An Introductory Guide" (arXiv:1907.11157): An introductory guide to the theory and implementation of QEC codes, with a focus on the surface code.109  
  * "Quantum Error Correction For Dummies" (arXiv:2304.08678): A review tailored for computer scientists, explaining the foundational principles of QEC with limited quantum physics background required.110  
* **Recent Advances:**  
  * **Below-Threshold Error Correction (2024):** Google demonstrated a surface code memory operating below the critical error threshold, where adding more physical qubits to a logical qubit successfully lowered the logical error rate.111  
  * **Concatenated Codes (2025):** Quantinuum, in partnership with Princeton and NIST, reported the first experimental realization of fault-tolerant computation using concatenated codes, a foundational concept of the threshold theorem that proves quantum computing can be scaled.113  
  * **Novel Geometric Codes (2025):** Microsoft developed a new family of 4D geometric codes that significantly reduce the number of physical qubits required per logical qubit and demonstrate a 1,000-fold reduction in error rates.114

### **Quantum Cryptography and Security**

This field encompasses two main areas: using quantum mechanics to create new, provably secure communication methods, and developing classical cryptography that can withstand attacks from future quantum computers.115

* **Quantum Key Distribution (QKD):** QKD protocols, such as the famous BB84 protocol, use the principles of quantum mechanics to allow two parties to generate a shared secret key for encryption. The security is guaranteed by the laws of physics; any attempt by an eavesdropper to intercept the key will disturb the quantum states and be detected.6  
* **Post-Quantum Cryptography (PQC):** In response to the threat posed by Shor's algorithm, researchers are developing new classical cryptographic algorithms whose security is based on mathematical problems believed to be hard for both classical and quantum computers. This is a major global effort to "quantum-proof" our digital infrastructure.116  
* **Key Review Papers:**  
  * "Advances in Quantum Cryptography" (arXiv:1906.01645): A comprehensive review covering QKD, quantum networks, and cryptographic tasks beyond key distribution.119  
  * "Security in Quantum Cryptography" (arXiv:2102.00021): A review focusing on the physical notion of security in quantum cryptography, particularly for QKD and secure communication.120  
  * "Quantum Cryptography Beyond Quantum Key Distribution" (arXiv:1510.06120): A survey of other applications in quantum cryptography, such as quantum money and secure multi-party computation.121

## **Staying Current: The Quantum Community**

Quantum computing is a fast-paced and collaborative field. Engaging with the global community is one of the best ways to stay informed about the latest breakthroughs, ask questions, and find opportunities.

* **Online Forums and Q\&A Sites:**  
  * **Quantum Computing Stack Exchange:** The premier Q\&A platform for technical questions related to quantum computing. It is an invaluable resource for developers and researchers facing specific problems.29  
  * **Reddit \- r/QuantumComputing:** A large and active subreddit for academic discussions, sharing news, and asking questions. It features a helpful weekly thread dedicated to career, education, and basic questions, making it welcoming for beginners.29  
* **Blogs and Newsletters:**  
  * **The Quantum Insider:** A major source for daily news, business analysis, and featured articles on the quantum technology industry. They offer a newsletter for weekly digests.126  
  * **Quantum Zeitgeist:** Provides daily news and analysis on quantum computing, with a focus on business, research, and technology trends.128  
  * **Quantum Computing Report:** Offers in-depth news and analysis of technical developments, funding events, and industry partnerships. An email alert service is available.129  
  * **Shtetl-Optimized:** The influential and highly respected blog of renowned quantum computing researcher Scott Aaronson, offering deep insights into the field.130  
  * **Official Blogs:** Many of the key players maintain excellent blogs, including the **AWS Quantum Technologies Blog** 131, the  
    **IBM Research Blog** 5, and the  
    **Qmunity Blog** by The Quantum Insider.132  
* **Community Platforms:**  
  * **IBM Quantum Community:** Centered around Qiskit, this is the largest quantum developer community in the world. It provides access to events, an open-source ecosystem, and the Qiskit Advocate program for dedicated community members.133  
  * **Pasqal Community:** A global network focused on neutral-atom quantum computing. It offers learning resources, access to open-source tools, and a dedicated Slack workspace for collaboration.135  
  * **Meetup.com:** Hosts numerous local and virtual groups for quantum computing enthusiasts to connect, share experiences, and learn from each other.136

#### **Works cited**

1. What is quantum computing? Learn the basics here\! \- Qureca, accessed October 1, 2025, [https://www.qureca.com/resources/article/quantum-computing-for-dummies/](https://www.qureca.com/resources/article/quantum-computing-for-dummies/)  
2. Demystifying Quantum Computing: A Beginner's Guide \- Akava, LLC, accessed October 1, 2025, [https://akava.io/blog/demystifying-quantum-computing-a-beginners-guide-for-developers](https://akava.io/blog/demystifying-quantum-computing-a-beginners-guide-for-developers)  
3. Quantum Computing Basics: A Beginner's Guide \- BlueQubit, accessed October 1, 2025, [https://www.bluequbit.io/quantum-computing-basics](https://www.bluequbit.io/quantum-computing-basics)  
4. Quantum Computing for Dummies: A Simple Guide to the Future \- SpinQ, accessed October 1, 2025, [https://www.spinquanta.com/news-detail/quantum-computing-dummies](https://www.spinquanta.com/news-detail/quantum-computing-dummies)  
5. What Is Quantum Computing? | IBM, accessed October 1, 2025, [https://www.ibm.com/think/topics/quantum-computing](https://www.ibm.com/think/topics/quantum-computing)  
6. Quantum Computing Technology: Understanding the Basics | NYIT, accessed October 1, 2025, [https://online.nyit.edu/blog/quantum-computing-technology-understanding-the-basics](https://online.nyit.edu/blog/quantum-computing-technology-understanding-the-basics)  
7. An Introduction to Quantum Computing \- Dummies.com, accessed October 1, 2025, [https://www.dummies.com/article/technology/computers/what-is-quantum-computing-300551/](https://www.dummies.com/article/technology/computers/what-is-quantum-computing-300551/)  
8. Quantum Computing for Dummies : A Simple Explanation for Normal People \- YouTube, accessed October 1, 2025, [https://www.youtube.com/watch?v=lypnkNm0B4A](https://www.youtube.com/watch?v=lypnkNm0B4A)  
9. Quantum Computer Algorithms: Key Techniques & Examples | SpinQ, accessed October 1, 2025, [https://www.spinquanta.com/news-detail/quantum-computer-algorithms](https://www.spinquanta.com/news-detail/quantum-computer-algorithms)  
10. Quantum Computing For Dummies | Wiley, accessed October 1, 2025, [https://www.wiley.com/en-us/Quantum+Computing+For+Dummies-p-00384048](https://www.wiley.com/en-us/Quantum+Computing+For+Dummies-p-00384048)  
11. Quantum Computing for Dummies Audiobook by whurley, Floyd Smith \- Audible, accessed October 1, 2025, [https://www.audible.com/pd/Quantum-Computing-for-Dummies-Audiobook/B0CMYXVB65](https://www.audible.com/pd/Quantum-Computing-for-Dummies-Audiobook/B0CMYXVB65)  
12. Linear Algebra for Quantum Computing ... \- The Singularity, accessed October 1, 2025, [https://the-singularity-research.github.io/linear\_algebra\_for\_quantum\_computing/](https://the-singularity-research.github.io/linear_algebra_for_quantum_computing/)  
13. 9.1 Linear algebra for quantum computing \- Fiveable, accessed October 1, 2025, [https://fiveable.me/quantum-computing/unit-9/linear-algebra-quantum-computing/study-guide/Cc4WgWVUYDq4oZjr](https://fiveable.me/quantum-computing/unit-9/linear-algebra-quantum-computing/study-guide/Cc4WgWVUYDq4oZjr)  
14. Basic Quantum Computing — Introduction | by Charlie Thomas \- Medium, accessed October 1, 2025, [https://medium.com/@charlie.thomas\_94667/basic-quantum-computing-introduction-f83dcfbd0e40](https://medium.com/@charlie.thomas_94667/basic-quantum-computing-introduction-f83dcfbd0e40)  
15. Learn Quantum Computing: 4 Proven Ways for Beginners \- SpinQ, accessed October 1, 2025, [https://www.spinquanta.com/news-detail/learn-quantum-computing-proven-ways-for-beginners20250120032606](https://www.spinquanta.com/news-detail/learn-quantum-computing-proven-ways-for-beginners20250120032606)  
16. Linear Algebra for Quantum Computation, accessed October 1, 2025, [https://ucilnica.fri.uni-lj.si/pluginfile.php/572/course/section/6045/linear\_algebra\_from\_quantum\_computation.pdf](https://ucilnica.fri.uni-lj.si/pluginfile.php/572/course/section/6045/linear_algebra_from_quantum_computation.pdf)  
17. Vectors & Matrices in Quantum Computing \- Azure Quantum \- Microsoft Learn, accessed October 1, 2025, [https://learn.microsoft.com/en-us/azure/quantum/concepts-vectors-and-matrices](https://learn.microsoft.com/en-us/azure/quantum/concepts-vectors-and-matrices)  
18. Introduction to Quantum Computing \- MIT xPRO, accessed October 1, 2025, [https://xpro.mit.edu/courses/course-v1:xPRO+QCFx1/](https://xpro.mit.edu/courses/course-v1:xPRO+QCFx1/)  
19. Introduction to Linear Algebra, Prerequisite Mathematics, and Circuit Composition \- Part 1, accessed October 1, 2025, [https://www.youtube.com/watch?v=ZNz7DN1K0Y0](https://www.youtube.com/watch?v=ZNz7DN1K0Y0)  
20. Quantum Computing Course – Math and Theory for Beginners \- YouTube, accessed October 1, 2025, [https://www.youtube.com/watch?v=tsbCSkvHhMo](https://www.youtube.com/watch?v=tsbCSkvHhMo)  
21. Quantum Computing For Dummies by Whurley | Goodreads, accessed October 1, 2025, [https://www.goodreads.com/book/show/61720018-quantum-computing-for-dummies](https://www.goodreads.com/book/show/61720018-quantum-computing-for-dummies)  
22. IBM Quantum Learning, accessed October 1, 2025, [https://quantum.cloud.ibm.com/learning](https://quantum.cloud.ibm.com/learning)  
23. IBM Quantum Platform, accessed October 1, 2025, [https://quantum.cloud.ibm.com/](https://quantum.cloud.ibm.com/)  
24. Learn quantum computing | Q-CTRL, accessed October 1, 2025, [https://q-ctrl.com/black-opal](https://q-ctrl.com/black-opal)  
25. Top Quantum Educational Solutions: Tools, Courses, & More \- SpinQ, accessed October 1, 2025, [https://www.spinquanta.com/news-detail/top-quantum-educational-solutions-tools-courses-more20250115020652](https://www.spinquanta.com/news-detail/top-quantum-educational-solutions-tools-courses-more20250115020652)  
26. Best quantum computing courses and programs | edX, accessed October 1, 2025, [https://www.edx.org/learn/quantum-computing](https://www.edx.org/learn/quantum-computing)  
27. Best Quantum Computing Courses & Certificates \[2025\] | Coursera ..., accessed October 1, 2025, [https://www.coursera.org/courses?query=quantum%20computing](https://www.coursera.org/courses?query=quantum+computing)  
28. The Complete Quantum Computing Course for Beginners Specialization \- Coursera, accessed October 1, 2025, [https://www.coursera.org/specializations/packt-the-complete-quantum-computing-course-for-beginners](https://www.coursera.org/specializations/packt-the-complete-quantum-computing-course-for-beginners)  
29. Learn-Quantum-Computing-For-Free, accessed October 1, 2025, [https://monitsharma.github.io/Learn-Quantum-Computing-For-Free/](https://monitsharma.github.io/Learn-Quantum-Computing-For-Free/)  
30. Quantum Machine Learning: What It Is, How It Works, and More | Coursera, accessed October 1, 2025, [https://www.coursera.org/articles/quantum-machine-learning](https://www.coursera.org/articles/quantum-machine-learning)  
31. PennyLane \- Xanadu, accessed October 1, 2025, [https://www.xanadu.ai/products/pennylane/](https://www.xanadu.ai/products/pennylane/)  
32. PennyLane \- Alliance Doc, accessed October 1, 2025, [https://docs.alliancecan.ca/wiki/PennyLane/en](https://docs.alliancecan.ca/wiki/PennyLane/en)  
33. IBM Quantum Computing | Qiskit, accessed October 1, 2025, [https://www.ibm.com/quantum/qiskit](https://www.ibm.com/quantum/qiskit)  
34. Qiskit \- Wikipedia, accessed October 1, 2025, [https://en.wikipedia.org/wiki/Qiskit](https://en.wikipedia.org/wiki/Qiskit)  
35. Cirq | Google Quantum AI, accessed October 1, 2025, [https://quantumai.google/cirq](https://quantumai.google/cirq)  
36. quantumlib/Cirq: Python framework for creating, editing, and invoking Noisy Intermediate-Scale Quantum (NISQ) circuits. \- GitHub, accessed October 1, 2025, [https://github.com/quantumlib/Cirq](https://github.com/quantumlib/Cirq)  
37. Quantum Programming Software — PennyLane, accessed October 1, 2025, [https://pennylane.ai/](https://pennylane.ai/)  
38. Quantum Algorithms Guide: Principles, Types, and Use Cases \- SpinQ, accessed October 1, 2025, [https://www.spinquanta.com/news-detail/the-ultimate-guide-to-quantum-algorithms](https://www.spinquanta.com/news-detail/the-ultimate-guide-to-quantum-algorithms)  
39. Quantum phase estimation algorithm \- Wikipedia, accessed October 1, 2025, [https://en.wikipedia.org/wiki/Quantum\_phase\_estimation\_algorithm](https://en.wikipedia.org/wiki/Quantum_phase_estimation_algorithm)  
40. HHL Algorithm for Linear Systems of Equations \- PhysLab, accessed October 1, 2025, [https://physlab.org/wp-content/uploads/2023/05/HHL\_22120009\_Fin.pdf](https://physlab.org/wp-content/uploads/2023/05/HHL_22120009_Fin.pdf)  
41. Quantum Fourier transform \- Wikipedia, accessed October 1, 2025, [https://en.wikipedia.org/wiki/Quantum\_Fourier\_transform](https://en.wikipedia.org/wiki/Quantum_Fourier_transform)  
42. An approximate Fourier transform useful in quantum factoring, accessed October 1, 2025, [https://arxiv.org/abs/quant-ph/0201067](https://arxiv.org/abs/quant-ph/0201067)  
43. What is the quantum Fourier transform, and how does it speed up quantum algorithms?, accessed October 1, 2025, [https://milvus.io/ai-quick-reference/what-is-the-quantum-fourier-transform-and-how-does-it-speed-up-quantum-algorithms](https://milvus.io/ai-quick-reference/what-is-the-quantum-fourier-transform-and-how-does-it-speed-up-quantum-algorithms)  
44. Chapter 5 \- QFT, Period Finding & Shor's Algorithm \- edX, accessed October 1, 2025, [https://courses.edx.org/c4x/BerkeleyX/CS191x/asset/chap5.pdf](https://courses.edx.org/c4x/BerkeleyX/CS191x/asset/chap5.pdf)  
45. Quantum Fourier Transform — Computing in Physics (498CMP), accessed October 1, 2025, [https://courses.physics.illinois.edu/phys498cmp/sp2022/QC/QFT.html](https://courses.physics.illinois.edu/phys498cmp/sp2022/QC/QFT.html)  
46. Quantum Algorithm (1): Shor's algorithm for factorization — part 1 | by QUANTUMPEDIA \- The Quantum Encyclopedia | Medium, accessed October 1, 2025, [https://quantumpedia.uk/quantum-algorithm-1-shors-algorithm-for-factorization-part-1-cffcb4f0d0c1](https://quantumpedia.uk/quantum-algorithm-1-shors-algorithm-for-factorization-part-1-cffcb4f0d0c1)  
47. Tutorial: Quantum Fourier Transform in Q\\\# \- Azure Quantum \- Microsoft Learn, accessed October 1, 2025, [https://learn.microsoft.com/en-us/azure/quantum/tutorial-qdk-qubit-level-program](https://learn.microsoft.com/en-us/azure/quantum/tutorial-qdk-qubit-level-program)  
48. Intro to Quantum Fourier Transform | PennyLane Demos, accessed October 1, 2025, [https://pennylane.ai/qml/demos/tutorial\_qft/](https://pennylane.ai/qml/demos/tutorial_qft/)  
49. Quantum measurements and the Abelian Stabilizer Problem, accessed October 1, 2025, [https://arxiv.org/pdf/quant-ph/9511026](https://arxiv.org/pdf/quant-ph/9511026)  
50. Intro to Quantum Phase Estimation | PennyLane Demos, accessed October 1, 2025, [https://pennylane.ai/qml/demos/tutorial\_qpe](https://pennylane.ai/qml/demos/tutorial_qpe)  
51. Quantum Phase Estimation (QPE) \- Classiq, accessed October 1, 2025, [https://www.classiq.io/insights/quantum-phase-estimation-qpe](https://www.classiq.io/insights/quantum-phase-estimation-qpe)  
52. 2-4. Phase Estimation Algorithm (Introduction) \- Quantum Native Dojo\! \- Qulacs, accessed October 1, 2025, [https://dojo.qulacs.org/en/latest/notebooks/2.4\_phase\_estimation\_beginner.html](https://dojo.qulacs.org/en/latest/notebooks/2.4_phase_estimation_beginner.html)  
53. Quantum Phase Estimation in Qiskit — Quantum Computing UK, accessed October 1, 2025, [https://quantumcomputinguk.org/tutorials/quantum-phase-estimation-with-code](https://quantumcomputinguk.org/tutorials/quantum-phase-estimation-with-code)  
54. Textbook algorithms in Cirq | Google Quantum AI, accessed October 1, 2025, [https://quantumai.google/cirq/experiments/textbook\_algorithms](https://quantumai.google/cirq/experiments/textbook_algorithms)  
55. Shor's algorithm \- Wikipedia, accessed October 1, 2025, [https://en.wikipedia.org/wiki/Shor%27s\_algorithm](https://en.wikipedia.org/wiki/Shor%27s_algorithm)  
56. Peter Shor's Publications \- MIT Mathematics, accessed October 1, 2025, [https://math.mit.edu/\~shor/elecpubs.html](https://math.mit.edu/~shor/elecpubs.html)  
57. Algorithms for quantum computation: discrete logarithms and factoring, accessed October 1, 2025, [https://cc.ee.ntu.edu.tw/\~rbwu/rapid\_content/course/QC/Shor1994.pdf](https://cc.ee.ntu.edu.tw/~rbwu/rapid_content/course/QC/Shor1994.pdf)  
58. Factoring integers using Shor's Algorithm — documentation \- Qrisp, accessed October 1, 2025, [https://qrisp.eu/general/tutorial/Shor.html](https://qrisp.eu/general/tutorial/Shor.html)  
59. How Shor's Algorithm Breaks RSA: A Quantum Computing Guide \- SpinQ, accessed October 1, 2025, [https://www.spinquanta.com/news-detail/shors-algorithm](https://www.spinquanta.com/news-detail/shors-algorithm)  
60. Shor's algorithm | IBM Quantum Documentation, accessed October 1, 2025, [https://quantum.cloud.ibm.com/docs/en/tutorials/shors-algorithm](https://quantum.cloud.ibm.com/docs/en/tutorials/shors-algorithm)  
61. Shor's algorithm | Cirq \- Google Quantum AI, accessed October 1, 2025, [https://quantumai.google/cirq/experiments/shor](https://quantumai.google/cirq/experiments/shor)  
62. Grover's algorithm \- Wikipedia, accessed October 1, 2025, [https://en.wikipedia.org/wiki/Grover%27s\_algorithm](https://en.wikipedia.org/wiki/Grover%27s_algorithm)  
63. Tight bounds on quantum searching, accessed October 1, 2025, [https://arxiv.org/pdf/quant-ph/9605034](https://arxiv.org/pdf/quant-ph/9605034)  
64. Theory of Grover Search Algorithm \- Azure Quantum | Microsoft Learn, accessed October 1, 2025, [https://learn.microsoft.com/en-us/azure/quantum/concepts-grovers](https://learn.microsoft.com/en-us/azure/quantum/concepts-grovers)  
65. Introduction to Grover's Algorithm \- GeeksforGeeks, accessed October 1, 2025, [https://www.geeksforgeeks.org/dsa/introduction-to-grovers-algorithm/](https://www.geeksforgeeks.org/dsa/introduction-to-grovers-algorithm/)  
66. Introduction | IBM Quantum Learning, accessed October 1, 2025, [https://quantum.cloud.ibm.com/learning/courses/fundamentals-of-quantum-algorithms/grover-algorithm/introduction](https://quantum.cloud.ibm.com/learning/courses/fundamentals-of-quantum-algorithms/grover-algorithm/introduction)  
67. Grover's algorithm | IBM Quantum Documentation, accessed October 1, 2025, [https://quantum.cloud.ibm.com/docs/tutorials/grovers-algorithm](https://quantum.cloud.ibm.com/docs/tutorials/grovers-algorithm)  
68. Quantum Computing: Grover's Algorithm (CIRQ) \- Kaggle, accessed October 1, 2025, [https://www.kaggle.com/code/viratkothari/quantum-computing-grover-s-algorithm-cirq](https://www.kaggle.com/code/viratkothari/quantum-computing-grover-s-algorithm-cirq)  
69. Grover's Algorithm | PennyLane Demos, accessed October 1, 2025, [https://pennylane.ai/qml/demos/tutorial\_grovers\_algorithm](https://pennylane.ai/qml/demos/tutorial_grovers_algorithm)  
70. HHL algorithm \- Wikipedia, accessed October 1, 2025, [https://en.wikipedia.org/wiki/HHL\_algorithm](https://en.wikipedia.org/wiki/HHL_algorithm)  
71. Solving Linear Systems of Equations with the Quantum HHL ... \- arXiv, accessed October 1, 2025, [https://arxiv.org/pdf/2509.16640](https://arxiv.org/pdf/2509.16640)  
72. Quantum Algorithm for Linear Systems of Equations | Phys. Rev. Lett., accessed October 1, 2025, [https://link.aps.org/doi/10.1103/PhysRevLett.103.150502](https://link.aps.org/doi/10.1103/PhysRevLett.103.150502)  
73. HHL Algorithm \- QuantumGrad, accessed October 1, 2025, [https://www.quantumgrad.com/article/462](https://www.quantumgrad.com/article/462)  
74. HHL algorithm \- isQ Compiler Docs, accessed October 1, 2025, [https://www.arclightquantum.com/isq-docs/latest/examples/hhl/](https://www.arclightquantum.com/isq-docs/latest/examples/hhl/)  
75. Teaching material Cirq \- quantum algorithms and tutorials A hands-on tutorial about writing quantum algorithms in Cirq. Cirq is an open-source Python library that enables you to run quantum algorithms on quantum computers and simulators from Google and \- QTEdu, accessed October 1, 2025, [https://qtedu.eu/material/cirq-quantum-algorithms-and-tutorials](https://qtedu.eu/material/cirq-quantum-algorithms-and-tutorials)  
76. Solving linear system problems with HHL — documentation \- Qrisp, accessed October 1, 2025, [https://qrisp.eu/general/tutorial/HHL.html](https://qrisp.eu/general/tutorial/HHL.html)  
77. Variational quantum eigensolver \- Wikipedia, accessed October 1, 2025, [https://en.wikipedia.org/wiki/Variational\_quantum\_eigensolver](https://en.wikipedia.org/wiki/Variational_quantum_eigensolver)  
78. A variational eigenvalue solver on a quantum processor, accessed October 1, 2025, [https://arxiv.org/abs/1304.3061](https://arxiv.org/abs/1304.3061)  
79. Measurement-Based Variational Quantum Eigensolver | Phys. Rev. Lett., accessed October 1, 2025, [https://link.aps.org/doi/10.1103/PhysRevLett.126.220501](https://link.aps.org/doi/10.1103/PhysRevLett.126.220501)  
80. Experiments using quantum circuits | Cirq, accessed October 1, 2025, [https://quantumai.google/cirq/experiments](https://quantumai.google/cirq/experiments)  
81. Variational Quantum Eigensolver (VQE) | PennyLane Tutorial \- YouTube, accessed October 1, 2025, [https://www.youtube.com/watch?v=qiRtUUZ5s9s](https://www.youtube.com/watch?v=qiRtUUZ5s9s)  
82. A brief overview of VQE | PennyLane Demos, accessed October 1, 2025, [https://pennylane.ai/qml/demos/tutorial\_vqe/](https://pennylane.ai/qml/demos/tutorial_vqe/)  
83. A Quantum Approximate Optimization Algorithm \- Green Compute UK, accessed October 1, 2025, [https://arxiv.org/abs/1411.4028](https://arxiv.org/abs/1411.4028)  
84. QAOA and optimization \- Demos \- Discussion Forum — PennyLane, accessed October 1, 2025, [https://discuss.pennylane.ai/t/qaoa-and-optimization/5188](https://discuss.pennylane.ai/t/qaoa-and-optimization/5188)  
85. \[PDF\] A Quantum Approximate Optimization Algorithm | Semantic Scholar, accessed October 1, 2025, [https://www.semanticscholar.org/paper/A-Quantum-Approximate-Optimization-Algorithm-Farhi-Goldstone/ea238b034c2042fc0ce4efcff288725e5e74f462](https://www.semanticscholar.org/paper/A-Quantum-Approximate-Optimization-Algorithm-Farhi-Goldstone/ea238b034c2042fc0ce4efcff288725e5e74f462)  
86. Intro to QAOA | PennyLane Demos, accessed October 1, 2025, [https://pennylane.ai/qml/demos/tutorial\_qaoa\_intro/](https://pennylane.ai/qml/demos/tutorial_qaoa_intro/)  
87. Recommendation for Quantum Computing textbook : r/QuantumComputing \- Reddit, accessed October 1, 2025, [https://www.reddit.com/r/QuantumComputing/comments/172v9h7/recommendation\_for\_quantum\_computing\_textbook/](https://www.reddit.com/r/QuantumComputing/comments/172v9h7/recommendation_for_quantum_computing_textbook/)  
88. Quantum computing \- GW Engineering, accessed October 1, 2025, [https://www2.seas.gwu.edu/\~simhaweb/quantum/modules/appendix/reading.html](https://www2.seas.gwu.edu/~simhaweb/quantum/modules/appendix/reading.html)  
89. The Best Quantum Computing Books | Five Books Expert ..., accessed October 1, 2025, [https://fivebooks.com/best-books/quantum-computing-chris-bernhardt/](https://fivebooks.com/best-books/quantum-computing-chris-bernhardt/)  
90. Books \- Quantum Computing Report, accessed October 1, 2025, [https://quantumcomputingreport.com/books/](https://quantumcomputingreport.com/books/)  
91. Quantum Computing Book Recommendations \- YouTube, accessed October 1, 2025, [https://www.youtube.com/watch?v=xpSevVullcQ](https://www.youtube.com/watch?v=xpSevVullcQ)  
92. Popular Quantum Computing Books \- Goodreads, accessed October 1, 2025, [https://www.goodreads.com/shelf/show/quantum-computing](https://www.goodreads.com/shelf/show/quantum-computing)  
93. The Best Quantum Books: Learn How To "Quantum" From The Best ..., accessed October 1, 2025, [https://quantumzeitgeist.com/the-best-quantum-books/](https://quantumzeitgeist.com/the-best-quantum-books/)  
94. Quantum Computation | Mathematics | MIT OpenCourseWare, accessed October 1, 2025, [https://ocw.mit.edu/courses/18-435j-quantum-computation-fall-2003/](https://ocw.mit.edu/courses/18-435j-quantum-computation-fall-2003/)  
95. Quantum Complexity Theory | Electrical Engineering and Computer Science, accessed October 1, 2025, [https://ocw.mit.edu/courses/6-845-quantum-complexity-theory-fall-2010/](https://ocw.mit.edu/courses/6-845-quantum-complexity-theory-fall-2010/)  
96. Unit 13: Quantum Information | Information and Entropy | Electrical Engineering and Computer Science | MIT OpenCourseWare, accessed October 1, 2025, [https://ocw.mit.edu/courses/6-050j-information-and-entropy-spring-2008/pages/quantum-information/](https://ocw.mit.edu/courses/6-050j-information-and-entropy-spring-2008/pages/quantum-information/)  
97. Chapter 5: Quantum Computing | Quantum Physics III \- MIT OpenCourseWare, accessed October 1, 2025, [https://ocw.mit.edu/courses/8-06-quantum-physics-iii-spring-2016/resources/mit8\_06s16\_chap5/](https://ocw.mit.edu/courses/8-06-quantum-physics-iii-spring-2016/resources/mit8_06s16_chap5/)  
98. Quantum Mechanics for Scientists and Engineers I Stanford Online, accessed October 1, 2025, [https://online.stanford.edu/courses/soe-yeeqmse01-quantum-mechanics-scientists-and-engineers](https://online.stanford.edu/courses/soe-yeeqmse01-quantum-mechanics-scientists-and-engineers)  
99. What are the best structured courses available online on quantum computing?, accessed October 1, 2025, [https://quantumcomputing.stackexchange.com/questions/2667/what-are-the-best-structured-courses-available-online-on-quantum-computing](https://quantumcomputing.stackexchange.com/questions/2667/what-are-the-best-structured-courses-available-online-on-quantum-computing)  
100. Top three Quantum Computing books you've ever read? : r/QuantumComputing \- Reddit, accessed October 1, 2025, [https://www.reddit.com/r/QuantumComputing/comments/1apd32t/top\_three\_quantum\_computing\_books\_youve\_ever\_read/](https://www.reddit.com/r/QuantumComputing/comments/1apd32t/top_three_quantum_computing_books_youve_ever_read/)  
101. Lecture Series: Introduction to Quantum Computers \- IonQ, accessed October 1, 2025, [https://ionq.com/resources/anthology/lecture-series-introduction-to-quantum-computers](https://ionq.com/resources/anthology/lecture-series-introduction-to-quantum-computers)  
102. A comprehensive review of Quantum Machine Learning: from NISQ to Fault Tolerance, accessed October 1, 2025, [https://arxiv.org/html/2401.11351v2](https://arxiv.org/html/2401.11351v2)  
103. \[2401.11351\] A comprehensive review of Quantum Machine Learning: from NISQ to Fault Tolerance \- arXiv, accessed October 1, 2025, [https://arxiv.org/abs/2401.11351](https://arxiv.org/abs/2401.11351)  
104. \[2502.01146\] Quantum Machine Learning: A Hands-on Tutorial for Machine Learning Practitioners and Researchers \- arXiv, accessed October 1, 2025, [https://arxiv.org/abs/2502.01146](https://arxiv.org/abs/2502.01146)  
105. Google Quantum AI, accessed October 1, 2025, [https://quantumai.google/](https://quantumai.google/)  
106. Los Alamos researchers unlock quantum machine learning, accessed October 1, 2025, [https://www.innovationnewsnetwork.com/los-alamos-unlock-quantum-machine-learning/60162/](https://www.innovationnewsnetwork.com/los-alamos-unlock-quantum-machine-learning/60162/)  
107. \[0905.2794\] Quantum Error Correction for Beginners \- arXiv, accessed October 1, 2025, [https://arxiv.org/abs/0905.2794](https://arxiv.org/abs/0905.2794)  
108. Quantum Error Correction: the grand challenge \- Riverlane, accessed October 1, 2025, [https://www.riverlane.com/quantum-error-correction](https://www.riverlane.com/quantum-error-correction)  
109. Quantum Error Correction: An Introductory Guide, accessed October 1, 2025, [https://arxiv.org/abs/1907.11157](https://arxiv.org/abs/1907.11157)  
110. \[2304.08678\] Quantum Error Correction For Dummies \- arXiv, accessed October 1, 2025, [https://arxiv.org/abs/2304.08678](https://arxiv.org/abs/2304.08678)  
111. Guest Post: What's Next for Quantum Error Correction?, accessed October 1, 2025, [https://thequantuminsider.com/2025/02/08/guest-post-whats-next-for-quantum-error-correction/](https://thequantuminsider.com/2025/02/08/guest-post-whats-next-for-quantum-error-correction/)  
112. Quantum error correction below the surface code threshold \- arXiv, accessed October 1, 2025, [https://arxiv.org/html/2408.13687v1](https://arxiv.org/html/2408.13687v1)  
113. Quantinuum with partners Princeton and NIST deliver seminal result in quantum error correction, accessed October 1, 2025, [https://www.quantinuum.com/blog/quantinuum-with-partners-princeton-and-nist-deliver-seminal-result-in-quantum-error-correction](https://www.quantinuum.com/blog/quantinuum-with-partners-princeton-and-nist-deliver-seminal-result-in-quantum-error-correction)  
114. Microsoft advances quantum error correction with a family of novel four-dimensional codes, accessed October 1, 2025, [https://azure.microsoft.com/en-us/blog/quantum/2025/06/19/microsoft-advances-quantum-error-correction-with-a-family-of-novel-four-dimensional-codes/](https://azure.microsoft.com/en-us/blog/quantum/2025/06/19/microsoft-advances-quantum-error-correction-with-a-family-of-novel-four-dimensional-codes/)  
115. Quantum Advantage in Cryptography \- arXiv, accessed October 1, 2025, [https://arxiv.org/pdf/2206.04078](https://arxiv.org/pdf/2206.04078)  
116. A tertiary review on quantum cryptography \- arXiv, accessed October 1, 2025, [https://arxiv.org/html/2506.02028v1](https://arxiv.org/html/2506.02028v1)  
117. Planning for post-quantum cryptography | Cyber.gov.au, accessed October 1, 2025, [https://www.cyber.gov.au/business-government/secure-design/planning-for-post-quantum-cryptography](https://www.cyber.gov.au/business-government/secure-design/planning-for-post-quantum-cryptography)  
118. Quantum Computing Moves from Theoretical to Inevitable | Bain & Company, accessed October 1, 2025, [https://www.bain.com/insights/quantum-computing-moves-from-theoretical-to-inevitable-technology-report-2025/](https://www.bain.com/insights/quantum-computing-moves-from-theoretical-to-inevitable-technology-report-2025/)  
119. \[1906.01645\] Advances in Quantum Cryptography \- arXiv, accessed October 1, 2025, [https://arxiv.org/abs/1906.01645](https://arxiv.org/abs/1906.01645)  
120. \[2102.00021\] Security in Quantum Cryptography \- arXiv, accessed October 1, 2025, [https://arxiv.org/abs/2102.00021](https://arxiv.org/abs/2102.00021)  
121. \[1510.06120\] Quantum Cryptography Beyond Quantum Key Distribution \- arXiv, accessed October 1, 2025, [https://arxiv.org/abs/1510.06120](https://arxiv.org/abs/1510.06120)  
122. Resources to get started programming quantum computers for non-physics majors, accessed October 1, 2025, [https://quantumcomputing.stackexchange.com/questions/1367/resources-to-get-started-programming-quantum-computers-for-non-physics-majors](https://quantumcomputing.stackexchange.com/questions/1367/resources-to-get-started-programming-quantum-computers-for-non-physics-majors)  
123. Quantum Computing Stack Exchange, accessed October 1, 2025, [https://quantumcomputing.stackexchange.com/](https://quantumcomputing.stackexchange.com/)  
124. Getting into Quantum Computing as a beginner : r/QuantumComputing \- Reddit, accessed October 1, 2025, [https://www.reddit.com/r/QuantumComputing/comments/17xu6j5/getting\_into\_quantum\_computing\_as\_a\_beginner/](https://www.reddit.com/r/QuantumComputing/comments/17xu6j5/getting_into_quantum_computing_as_a_beginner/)  
125. Quantum Computing \- Reddit, accessed October 1, 2025, [https://www.reddit.com/r/QuantumComputing/](https://www.reddit.com/r/QuantumComputing/)  
126. The Quantum Insider: Quantum Computing News & Top Stories, accessed October 1, 2025, [https://thequantuminsider.com/](https://thequantuminsider.com/)  
127. Daily \- The Quantum Insider, accessed October 1, 2025, [https://thequantuminsider.com/category/daily/](https://thequantuminsider.com/category/daily/)  
128. Quantum Zeitgeist \- Daily Quantum Computing News & Analysis, accessed October 1, 2025, [https://quantumzeitgeist.com/](https://quantumzeitgeist.com/)  
129. Quantum Computing Report \- Market Analysis, News & Resources, accessed October 1, 2025, [https://quantumcomputingreport.com/](https://quantumcomputingreport.com/)  
130. Shtetl-Optimized, accessed October 1, 2025, [https://scottaaronson.blog/](https://scottaaronson.blog/)  
131. AWS Quantum Technologies Blog, accessed October 1, 2025, [https://aws.amazon.com/blogs/quantum-computing/](https://aws.amazon.com/blogs/quantum-computing/)  
132. Blog \- Q-munity \- The Quantum Insider, accessed October 1, 2025, [https://qmunity.thequantuminsider.com/blog/](https://qmunity.thequantuminsider.com/blog/)  
133. Quantum Community \- IBM Research, accessed October 1, 2025, [https://research.ibm.com/topics/quantum-community](https://research.ibm.com/topics/quantum-community)  
134. IBM Quantum Computing | Community, accessed October 1, 2025, [https://www.ibm.com/quantum/community](https://www.ibm.com/quantum/community)  
135. Quantum Community \- Pasqal, accessed October 1, 2025, [https://www.pasqal.com/community/](https://www.pasqal.com/community/)  
136. Quantum Computing groups \- Meetup, accessed October 1, 2025, [https://www.meetup.com/topics/quantum/us/](https://www.meetup.com/topics/quantum/us/)

[image1]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAMgAAADICAYAAACtWK6eAAAAsUlEQVR4Xu3BAQEAAACCIP+vbkhAAQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAB8GXHmAAEdo+NeAAAAAElFTkSuQmCC>