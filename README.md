# Gaussian-and-DRAG-pulse-optimization

This code simulates a quantum system, specifically a transmon qubit under the influence of Gaussian and DRAG pulses, using QuTiP, a Python library for quantum simulations. The setup defines a basic transmon Hamiltonian with a linear term and a nonlinear term corresponding to the qubit's anharmonicity. It also includes control Hamiltonians for bit-flip (σx) and phase-flip (σy) operations, manipulated by Gaussian and DRAG pulses. The Gaussian pulse is computed based on its center time, duration, and standard deviation, with parameters defined by specific formulas for normalization. The DRAG pulse is derived by applying a time derivative to the Gaussian pulse, and its amplitude is controlled by a parameter λ, adjusting the pulse to mitigate leakage errors. These pulses are then used to drive the qubit system. The time evolution of the system is solved using QuTiP's `mesolve` function, and the results are stored for further analysis.

This approach draws on established quantum control theory, particularly techniques for correcting errors in superconducting qubits, as described in references such as

1. https://arxiv.org/pdf/0901.0534 for Gaussian pulses
2. 
3. https://arxiv.org/pdf/1005.1279 for DRAG pulses
4. 
5. https://arxiv.org/pdf/1904.06560 on the transmon qubit Hamiltonian.
