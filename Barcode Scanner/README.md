**Light-Based Barcode Reader Prototype with Automated Scanning**

This project involves analyzing Light Dependent Resistor (LDR) values to determine the widths of alternating black and white stripes on paper, simulating barcode patterns.
It also features an automated scanning process using a stepper motor to move the paper and capture readings.  <br>

Concept: Swiping the stripped paper between an LDR and LED next to each other, The value of resistance and hence voltage accross it decreases for white strip and increases for black.
We store those analog values in an array, for some intervals of steps of stepper motor; and after plotting them as shown in the demonstration video, we see that taking average of all values,
we can roughly say that the values above average value are black strips and those below are white strips.
By keeping a threshold for when the graph stays above average for one cycle we can distinguish wider black strips and thinner black strips (same can be done for white too)
Hence, we can encode different permutations of wider and thinner black and white strips and print them into a barcode√.    <br>

Standby: The device constantly takes average of ldr values for ambient light and sudden change in value from the average indicates that barcode is detected.  <br>

An IR sensor if it could have detected black strips would be much easier to use.  <br>
Components Used:
Light Dependent Resistance (LDR)
LED and 220 ohm resistance
Stepper motor
ULN driver for Stepper motor
BreadBoard Powersupply: For powering stepper motor
Arduino UNO
Rack and Pinion gear mechanism
Computer for analyzing values
Wires and Breadboard
