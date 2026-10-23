When NOTing an stuff in brackets, keep the NOT on the 'variables' and switch the signs.

E.g. $(\overline{\text{X+Y}})=\overline{\text{X}}.\overline{\text{Y}}$ (De Morgan's first law)
and $(\overline{\text{X.Y}})=\overline{\text{X}}+\overline{\text{Y}}$ (De Morgan's second law, by duality)

These are called *De Morgan's Laws*.

This extends to more than two variables. You can prove this with a truth table, or algebraically:
- Prove $\overline{(A+B+C)}=\overline{\text{A}}.\overline{\text{B}}.\overline{\text{C}}$
- Let $A+B=D$
- So now we are proving $\overline{\text{(D+C)}}=\overline{\text{D}}.\overline{\text{C}}$
- Since $D=A+B$, $\overline{D}=\overline{A+B}$
- Use De Morgan's first law to get $\overline{D}=\overline{A}.\overline{B}$
- Substitute back into the RHS of equation in bullet point 3 to get $\overline{(A+B+C)}=\overline{\text{A}}.\overline{\text{B}}.\overline{\text{C}}$

De Morgan's laws are useful when you have a lot of inversions.


In a **combinational** logic circuit, inputs are turned into outputs. There are no loops or anything. A combinational logic circuit with $n$ input variables has $2^n$ possible input combinations.
![[Pasted image 20261019171940.png]]
Here is an example of what cannot happen in a combinational circuit. There are no cyclic paths/feedback.

Here is how to derive a 'sum-of-products' expression for a boolean equation from a truth table:
1. Go down the truth table until you find a row with output '1'. (ignore all columns with output 0)
2. If the input variable is 1, leave it as is. If the input value is 0, complement it (i.e. NOT it)
3. AND the input variables together (not 0.1=1, I mean just write $X.Y$ on the paper)
4. Do this for each column with output 1, then OR each little expression together.

For example:
![[Pasted image 20261019174418.png]]
Here is how you would derive an expression:
- First find the columns with output f=1. This is column 2 and 4. I will only go through column 2
- A is 0, so write it as $\overline{A}$. B is 1, so keep it as $B$
- AND these two to get $\overline{A}.B$
- Do the same process on column 4 to get $A.B$
- OR these together to get $(\overline{A}.B)+(A.B)$

So the sum of products expression for this truth table is $(\overline{A}.B)+(A.B)$.

This method works with more than two variables.

You can also derive a product-of-sums equation by doing the opposite (i.e. look for columns with output 0)

Using the above table again as an example:
- First find the columns with output 0, this is column 1 and 3
- Derive the equation using the above method to get $\overline{f}=(\overline{a}.\overline{b})+(a.\overline{b})$
- Invert to get $f=\overline{(\overline{a}.\overline{b})+(a.\overline{b})}$
- Apply De Morgan's first law to get $f=\overline{(\overline{a}.\overline{b})}.\overline{(a.\overline{b})}$
- Apply De Morgan's second law to the individual terms:
	- First term: $\overline{\overline{a}.\overline{b}}=\overline{\overline{a}}+\overline{\overline{b}}=a+b$
	- Second term: $\overline{a.\overline{b}}=\overline{a}+\overline{\overline{b}}=\overline{a}+b$
- So we end up with $f=(a+b).(\overline{a}+b)$

(product = AND (.), sum = OR (+))



It should be noted that a logic gate is an abstraction; in reality this is made up of many transistors and whatchumacallits but at this stage we can just treat them as a whole logic gate.




![[Pasted image 20261019184925.png]]
This is a *logic buffer*. It just returns the input (it is the opposite of a NOT gate, sometimes called a YES gate). Mathematically this doesn't do anything, but in reality it can be used to amplify a weak signal (from what I understand an electric signal is just a general term encompassing both current and voltage).


In reality, an inverter (NOT gate) and NOR gate are created by wiring the input wires together.

Universal gates and NAND and NOR. They are called universal gates since you can use them alone (only NAND or only NOR) to create any other type of basic logic gate.

For instance:
- You can make an OR gate from NOR by first passing the inputs through the NOR gate, then wiring the inputs together (so input A = input B) and passing it through another NOR gate which acts as an inverter, giving you the OR gate as shown in the diagram below

![[Pasted image 20261019190931.png]]

You can also make an OR gate with NANDs, but first must do some maths to introduce the AND operator (.):
- $f=a+b$ (this is what we are aiming for)
- Nothing can be done with this, so invert RHS twice to get $f=\overline{\overline{a+b}}$
- Apply De Morgan's first law to the inner $\overline{a+b}$ to get $f=\overline{\overline{a}.\overline{b}}$
- Therefore we must invert both inputs, then NAND them (in other words, let $X=\overline{a}$ and $Y=\overline{b}$. the NAND gives us $\overline{X.Y}$ which is the same as $\overline{\overline{a}.\overline{b}}$)
- Inverting an input means we need to wire the inputs together again, then pass both $\overline{a}$ and $\overline{b}$ through the NAND, shown in the diagram below
![[Pasted image 20261019191338.png]]

Wiring together inputs with universal gates makes them act as an inverter, as shown by these truth tables:
![[Pasted image 20261019191940.png]]

