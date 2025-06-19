# PortOpt

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Qiskit](https://img.shields.io/badge/Qiskit-0.39.0-brightgreen)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.x-orange)
![Pandas](https://img.shields.io/badge/Pandas-1.x-lightgrey)
![Numpy](https://img.shields.io/badge/Numpy-1.x-lightgrey)

## Overview

This project explores **quantum portfolio optimization** using both classical and quantum techniques. It includes:

1. **Hierarchical Risk Parity (HRP)** model for portfolio construction.
2. **Efficient Frontier** from **Modern Portfolio Theory (MPT)** to analyze the optimal portfolio.
3. Quantum algorithms from **Qiskit**, specifically the **Quantum Approximate Optimization Algorithm (QAOA)** and **Sampling Variational Quantum Eigensolver (SamplingVQE)**.

The analysis is conducted on stock data from four companies under the **Nifty50** index.

## Dataset

The dataset consists of stock prices for companies listed under the **Nifty50** index. The stock data is used to compute returns, covariance matrices, and other metrics necessary for portfolio optimization.

## Classical Approaches

### 1. Hierarchical Risk Parity (HRP)
Hierarchical Risk Parity is a portfolio optimization method that groups assets into clusters using machine learning techniques and allocates weights based on their hierarchical structure. It does not rely on assumptions of asset returns' normality, making it robust for non-linear relationships.

### 2. Efficient Frontier under MPT
The **Efficient Frontier**, derived from **Modern Portfolio Theory (MPT)**, is a curve representing the set of optimal portfolios that offer the highest expected return for a defined level of risk. This method helps in identifying the portfolio that maximizes returns while minimizing risk.

## Quantum Approaches

### 1. Quantum Approximate Optimization Algorithm (QAOA)
QAOA is a quantum algorithm designed to solve combinatorial optimization problems by alternating between quantum and classical optimization processes. It is particularly suited for constrained optimization tasks such as portfolio optimization.

### 2. Sampling Variational Quantum Eigensolver (SamplingVQE)
SamplingVQE is another quantum variational algorithm aimed at solving optimization problems by approximating the lowest energy (or cost) of a system. It leverages quantum circuits and classical optimization routines to find solutions to portfolio optimization challenges.

## Installation

To install the required packages, run the following command:

```bash
pip install -r requirements.txt
```

## Quantum Backend

This project uses **Qiskit** for implementing quantum algorithms. The local simulators like **qasm_simulator** and **statevector_simulator** are used for testing. To run the code on actual quantum hardware, you need to set up an IBMQ account.

## Results and Conclusion

This project compares the performance of classical optimization techniques with quantum approaches. Both the **Hierarchical Risk Parity (HRP)** model and **Efficient Frontier** were analyzed, while the **QAOA** and **SamplingVQE** algorithms were employed to optimize the same portfolio using quantum computing. The results demonstrate the potential of quantum algorithms for portfolio optimization, although further advancements are needed for practical application.

## Acknowledgements

We extend our gratitude to the developers of **Qiskit**, **Pandas**, **Numpy**, and **Matplotlib**, whose tools have been instrumental in this research. Special thanks to the **Qiskit Community** for making quantum computing accessible.





