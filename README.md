# 2D_PLOTTER

The code will involve two main parts:

Arduino Code: To control the motors based on the input commands.
Python Code: To process an image and generate the necessary movement commands for the Arduino.

Arduino Code

This code sets up the stepper motors and the pen's servo motor.
listens to the serial port for G-code-like commands
The processCommand function decodes the command, moves the motors to the specified positions, and controls the pen's position (up or down).

Python Code

This code reads an image, converts it to a binary format, and finds the contours.
sends movement commands to the Arduino over a serial connection.
Each point of the contour is translated into a movement command for the plotter.
