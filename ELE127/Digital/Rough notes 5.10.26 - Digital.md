
Truth tables are used to show how different logic gates work:

![[Pasted image 20261005174151.png]]

Here are some more complex logic gates:
![[Pasted image 20261005174244.png]]

- **NAND** is the opposite of AND
- **NOR** is the opposite of OR
- **XOR** (exclusive OR) is OR but 1+1 produces 0
- **XNOR** is the opposite of XOR

(the little dot on each diagram shows the output is inverted. It is called an *inversion bubble* and is a shorthand way of drawing an inverter/NOT gate)

You should probably memorise these truth tables.

![[Pasted image 20261005175024.png]]

You can connect the output of a logic gate to the input of another logic gate ($G0$, $G1$, $G2$, $G3$, and $G4$ are logic gates) and logic gates like $G3$ can take more than 2 inputs but you **CANNOT** connect two outputs together as this could create a short circuit.

(The black dots on the picture show that the wires are connected, not just crossing)

Just like in maths, logic gates have an order of priority (like BODMAS):
- The highest priority is inversion (e.g. NOT)
- The 2nd highest priority is addition (e.g. AND)
- The lowest priority is OR

A truth table for any logic gate function has $2^{n}$ rows, where n is the number of variables.
![[Pasted image 20261005180024.png]]





Literal analysis is when you follow along the circuit diagram to figure out the solution to one of these equations: (a literal is a 0 or 1)
![[Pasted image 20261005180836.png]]

This is only useful for small circuits.

Symbolic analysis is similar to literal analysis but instead of tracking ones and zeroes, you're tracking algebra to make an expression at the end for the entire circuit:
![[Pasted image 20261005181150.png]]

You can also view logic gates with switches: AND is switches in series, OR is switches in parallel
![[Pasted image 20261005181608.png]]