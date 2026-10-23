Kirchhoff's voltage law states that the **sum of voltages around a loop add to zero.** (i.e. place a multimeter at either end of each component in the loop, add up the voltages, this number should be zero) Kirchhoff's current law states that the **sum of currents into a node must be zero**. This will be covered in the future more (probably in a different module. Maybe ELE128)

## Kirchhoff's rules (NOT PART OF LECTURE)
Kirchhoff's laws were initially derived from Faraday's law:
`A changing magnetic field through any area results in a voltage (potential difference) across that area`.
The reverse is also true (a voltage results in a changing magnetic field)

Most circuits (with the exception of fancy radio stuff) have a voltage and thus have a magnetic field, however this field is pretty static. That means, in this case, there is no changing magnetic field, thus there is no voltage.

This sounds wrong, but it actually makes sense, since some components can create a voltage gain (like a battery) while others create a voltage drop (like resistors or diodes). This means the sum of all the voltages adds to zero, so Faraday's law still applies.

Keep in mind using Kirchhoff's laws that they depend on the direction of the current (since Faraday's law depends on the 'direction' of the area). If the current goes through a component in the opposite direction to how you defined your loop (clockwise or anti-clockwise) then negate that number.

## Continuing...

Add up resistances in series. To prove this is true, note that $V_S=V_1+V_2+V_3+...$ (Kirchhoff's voltage law) where $V_1$, $V_2$, $V_3$ are voltage drops across resistors. Then remember $V=IR$ so $V_S=IR_1+IR_2+IR_3+...$ where $I$ is the current in the series loop. Thus $V_S=I(R_1+R_2+R_3+...)$.

The greater the resistance, the lower the current flow for the same voltage source.




---


Resistors in series have greater resistance than resistors in parallel (e.g. it is harder to suck from 2 straws in series than 2 straws in parallel)

















