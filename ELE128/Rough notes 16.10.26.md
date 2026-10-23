Loop analysis is an altered version of nodal analysis which uses imaginary *loop currents* such as $I_A$ and $I_B$. This simplifies calculations in circuits with many loops.

Here are the steps for loop analysis:
1. Identify loops within the circuit
2. Define the loop current for each loop
3. Draw voltage arrows for all components in the circuit (points towards positive terminal)
4. Derive equations for branch currents using KCL and loop currents
5. Apply KVL on each loop to create an equation for each loop
6. Solve for the unknown in these equations



---

So far we have been treating voltage and current sources as if they have no internal resistance. In reality, they do. (If you want this can be represented by adding another resistor $r_{int}$ in series after an active component)


An ideal voltage source will have zero internal resistance:
![[Pasted image 20261023145557.png]]
This circuit shows a voltage source and simulates its internal resistance with resistor $r_{int}$. There is a voltage drop across $r_{int}$ so the voltage received by the resistor $R$ would be less than $V_S$. Ideally $r_{int}$ would have resistance $0\ohm$ to prevent this.
Zero ohms can also be represented as a **short circuit**. In superposition analysis we can replace voltage sources with 0V voltage sources, which have no resistance ($R=\frac{V}{I}$), so can be considered as a short circuit.

Current sources will also have an internal resistance in reality. 
In superposition analysis we replace current sources with 0A current sources. This creates a section of circuit with no current flowing, in other words, an **open circuit**. Thus an ideal current source creates an open circuit, so have an internal resistance of $\infty\ohm$.

In other words:
- Recall that a voltage source *maintains a constant voltage* no matter the current
- In superposition analysis, voltage sources are set to 0V.
- This creates a section of circuit where, no matter the current, there is no voltage drop
- In other words, this is a short circuit
Similarly:
- Recall that a current source *maintains a constant current* no matter the voltage across it.
- In superposition analysis, current sources are set to 0A.
- This creates a section of circuit where, no matter the voltage, no current flows through
- In other words, this is an open circuit.

In superposition analysis, we consider one voltage source/current source at a time, and finding the voltage/current contribution to the target component, then adding each contribution.

Step by step procedure for superposition analysis:
1. Identify active components
2. For each source:
	1. Replace other active components with short circuits (voltage sources) and open circuits (current sources)
	2. Work out the voltage/current across the component in this simplified circuit
3. Add up all the voltages/currents obtained 

Keep in mind that voltage across parallel resistors is the same.