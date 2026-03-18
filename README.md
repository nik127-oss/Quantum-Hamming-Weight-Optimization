# Ancilla-Free Quantum Hamming Weight Optimization

## Overview
This project presents an optimized ancilla-free quantum circuit for Hamming weight computation, designed for resource-constrained quantum systems in the NISQ era. The work focuses on reducing non-Clifford gate complexity while maintaining circuit accuracy and low depth.

## Key Contributions
- Designed an ancilla-free quantum circuit for Hamming weight computation
- Reduced T-gate complexity by up to 69% using approximation techniques
- Applied controlled phase rotation truncation and approximate QFT
- Analyzed trade-offs between accuracy and computational efficiency
- Implemented and validated the circuit using Qiskit

## Technical Details
The approach encodes the Hamming weight into quantum phase using controlled rotations and reconstructs the output using an inverse Quantum Fourier Transform (QFT). Optimization is achieved by:
- Removing small-angle phase rotations below a threshold
- Using approximate inverse QFT to reduce gate count
- Evaluating the circuit in terms of T-gate cost and scalability

## Tools and Technologies
- Qiskit
- Python
- Statevector simulation

## Results
- Up to 69% reduction in T-gate count for larger input sizes
- Sublinear growth in optimized circuit complexity compared to exact implementation
- Demonstrated trade-off between phase accuracy and gate efficiency
