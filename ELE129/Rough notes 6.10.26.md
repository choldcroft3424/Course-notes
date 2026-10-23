
When coding Arduino:
- `void setup()` runs code once
- `void loop()` runs code continuously

Basic functions:
- Use `pinmode(n, OUTPUT)`in `setup()` to set the pin `n` as an output (does not take input).
- Use `digitalWrite(n, value)` to deliver power to digital pin `n`.  `value` can be `HIGH`, `LOW`, `0`, `1` (or other values with `analogWrite`).
- Use `delay(ms)` to wait `ms` milliseconds and protect components


Use `//` or `/* */` to create inline or multiline comments which are ignored by the compiler.

Use a header comment at the start of the code to describe what the code does, who wrote it and when.

Use a diode facing opposite current with a DC motor so when the circuit is turned off and the magnetic field collapses, residual current can dissipate through the diode instead of damaging the motor.

Use a capacitor with a motor to filter out high frequency electrical noise.

Use `digitalRead(pin)` to poll the input value from a pin.
Why does temperature sensor, slide switch enxtra extra 9v supply?

Use `Serial.print()` to print a message to the serial monitor.

Use `Serial.begin(9600)` to open the serial port at 9600 bits/s.

Use `map(temperature, 20, 358, 0, 30)` to map/linearly interpolate the temperature range (20-358) to degrees C (0-30).
The function more generally speaking maps one scale to another.











