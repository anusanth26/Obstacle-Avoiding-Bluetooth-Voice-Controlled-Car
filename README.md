# Obstacle Avoidance Car

## Overview
This project is an Arduino-based obstacle avoidance car that can move forward, backward, left, and right based on ultrasonic sensor input. It also supports Bluetooth and voice control for remote operation. The car is powered by an Arduino board, a motor driver, and a servo-mounted ultrasonic sensor for real-time obstacle detection.

## Features
- **Obstacle Avoidance:** Uses an ultrasonic sensor to detect obstacles and navigate around them.
- **Bluetooth Control:** Can be controlled using Bluetooth commands.
- **Voice Control:** Responds to voice commands to move in different directions.
- **Motor Control:** Uses an Adafruit motor shield to drive four DC motors.

## Components Used
- Arduino board
- Adafruit Motor Shield
- HC-SR04 Ultrasonic Sensor
- Bluetooth module (e.g., HC-05)
- Servo motor
- 4 DC motors
- Power supply (Battery pack)

## Pin Configuration
| Component         | Pin |
|-------------------|-----|
| Ultrasonic Trig   | A1  |
| Ultrasonic Echo   | A0  |
| Servo Motor       | 10  |
| Motor 1           | M1  |
| Motor 2           | M2  |
| Motor 3           | M3  |
| Motor 4           | M4  |

## Code Explanation
- The car continuously checks for obstacles using the ultrasonic sensor.
- If an obstacle is detected within 12 cm, it stops, moves backward, and looks for a clear path before proceeding.
- The Bluetooth module allows for remote control via serial communication.
- Voice commands are processed similarly to Bluetooth commands, enabling hands-free operation.

## Commands
| Command | Action |
|---------|--------|
| F       | Move forward |
| B       | Move backward |
| L       | Turn left |
| R       | Turn right |
| S       | Stop |
| ^       | Move forward (Voice) |
| -       | Move backward (Voice) |
| <       | Turn left (Voice) |
| >       | Turn right (Voice) |
| *       | Stop (Voice) |

## Installation & Usage
1. Connect all components as per the circuit diagram.
2. Upload the provided code to the Arduino using the Arduino IDE.
3. Use a Bluetooth terminal app to send control commands or integrate a voice control system.
4. Power the car and test movement and obstacle avoidance functionality.


