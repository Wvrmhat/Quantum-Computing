# Quantum Computing 
Makes use of qubits, can be in any state at once when unobserved known as superposition. However when it is observed/measured then it has to decide on a state.

**Entanglement**: a connection where qubit's react to a changed in another qubit instantly. Therefore when measuring one entangled qubit, you can determine the properties of it's partners.

**Qubit manipulation**: 
Quantum gates are applied to qubits to entangle them and manipulate probabilities. The outcome collapses the superposition to a sequence of 0s and 1s. Allowing all calculations to be done at the same time. It does not "try all the options", it decides the most likely answer.
> Normal logic gates take a set of inputs and has one definite output
> Exploiting superposition and entanglement would be more efficient than whatever would be possible on normal computer

<details>
	<summary>Uses for quantum computing</summary>
	
 - Database searching
 - Decryption of private/RSA keys
 - Simulations
 - Developing new materials with longer chains molecules

</details>

--- 
## Primitives

**Estimator primitive**: Computes expectation values (evs) of observables with the respective states from quantum circuits (qc).

**Expectation value (evs)**: represents average outcome of a quantum observable. Practically they are used to help predict the average result of measurements.

**Sampler Primitive**: Returns shot by shot bit strings  sampled from the probability distribution of the quantum state prepared on the device. 
```
sampler.run([
  (circuit1, param_values1, shots1),
  (circuit2, param_values2, shots2),
])
```
It can be used to compute expectation values but then you would need to implement post-processing yourself. While the **estimator** handles this automatically.
