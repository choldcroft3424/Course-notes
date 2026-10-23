A hazard is anything that can cause harm. A risk is the likelihood of this hazard causing harm.

These can be quantified into a risk table:
![[Pasted image 20260930211428.png]]

To assess a risk, you must:
- Identify hazards (identify what could cause harm by looking around, looking at instructions, data sheets etc)
	- Identify long term hazards such as radiation AND identify hazards to third parties such as people walking by
	- 
You can decide on precautions in this order (start from the top and work down until you can implement one of these):
- Eliminate the hazard
- Replace it with something safer
- Prevent access to the hazard
- Reduce people's exposure to the hazard
- Wear PPE (protective clothing to reduce the risk)
- Provide welfare facilities such as first aid boxes

![[Pasted image 20260930212214.png]]

Common hazards include:
- Trip and slip hazards
- Exposure to toxic chemicals
- Musculoskeletal disorders such as tendonitis from carrying heavy loads
- Losing your balance at height (e.g. on a ladder)
- Things catching on fire
- Electrocution



---



Requirements of greenhouse system:
- Keep greenhouse in range 3-25C
- When too cold, heater turns on
- When too warm, windows + fan open

 
 Sensors detect environmental changes, actuators are the "muscles" that convert electrical signals to physical actions.


An analogue temperature sensor in this case outputs a voltage in the range 20-358mV which maps to 0-30 C.


Actuators in this system are:
- 3 LEDs (green, blue, red)
	- Red indicates max temperature is reached
	- Blue indicates min temperature is reached
	- Green indicates within temperature threshold
- Digital fan, heater (on/off)
- Digital (on/off) actuators to open/close windows


![[Pasted image 20261001152143.png]]




The system corrects itself if temperature < 8 or > 20, this is called hysteresis. (e.g. prevents heater from constantly flicking on and off at 3 C)

---

Components for robot project:

LEDs are polarised so must be inserted the right way around (short end is cathode -, long leg is anode +)


### DC geared motors:
- Speed is controlled by varying voltage
- Direction is controlled by H bridge (different combinations of switches in the diagram below create different directions)
![[Pasted image 20261001153208.png]]

Data sheet showing how to connect H bridge to motors:

![[Pasted image 20261001153349.png]]

Speed of motors is controlled by pulse width modulation (PWM), meaning "pulses" of electrical connection occur at different speeds, more pulses means faster wheels. This allows for speed to be controlled
![[Pasted image 20261001153643.png]]

These must be connected to pins with a tilda ~

A phototransistor is used, connecting the wheels to the circuit when light from the emergency beacon is detected.

Ultrasonic obstacle sensors are used to detect objects by emitting soundwaves and detecting if they bounce back. The time taken to bounce back corresponds to distance.



