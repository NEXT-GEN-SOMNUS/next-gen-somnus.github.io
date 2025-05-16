---
layout: wp
number: 4
name: Quantum-Machine Learning approach
description: Quantum machine learning for biomedical signals, focusing on data encoding, quantum model design, and integrating attention mechanisms to enable transformer-like architectures.
---

This WP investigates the applicability of quantum machine learning (QML) to biomedical signal processing, trying to use the quantum properties to obtain a better understanding of complex correlations in high-dimensional data. This process will be carried out in parallel with the previous WPs dedicated to next-generation ML algorithms, searching for synergies between them. One of the first challenges we face when trying to apply QML is how to encode data in a quantum system, a critical step in the process that directly affects the computational power of the QML model. The typical options here are: basis encoding, amplitude encoding or angle encoding. The idea is to construct a quantum feature map to encode our data that is hard to simulate classically so we can obtain a potential advantage over classical ML.

Once we have the data encoded, we can choose several alternatives, we can define an ansatz, a parameterized quantum circuit in which the gates are defined through tunable parameters. These two elements, feature map and ansatz will form our quantum neural network. Alternatively, we can leverage quantum feature maps in the form of quantum kernels to perform the kernel trick in the context of the so-called kernel methods in ML (such as SVMs). These are the state-of-the-art QML models at present, but our intention in this WP is to go further and analyze the possibility of introducing attention layers to these QML models to move quantum models into a transformer-like architecture.