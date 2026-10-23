
The pn junction is basically just a diode.

Recap:
- n-type semiconductors have mobile negative charges
- p-type have mobile positive charges
- Joining n-type and p-type (not physically possible) causes an annihilation event where electrons and holes combine, creating a depletion region
- This creates an electric field, causing electrons to drift towards the positively charged side

**Reverse biasing the junction** is making the electric field stronger. 

**Forward biasing** the junction counteracts the electric field in the diode, creating a large "diffusion current" (as the obstacle preventing them from diffusing across the junction has reduced).

Think of it like a dam; making a dam higher doesn't have an effect, but reducing its height causes water to rush out (like the diffusion current).

So there are two currents:
- Diffusion current, which is electrons and holes moving from - to + and + to -
- Drift current, which is energy carriers getting caught up in the electric field.*

Diode behaviour is described by the Shockley Diode Equation:
$$I=I_0[\exp{(\frac{eV}{kT})-1}]$$

($\exp{(x)}$ means $e^x$. $e$ meaning Euler's constant, not elementary charge)
It says:
- The current flowing through the diode is dependent on $I_0$ (saturation current)
- $eV$ is the amount of energy by which the barrier has been reduced in the pn junction
- $kT$ shows how much energy is available to electrons from ambient temperature ($T$ is in kelvin)
- $-1$ shows the drift current (a constant reverse bias)

The $e$ (elementary charge) is sometimes written as $q$.

A diode at reverse bias causes the power of $\exp$ to be negative, so this is a large negative number. The equation evaluates to roughly $-I_0$

Remember $P=IV$


In the light, electron hole pairs can be made in the depletion region, but because of the electric field, these move in the same way as the drift current. This creates an extra current called the **photocurrent**.

Thus the Shockley diode equation becomes $$I=I_0[\exp{(\frac{eV}{kT})}-1]-I_L$$ where $I_L$ is the photocurrent.

Since photocurrent is a constant subtractor, at reverse bias $I$ becomes negative, so power is negative (since $P=IV$) so we are extracting power from the diode (this is how a solar panel works).























 