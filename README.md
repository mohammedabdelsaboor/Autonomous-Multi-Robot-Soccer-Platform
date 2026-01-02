# Heterogeneous Multi-Robot Soccer Framework (ROS 2)
![image](https://github.com/user-attachments/assets/806d6eb5-237f-4fae-aac8-5a283b942cc4)

## Project Description
This repository presents a heterogeneous multi-robot soccer system developed using ROS 2. The system consists of two autonomous mobile robots operating in a football-like environment with two goals and a single ball. Each robot independently perceives the environment, plans its motion, and executes control actions in real time.

The project aims to study perception, navigation, and control in competitive multi-robot scenarios using a modular and scalable software architecture.

---

## Robotic Platforms
The system includes two heterogeneous robots:
- A three-wheel omni-directional mobile robot designed for high maneuverability.
- A four-wheel mecanum mobile robot designed for stable holonomic motion.

---

## Sensors and Actuation
Each robot is equipped with:
- Two onboard cameras for ball and goal detection.
- One overhead camera for global environment observation.
- Two LiDAR sensors for localization, path planning, and dynamic obstacle avoidance.
- A servo-actuated gripper for ball handling.
- An infrared (IR) sensor for reliable ball possession detection.

Low-level motor and actuator control is executed on Arduino microcontrollers, while high-level decision making is handled within ROS 2.

---

## Software Architecture
The system follows a layered ROS 2 architecture:
- Perception layer for object detection and state estimation.
- Navigation layer for path planning and obstacle avoidance.
- Strategy layer for decision making and behavior selection.
- Control layer for velocity generation.
- Communication layer for serial interaction with Arduino.

This modular design allows easy extension, testing, and integration of additional robots or algorithms.

---

## Repository Structure
