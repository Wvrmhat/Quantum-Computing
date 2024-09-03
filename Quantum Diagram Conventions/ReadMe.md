# Quantum diagram conventions
Quantum circuits are read from left to right since time also flows from left to right. The left-most gate is applied first 

<details>
	<summary>Reading circuit diagrams</summary>
	
	

 1. **Qubit register**: horizontal line representing qubit, labeled from top to bottom starting at 0.
 
 2. **Quantum gate**:  Similar to logic gates, represented by boxes. For example H is the Hadamard gate.
 
 3. **Controlled gate**:  Acts on multiple qubits. Example the CNOT gate with a black circle for the control, and cross within circle is the target qubit.
 
 4. **Measurement operation**:  Meter symbol, measures qubit and outputs information.

![quantum circuit diagram](https://learn.microsoft.com/en-us/azure/quantum/media/annotated-sample-circuit.png)
	
</details>

> Number of  wires entering a gate represent both the input and output. Therefore if quantum gate had more outputs than inputs, it would not be unitary/reversible.
---
## Multi-qubit operations
Follow same conventions to single-qubit ones. For example a two-qubit (meaning two inputs), unitary operation ***B*** can be defined as (HS ⊗ X). 
![multi-qubit operation](https://learn.microsoft.com/en-us/azure/quantum/media/4.svg)
 The reason it is read as (HS ⊗ X) or that it's read reversed. Is because "Matrix operation" ⊗
 

 - ⊗ **Tensor product**: combines two quantum states into a larger one. Here we combine HS and X.
 - H: Hadamard gate creates superposition.
 - S (Phase gate): adds a phase of (\pi/2)

