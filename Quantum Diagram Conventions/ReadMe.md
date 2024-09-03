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
 - H: Hadamard gate creates equal superposition and transforms base sates. ![enter image description here](https://www.mathworks.com/help/matlab/math/gatesymbol_hgate.png)
 - S (Phase gate): adds a phase of ($\pi$/2) to |1 $\rangle$
 ![enter image description here](https://upload.wikimedia.org/wikipedia/commons/thumb/1/11/Qcircuit_S.svg/225px-Qcircuit_S.svg.png)
 
 - T (Phase gate): adds a phase of ($\pi$/4) to |1 $\rangle$
 ![enter image description here](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c1/Qcircuit_T.svg/225px-Qcircuit_T.svg.png)
 
 - Z (Pauli-Z gate): flips the phase of qubit 1 to -1 but leaves |0 $\rangle$ as is.
 ![enter image description here](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f7/Qcircuit_Z.svg/162px-Qcircuit_Z.svg.png)
 - X (Pauli-X NOT gate): flips state of qubit
 ![enter image description here](https://upload.wikimedia.org/wikipedia/commons/thumb/4/43/Qcircuit_X.svg/225px-Qcircuit_X.svg.png)
 
 - Y (Pauli-Y gate): flips the state and phase
![enter image description here](https://upload.wikimedia.org/wikipedia/commons/thumb/9/92/Qcircuit_CY.svg/189px-Qcircuit_CY.svg.png)

 - CNOT (Controlled-NOT Gate):  two-qubit gate that flips the second qubit(target) if its state is |0 
$\rangle$. (performs a Pauli-X on target but remains unchanged if control/first cubit is in 0 state.)
 ![CNOT gate](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR-4xCoqItaoyu0fq5tdhF73yx-ssLU1ji75w&s)

- 
