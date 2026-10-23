
### Recap of a level maths
#### Functions

When one quantity depends on another, this can be modelled by a function:

- A function is a rule takes in an input and produces an output
- A function describes a **relationship** between an input and output

In $y=f(x)$:
- $x$ is the independent variable
- $y$ is the dependant variable
- The thing inside the brackets is the argument

A function has:
- A domain (allowed inputs)
- A range (allowed outputs)

that in engineering must reflect reality (eg time cannot be negative)


e.g. if $f(x)=x^{2}$:
- Domain is $f(x) \in \mathbb{R}$
- Range is $[0, \infty)$
Most of the time, undefined values can be neglected.

Evaluate a function by replacing the independent variable with a number, e.g. $f(x)=x^{2} \text{, } f(2)=(2)^{2}=4$.


You can also evaluate by substituting an expression into a function. e.g. $f(x)=x^{2} \text{,  } f(x^{3})=(x^{3})^{2}=x^{6}$.
Make sure to use brackets especially in more complex functions.

You can compose functions in a similar way. Note that $f(g(x)) \ne g(f(x))$.

See lecture capture 1/10/26 roughly 33mins for table of graph transformations.

Checkpoint
e.g. if $f(x)=3x^{2}-4x+1$, $f(x+1)=3(x+1)^{2}-4(x+1)+1=3(x^{2}+2x+1)-4x-4+1=3x^{2}+2x.$ 

Functions give the mathematical structure, variables tell us the physical meaning. (e.g lots of situations can be modelled with functions in the shape of $y=e^{-x}$)

Functions must be uniquely defined, e.g. $x=y^{2}$ is not a function as it could be represented as either $y=\sqrt{x}$ or $y=-\sqrt{x}$.

#### Polynomials

Any function can be converted (approximately) to a power series using a Taylor expansion (similar to Maclaurin series)

An $n$th degree polynomial is a polynomial with $n$ roots (including complex and repeat roots). It has a highest power of $x^{n}$. Polynomials of degree 4 or higher don't have a formula to solve them, solve these by iteration or factorising (use the factor theorem).

You can use the factor theorem in reverse to construct a polynomial. Or use the relationships between roots ($\alpha+\beta+\gamma=1$, etc)

If a polynomial is an ev=en degree (highest power is 2, 4, 6, etc) it rises at both ends (or falls if the leading coefficient is negative). If it is an odd degree, it will fall on the left and rise on the right (or vice versa with negative leading coefficient).

- Negative real roots indicate a decaying response
- Positive real roots indicate a growing response
- Complex roots indicate an oscillation

Checkpoint
Roots -3, 2, 4.
$f(x)=(x+3)(x-2)(x-4).$

Expanded:
$f(x)=(x+3)(x^{2}-6x+8)=x^{3}-6x^{2}+8x+3x^{2}-18x+24=x^{3}-3x^{2}-10x+24$



When constructing a polynomial from its roots, there are an infinite number of solutions as we do not know the vertical scale. E.g. roots 1 and 2 could give any polynomial in the form $f(x)=A(x-1)(x-2), A\in\mathbb{R}$.

A root with even multiplicity (e.g. $(x-1)^{2}(x+1)$ causes the graph to 'bounce' and not cross the x axis. A root with odd multiplicity (e.g. $(x-1)^{3}(x+1)$) causes a crossing/point of inflection.

----


Multiplying both sides of an inequality by a negative reverses the sign:
- $2<5$
- $-2>-5$

When solving polynomial inequalities, solve like normal then test ranges less than, in between, and greater than the roots. (don't bother factorising, just use the quadratic formula)


e.g. if roots are 2 and 3, test $x<2$, $2<x<3$, $x>3$.


e.g. solve $\frac{x-2}{x-5}>0$.
- Critical values x=2, x=5
- Intervals are $x<2$, $2<x<5$, $x>5$.
- Test each interval (outside roots is positive, inside roots is negative)
- Solution is $x<2$, $x>5$
	- $x<2$ as the inequality is strict ($>$, not $\ge$)
	- $x>5$, not $x\ge5$ as the value of x at 5 is undefined


If $|A|<c$, then $-c<|A|<c$. This can be used to solve:
- $|2x-1|<5$
- $-5<2x-1<5$
- Add one to all sides: $-4<2x<6$
- Divide by 2: $-2<x<3$
You could also separate the absolute value into positive and negative like at A-level.

If $|A|>c$, then $A<-c$ and $A>c$.

e.g. $\frac{x-6}{x-5}\le\frac{2}{x-3}$:
-  $\frac{x-6}{x-5}-\frac{2}{x-3} \le 0$
- Combine into one fraction, get a common denominator, factorise
- Eventually you get $\frac{(x-4)(x-7)}{(x-5)(x-3)} \le 0$
- Test intervals with critical values x=3,x=4,x=5,x=7 (make sure to use strict inequalities with 3 and 5 as these are undefined):

| Ranges | $x<3$ | $3<x\le 4$ | $4\le x<5$ | $5<x\le 7$ | $x\ge7$ |
| ------ | ----- | ---------- | ---------- | ---------- | ------- |
| + or - | +     | -          | +          | -          | +       |

- The function is $\le0$ for all $3<x\le4$ and $5<x\le7$. Therefore this can be written as $x\in(3, 4] \ \cup (5, 7]$.

