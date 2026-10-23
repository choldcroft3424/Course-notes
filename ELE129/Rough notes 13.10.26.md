The limit switch switches one way when the window is fully open, and the other way when the window is fully closed, indicating the motor should stop opening/closing.

In Arduino, arrays start at 0. In Matlab, they start from 1.

Make sure to initialise an array asap or it will just contain garbage memory.

Consider using arrays of pins, e.g. to set pinMode on many actuators at once using a for loop. It also makes the system more scalable. You could also store the statuses of actuators in arrays (e.g. an array for what each actuator should do when the temperature is too high, one when it's too low, etc).




























