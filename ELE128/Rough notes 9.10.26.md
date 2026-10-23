
The connection between two OR MORE components is called a **node**. (ie a corner point). E.g. node 2 is the connection between the voltage source and R1. 
*A node is not always a corner, e.g. there can be a node between two components in series.*
![[Pasted image 20261009110550.png]]

There may be fewer nodes than you think in a circuit since different nodes that are electrically equivalent are actually just one node.
![[Pasted image 20261011134755.png]]
For instance, A, B, C and D seem like 4 different nodes but they are electrically equivalent (they are on the same wire with no components between them) so it is just one node.

Two corners can both be one node if there are no more components between the two corners.
![[Pasted image 20261009110646.png]]
E.g. the bottom left corner is still Node 3 since there are no more components between the bottom right and bottom left.
This means you can represent the voltage across a component as the voltage between two nodes.
e.g. $V_{R1}=V_{12}$. (it is $V_{12}$ and not $V_{21}$ since the more positive node comes first.)

A **branch** is a component or group of components connected between two nodes. E.g. R1. Typically any component with a positive and negative terminal (afaik this is all components) is a branch, but multiple components in series can also be a branch.
![[Pasted image 20261011135011.png]]
In this case each resistor is a branch, but all four resistors put together is also a branch, since they all share a positive and negative terminal to the rest of the circuit.


A **loop** is a path fully round the circuit without going through a component more than once.
- You can trace the loop from positive to negative OR negative to positive (it doesn't matter, your answer may be negative though)
- The loop DOES NOT need to go through the battery

Example of nodes, branches and loops:
![[Pasted image 20261009111256.png]]

![[Pasted image 20261009111428.png]]


**Kirchhoff's current law (KCL)** states that the sum of all current entering a node is zero (i.e. the current going in = the current coming out). You may not need to derive a KCL expression for each node.

![[Pasted image 20261009111810.png]]
So $I_1+I_2+I_3+I_4=0$.

![[Pasted image 20261009111909.png]]
Current going in = current coming out. So $I_1+I_2=I_3+I_4$.

Split a current into $I=I_1+I_2$ in parallel.


**Kirchhoff's voltage law (KVL)** states that the sum of voltage around a closed loop is zero (i.e. voltage rise = voltage drop). You may need to negate some terms to reflect the direction of current.



Use KCL, KVL and Ohm's law together to find currents, resistances and voltages.

---
A ground point/reference node is a node that is defined as having 0V. This is useful in nodal analysis since we already know the voltage at that point (it is a good idea to pick a reference node connected to the negative terminal of the voltage source)

Sourcing=supplying energy to circuit
Sinking=using energy

The aim of nodal analysis is to figure out the voltages at each node (using KCL).

![[Pasted image 20261009131642.png]]

Step 5: use ohms law (remember to put the more positive voltage first to give a non-negative answer) with reference to voltages AT CERTAIN NODES


![[Pasted image 20261017154017.png]]
This circuit has a short circuit between nodes A and B. This is because current must flow through R1, but  then will choose to go through AB through the path of least resistance, so no current flows to R2 (I2=0). As a result in your analysis you can ignore the right hand side loop since no current flows through it.

An open circuit is a circuit that is not fully connected (i.e. there may be a wire missing). In this case the resistance between two unconnected nodes is $\infty\text{A}$ and the current between them is 0.
































 

