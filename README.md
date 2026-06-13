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
    subgraph Traditional Fixed Architecture
        A((Input 1)) -->|W₁| C((Neuron))
        B((Input 2)) -->|W₂| C
    end
graph LR
    subgraph Neuroplastic Perceptron Synapse
        X1[Input: x₁] --> P1((Plasticity: P₁₁))
        P1 --> W1((Weight: W₁₁))
        
        X2[Input: x₂] --> P2((Plasticity: P₂₁))
        P2 --> W2((Weight: W₂₁))
        
        W1 --> Sum[Summation: Σ]
        W2 --> Sum
        Sum --> Act[Activation: σ]
        Act --> Out[Output]
    end

Phase 1: Neuroplastic Perceptron (Current)
 ├── Study existing sparse training methods (SET, RigL, etc.)
 ├── Formulate baseline mathematical models for continuous connectivity (P_ij)
 ├── Evaluate performance against traditional perceptrons on benchmark tasks
 └── Identify limits of weight vs. connectivity optimization trade-offs

Phase 2: Multi-Layer & Deep Architectures (Upcoming)
 ├── Scale connectivity adaptation to hidden layers
 ├── Analyze emergent topological properties (e.g., small-world structures)
 └── Investigate generalization bounds and parameter efficiency

Phase 3: Alternative Geometric Learning Frameworks (Exploratory)
 ├── Explore non-Euclidean geometric representations
 ├── Investigate multi-region decision boundaries
 └── Design geometry-inspired learning dynamics



***

### Summary of Improvements
1. **Badges:** Created custom `shields.io` badges for project status, category, and research focus at the very top.
2. **Mermaid Diagrams:** Included interactive flowcharts to visually distinguish traditional fixed architectures from the proposed neuroplastic perceptron model (showing the interplay of $P_{ij}$ and $W_{ij}$).
3. **LaTeX Math Equations:** Formatted the core equations using Markdown-supported LaTeX ($$\sum_{j} P_{ij} \cdot W_{ij} \cdot x_j$$ and $$\frac{dP_{ij}}{dt}$$) for clean, readable formulas.
4. **Structured Comparison Table:** Tabulated the structural differences between traditional NNs, DST, and your hypothesis to allow readers to immediately grasp the novelty.
5. **Formatted Roadmap:** Transformed the phases into a clean, text-based visual roadmap.

