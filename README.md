# PID-Line-Follower-Robot
This is my attempt at programming and building a wheeled robot that follows a line as it twists and curves using a programmed PID controller.
The motivation behind this project is to understand real world applications of the PID controller.

# Tools
The Robot will use two DC motors to push itself forward, and utilize a DC motor driver for complete control over each motors speed which will allow us to control the robots direction as well.
The robot will also be powered by two Li-Ion batteries The IR sensors will help us with the error correction and will tell the robot how far it is from the black line.
All of these components will connect to the Arduino which is the main microcontroller we will run our program on.
- Computer with Arduino IDE
- 1x Arduino microcontroller (can use others)
- 1x L298N DC motor driver
- 1x 360 degree rotating swivel wheel
- 1x boost converter
- 2x DC motors (3V - 6V)
- 2x Standerd Rubber Wheels
- 2x 18650 Li-Ion batteries
- 4x IR Sensors

# Block Diagram
The block diagram below shows how all the components connect together.

The robot will be powered by two 3.7V Li-Ion batteries which will be connected to the DC motor driver. Since the DC motor driver can take no less than 12V, we'll use a
boost converter to boost from 3.7V to 12V. The two DC motors which will allow the robot to move forward and turn will also be connected to the IN ports of the DC motor Driver. The motor driver will output 5V to power the Arduino

The IR sensors connect to the Arduino and send whether the black line is detected or not and send that as a digital OUT signal of either 1 or 0. 
![image alt](https://github.com/FaisalW15/PID-Line-Follower-Robot/blob/main/PID_Line_Follower_Block_Diagram.png?raw=true)
