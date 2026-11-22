# Modeling Crosstalk in Two-Qubit Quantum Systems

A nonlinear differential equation model of crosstalk between two qubits, calibrated with experiments on IBM's ibm_fez quantum processor.

## Overview
On multi-qubit processors, one qubit's state can affect another's error rate, which is called crosstalk. This project models two-qubit decay with a coupled nonlinear system that adds a crosstalk term to the standard linear decay model:

dP_A/dt = -γ_out · P_A + σ · P_A · P_B
dP_B/dt = -γ_out · P_B + σ · P_A · P_B

## Key Results
- Calibrated the model using 4,096-shot experiments run through IBM Qiskit
- Estimated the crosstalk coefficient: −28222.36 s⁻¹ ≤ σ ≤ −28088.10 s⁻¹
- Found that crosstalk causes qubits to decay roughly 2x faster than an ideal linear model predicts
- Visualized the results with Euler's method simulations, phase portraits, and Bloch spheres

## Files
- `paper.pdf`: full write-up, including the code in the appendix

## Tools
Python, NumPy, Matplotlib, Qiskit, Excel

## Authors
Samuel Cohen, Nithin Palacherla, Gavin Prussia