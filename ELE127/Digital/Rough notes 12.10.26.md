Here are some axioms that are always true when doing Boolean algebra
1. **Closure** - i.e. boolean operations only ever produce 1 or 0
2. **Identity**
	- X + 0 = X
	- X.1 = X
3. **Commutative**
	X+Y = Y+X, X.Y = Y.X
4. **Distributive**
	X.(Y+Z) = X.Y + Y.Z
	X+(Y.Z) = (X+Y).(Y+Z)
5. **Complement** properties
	X+$\overline{\text{X}}$=1
	X.$\overline{\text{X}}$=0

There is also the **duality principle**. (which is how many of these expression are derived). This is where changing '+'s to '.'s and '0's to '1's (or vice versa) in a valid boolean IDENTITY/theorem yields another valid expression. The resulting expression is known as its **dual**.
For instance:
- X + 0 = X is an identity
- Then, swapping +s and 0s, we get X.1=X which is also true.

It does not work in this case:
	X.Y=1
	X+Y=0
Because X.Y=1 is not always true.


Here are 4 fundamental theorems of boolean algebra (these can be assumed to be true because of the axioms land out above)
1. Null law
	X+1 = 1
	X.0 = 0
2. Involution
	$\overline{\overline{\text{X}}}$=X
3. Idempotency
	X + X = X
	X.X = X
4. Absorption
	X + (X.Y) = X
	X.(X + Y) = X
5. Simplification
	X + $\overline{\text{X}}$.Y = X + Y
	X.($\overline{\text{X}}$+Y) = X.Y
6. Associativity
	X + (Y + Z) = (X + Y) + Z
	X.(Y.Z) = (X.Y).Z
7. Consensus
	X.Y + $\overline{\text{X}}$.Z + Y.Z = X.Y + $\overline{\text{X}}$.Z
	(X + Y).($\overline{\text{X}}$ + Z).(Y + Z) = (X + Y).($\overline{\text{X}}$ + Z)

These can all be proven with truth tables.
*consensus can be remembered as if you have 3 people, 2 say yes, one says no, then the consensus is yes*
Probably don't ned to learn 7 or 4

