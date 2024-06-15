# Maze-Solving-Robot-with-ArduinoUNO
/*
 * Maze Solving Robot Project Code
 * 
 * Description:
 * This code is for a Maze Solving Robot using an Arduino Uno microcontroller. The robot uses three infrared (IR) sensors 
 * and a color sensor to navigate through a maze. The robot starts at a green line, follows black lines to navigate the maze, 
 * and stops at a red line indicating the end of the maze. The robot is equipped with DC motors controlled by a motor driver circuit.
 *
 * Parts Used:
 * - Arduino Uno (microcontroller)
 * - IR Sensors (KY-033): for line detection
 * - Color Sensor (TCS3200): for detecting the start (green) and end (red) of the maze
 * - DC Motors: for driving the wheels
 * - Motor Driver Circuit: for controlling the speed and direction of the motors
 * 
 * Function of the Code:
 * - Initializes the sensors and motors
 * - Starts the robot when the green line is detected
 * - Follows the black lines using the center IR sensor
 * - Turns left when the left IR sensor detects black
 * - Turns right when the right IR sensor detects black and the left IR sensor detects white
 * - Performs backtracking when a dead-end is detected (all three IR sensors detect white)
 * - Stops the robot when the red line is detected
 */
