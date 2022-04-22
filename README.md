DC SERVO MOTOR CONTROLLER


This is a port of the very sophisticated DC Servomotor Controller SMC3 by Elm Chan for the ATmega328.

It includes the results of a detailed analysis of the inner workings of the source code and (hopefully) more beginner-friendly explanation of the meaning of the control parameter and how to choose sensible values for the desired application.

This analysis includes a full translation of the assembler code into C code. This was started as a tool to understand the inner workings of SMC3 but it is turning into a full project of its own right now.

The program logic is as close to the carefully optimized assembler version as possible, but it is much easier to read than the highly optimized hand-crafted assembler masterpiece by Elm Chan.

It relies on the Arduino environment for the UART part and some initializations, but the resulting code behaves identical to the original version. The main point is to show the internal logic and to be a more accessible base for modifications. The price for this convienence is a much bigger binary size: 4.8kB instead of 1.8kB
