
**Active components** are components that supply energy in the form of voltage or current.

Voltage sources include batteries, power supplies
Current sources include photodiodes, transistors

**Passive components** store or dissipate electrical energy. 
These include:
- **Resistors** which dissipate energy into heat
- **Capacitors** which store energy in an electric field
- **Inductors** which store energy in a magnetic field



A direct current (DC) is a current **or voltage** that does not change with time (it is not a function of time). An alternating current or voltage (AC) is one that does change as a function of time.

![[Pasted image 20261002123440.png]]

![[Pasted image 20261002123606.png]]

![[Pasted image 20261002123619.png]]

A negative charge is brought about by the presence of electrons. A positive charge is brought about by the presence of a hole (lack of electron) or proton. The unit for charge is the **coulomb (C)** (1 electron = $1.6\times10^{-19}\text{C}$).

A difference in charges creates a **potential difference** (voltage) measured in volts (V).

![[Pasted image 20261002124121.png]]

Current is the **rate of flow of charge.** In the above example, letting go of the positive charge will cause it to be attracted to the negative charge. The speed at which it moves is the current.
$I=\frac{Q}{t}$. Current is technically measured in coulombs per second ($Cs^{-1}$) but this gets messy so it is measured in Amps (A).

Due to historical reasons we use conventional current flow where current flows from positive to negative.

![[Pasted image 20261002124618.png]]

The unit for energy is joules (J). Energy is required to separate charges, creating a potential difference. Therefore **energy = voltage x charge**. Or $Energy=VQ$. Rearranging $I=\frac{Q}{t}$ gives $Q=It$, subbing this in gives $Energy=VIt$.

Power is the rate of energy supplied/used.





----


![[Pasted image 20261002130421.png]]


A voltage source (e.g. a battery) has a magnitude (given by $V_S$) and a direction/polarity given by the arrow (long leg=+, short leg = -). The arrow points towards the more positive terminal.

In a component like a resistor, the arrow points towards the positive terminal. This means the arrow points in the opposite direction to current; this is useful since it shows the component uses up voltage.

A voltage source can both supply and receive energy.
**Voltage is independent of current.**

Since energy = $VIt$, there is a current associated with a voltage source given by $I$.


Voltage is constant but current can change
![[Pasted image 20261002131151.png]]

Current source diagram:

![[Pasted image 20261002131025.png]]


Similarly a current source has a voltage $V$ associated with it.


![[Pasted image 20261002131224.png]]




### Calculations

A battery rated at 120Ah has a potential difference of 12v.


Find the total energy stored when fully charged:
- Energy = $VIt$
- 120Ah = 120 x (60 x 60) = 433,000 As (=$It$)
- 12 volts battery
- Energy = $VIt$ = 12 x 433,000 = 5.18 x $10^{6}$ J = 5.18 MJ


Find current drawn by a 10W component connected:
- Power = $VI$
- $I=\frac{P}{V}$=$\frac{10}{12}$=0.83A


How long could the battery sustain the component:
- Energy = $VIt$
- $t=\frac{\text{Energy}}{VI}$
- $t=\frac{5.18\times10^{6}}{12\times0.83}$
- $t=5.20\times10^{5}$ seconds



Materials have three properties which determine their resistance:
- Resistivity ($\rho$)
- Area (A)
- Length (L)

So resistance = $\frac{\rho L}{A}$ (divide by A since larger area = lower resistance). Units are ohms ($\ohm$)

![[Pasted image 20261002132732.png]]

![[Pasted image 20261002132834.png]]




Ohm's law states that $V=IR$.

![[Pasted image 20261002133213.png]]




Ohm's law can be rearranged and combined with other equations. E.g. energy = $VIt$, $V=IR$, so energy = $IRIt$=$I^{2}Rt$.
This can be useful if you don't have some information.


More calculations:
- 9V battery, 3$\ohm$ resistor, find current
	- Ohm's law $I=\frac{V}{R}$
	- $I=\frac{9V}{3\ohm}$
	- $I=3\text{A}$

Some diagrams show current going negative to positive, in this case you can use conventional current but flip the polarity by adding minus sign:

![[Pasted image 20261002134253.png]]


Resistors in series can be simplified by adding resistances and voltages, here's the proof:
![[Pasted image 20261002134600.png]]


Similar proof for resistors in parallel:
![[Pasted image 20261002134945.png]]

or remember $R_T = \frac{1}{R_1}+\frac{1}{R_2}+\frac{1}{R_3}+...$


