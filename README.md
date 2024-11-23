# Maximum Coverage in Random-Arrival Streams

**INFO-F440: Algorithms for Big Data (2023/24) - ULB**  
Work: Herma Elezi , Nicolas Bongay

<div align="center">
    <img src="https://actus.ulb.be/medias/photo/logo-universite-libre-bruxelles_1661952138925-png?ID_FICHE=19524" alt="ULB Logo" width="300"/>
</div>

This repository provides implementations and analysis of algorithms for solving the **Maximum Coverage Problem** in random-arrival streaming models. The Maximum Coverage Problem involves selecting `k` sets from a collection such that their union has the largest cardinality. This problem is relevant in domains such as facility allocation, content recommendation, and data summarization.

---

## Features

- **MV-4 Algorithm**: A set-streaming algorithm designed for arbitrary-arrival streams, achieving a `1/2 − ε` approximation with sublinear space.
- **SALSA Algorithm**: A streaming algorithm offering a `1/2 + c₀` approximation for random-arrival streams.
- **GS-SALSA**: Generalized subsampling of SALSA, improving approximation factors in random-arrival models while maintaining low space complexity.

---

## Algorithms Overview

| Algorithm | Model           | Approximation Factor   | Space Complexity     |
|-----------|-----------------|------------------------|----------------------|
| MV-4      | Arbitrary-Arrival | `1/2 − ε`             | `Õ(kε⁻³)`           |
| SALSA     | Random-Arrival   | `1/2 + c₀`            | `Õ(k²)`             |
| GS-SALSA  | Random-Arrival   | `1 − 1/e − ε − o(1)`   | `Õ(k²ε⁻³)`          |

---


## References

1. **Andrew McGregor and Hoa T Vu**: *Better Streaming Algorithms for the Maximum Coverage Problem*, 2019.
2. **Shipra Agrawal et al.**: *Submodular Maximization on Massive Data Streams*, 2018.
3. **Ashkan Norouzi-Fard et al.**: *Beyond 1/2-Approximation for Submodular Maximization*, 2018.

