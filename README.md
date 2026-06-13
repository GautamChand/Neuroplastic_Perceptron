# Neuroplastic_Perceptron
An experimental machine learning research project investigating whether connectivity can become a learnable component of neural networks through mathematically defined neuroplasticity rules.
# Neuroplastic Perceptron: Beyond Sparse Training

> **Can connectivity become a learnable component of neural networks rather than a fixed architectural choice?**

---

<p align="center">
  <img src="https://img.shields.io/badge/Project%20Status-Active%20Research-blueviolet?style=for-the-badge" alt="Project Status"/>
  <img src="https://img.shields.io/badge/Category-Deep%20Learning-blue?style=for-the-badge" alt="Category"/>
  <img src="https://img.shields.io/badge/Focus-Neuroplasticity%20%26%20Sparse%20Training-orange?style=for-the-badge" alt="Focus"/>
</p>

---

## 1. Introduction & Research Vision

Artificial neural networks (ANNs) have achieved remarkable success across diverse domains. Advances in computing power, massive datasets, and sophisticated optimization techniques enable models to solve increasingly complex problems. 

However, modern architectures rely on a fundamental design assumption: **the network architecture is largely static, while learning occurs almost exclusively through optimization of weight parameters.**

Biological neural systems operate fundamentally differently. The human brain continuously adapts its internal topology through **neuroplasticity**. Connections between neurons strengthen, weaken, emerge, or disappear entirely based on experience, stimulus, and usage. In biological brains, learning is not limited to adjusting connection strengths—it actively shapes the wiring diagram itself.

This project investigates whether we can bridge this gap by treating network connectivity as a dynamic, learnable state variable.

---

## 2. Dynamic vs. Static Connectivity

Traditional deep learning models optimize a set of weights $W = \{w_1, w_2, \dots, w_n\}$ within a fixed, pre-defined topology graph:

```mermaid
graph LR
    subgraph "Traditional Fixed Architecture"
        A((Input 1)) -->|W₁| C((Neuron))
        B((Input 2)) -->|W₂| C
    end
itional NNs, DST, and your hypothesis to allow readers to immediately grasp the novelty.
5. **Formatted Roadmap:** Transformed the phases into a clean, text-based visual roadmap.

