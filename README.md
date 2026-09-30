# Fire-Fighting Robot

# Project Overview

The Fire-Fighting Robot is an autonomous sensor-based robotic prototype designed to detect and locate a flame source, navigate through a controlled environment, avoid obstacles, respond to line boundaries, and activate a fan-based fire-suppression mechanism. The system combines multiple flame sensors, IR-based sensing, line sensors, dual DC motor control, TB6612FNG motor-driver interfacing, sensor calibration, and PID-based control logic for real-time robotic operation.

The robot continuously analyzes sensor inputs and makes movement decisions according to the detected environment. It prioritizes obstacle avoidance, line detection, and flame detection before performing normal forward movement. When a flame is detected, the robot stops normal navigation and enters a flame-localization routine to determine the strongest flame direction, approaches the detected source, activates the fan for suppression, and then performs a recovery movement.

The project demonstrates the integration of embedded programming, analog sensor processing, PWM motor control, autonomous navigation, flame localization, obstacle avoidance, line-sensor calibration, and automated fire suppression in a single robotic system.

# Hardware Components

The project uses the following major hardware components:

- Arduino-Compatible Microcontroller

- Flame Sensors

- Line Sensors

- IR-Based Obstacle Sensing

- TB6612FNG Dual Motor Driver

- Two DC Motors

- Fan-Based Suppression Mechanism

- Push Buttons / Control Inputs

- Robot Chassis and Power Supply

# Programming Languages & Technologies

- C++
- Arduino IDE

# Working Flow
1. Power ON – The robot initializes its sensors, motors, and control pins before starting operation.
2. Start Input – The robot waits for the initial control input to begin the sensor calibration process.
3. Line Sensor Calibration – The robot rotates and records minimum and maximum readings from the line sensors.
4. Autonomous Mode – After the second control input, the robot continuously monitors its sensors and controls its movement.
5. Obstacle Detection – IR-based sensors detect obstacles and trigger reverse-and-turn movements to avoid them.
6. Line Detection – Calibrated line sensors detect boundaries and control the robot's reverse and turning response.
7. Flame Detection – Multiple flame sensors continuously monitor the environment for the presence of a flame.
8. Flame Localization – When a flame is detected, the robot rotates and compares sensor readings to identify the strongest flame direction.
9. Flame Approach – The robot aligns itself with the detected flame direction and moves toward the flame.
10. Fire Suppression – The robot stops near the flame and activates the fan-based suppression mechanism for approximately three seconds.
11. Recovery Movement – After suppression, the robot turns off the fan, reverses, turns, and resumes its programmed movement.

# Applications

The concept demonstrated by this prototype can be explored for:

1. Industrial Safety — supporting fire-response systems in controlled industrial environments.
2. Warehouses — monitoring and responding to localized fire hazards.
3. Hazardous Areas — reducing the need for immediate human access to certain dangerous locations.
4. Fire-Prone Environments — serving as a prototype for autonomous fire-response systems.
5. Emergency Response Research — studying robotic assistance in hazardous situations.
6. Educational Robotics — demonstrating sensor integration and autonomous decision-making.
7. Robotics & Automation Research — developing autonomous emergency-response robots.
