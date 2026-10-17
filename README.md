 <div align="center">

# Arduino Obstacle Avoiding Robot Car

**An autonomous robot car that detects obstacles and navigates by scanning its surroundings.**

<img src="https://img.shields.io/badge/Arduino-00979D?style=flat-square&logo=arduino&logoColor=white" alt="Arduino">
<img src="https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white" alt="C++">
<img src="https://img.shields.io/badge/Arduino_IDE-1.8.13-00979D?style=flat-square&logo=arduino&logoColor=white" alt="Arduino IDE 1.8.13">
<img src="https://img.shields.io/badge/AFMotor-Library-555555?style=flat-square" alt="AFMotor Library">

</div>

## Project Overview

This project is an Arduino-based autonomous robot car that detects obstacles using an ultrasonic sensor and chooses a direction based on the available distance.

A servo motor rotates the sensor to scan the left and right sides. The robot stops, reverses, compares the measured distances, and turns to avoid obstacles.


<div align="center">
  <img src="Bellabot.jpg" alt="Arduino Obstacle Avoiding Robot Car" width="500">
  <p><i>Arduino-based obstacle-avoiding robot car</i></p>
</div>

## Components Used

- Arduino Uno (or compatible board)
- HC-SR04 Ultrasonic Sensor
- Servo Motor (e.g., SG90)
- L293D-compatible Adafruit Motor Shield V1
- 4 DC Geared Motors
- 4 Wheels and Robot Chassis
- Battery Pack and Jumper Wires

## Working Principle

1. **Distance Measurement:** The HC-SR04 sensor measures the distance to an obstacle in front of the robot.
2. **Forward Movement:** If the measured distance is greater than 35 cm, all four motors move the robot forward.
3. **Obstacle Detection:** If an obstacle is detected within 35 cm, the robot stops and reverses briefly.
4. **Environment Scanning:** The servo rotates the ultrasonic sensor to measure distances on both sides.
5. **Direction Selection:** The robot compares the left and right distance readings and turns toward the side with more space.
6. **Continuous Navigation:** The loop repeats, allowing the robot to detect and avoid obstacles as it moves.

## Hardware Configuration

| Component | Arduino Connection |
|---|---|
| Ultrasonic Trigger | A3 |
| Ultrasonic Echo | A2 |
| Servo Signal | Digital Pin 10 |
| DC Motor 1 | Motor Shield M1 |
| DC Motor 2 | Motor Shield M2 |
| DC Motor 3 | Motor Shield M3 |
| DC Motor 4 | Motor Shield M4 |

## Software & Libraries

- **Arduino IDE 1.8.13** used to write and upload the program.
- **AFMotor Library** controls the DC motors through the compatible Motor Shield V1.
- **Servo Library** controls the servo motor used for scanning.
- **Arduino C++** implements the obstacle detection and movement logic.

## How to Run

1. Install [Arduino IDE 1.8.13](https://www.arduino.cc/en/software).
2. Install the compatible `AFMotor` library.
3. Connect the ultrasonic sensor, servo motor, and motor shield according to the configuration above.
4. Open the Arduino sketch (`.ino`) in the IDE.
5. Select the appropriate Arduino board and COM port.
6. Upload the code and power the robot.

## Key Features

- Autonomous obstacle detection
- Servo-based left and right scanning
- Four-motor movement control
- Distance-based turning decisions
- Adjustable obstacle detection threshold

 ## Connect With Me

<div align="center">

**Kaneez Fatima**

[GitHub](https://github.com/fatimakh905) · [LinkedIn](https://linkedin.com/in/kaneez-fatima-8a1516335/)

</div>

