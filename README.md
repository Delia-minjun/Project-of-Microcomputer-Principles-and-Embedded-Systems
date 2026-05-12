<h1 align="center"> STM32 Smart Desktop Pet (Enhanced Version)</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Hardware-STM32_Minimum_System_Board-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white" alt="MCU" />
  <img src="https://img.shields.io/badge/Sensor-HC--SR04-brightgreen?style=flat-square" alt="Sensor" />
  <img src="https://img.shields.io/badge/Course-Embedded_Systems-blue?style=flat-square" alt="Course" />
</p>

## Overview
This repository contains an open-source, enhanced derivative work of a Smart Desktop Pet. It was developed as the final project for the **Microcomputer Principles and Embedded Systems** course.

Based on an **STM32 Minimum System Board (Core Board)**, the project builds upon an existing open-source desktop pet framework and introduces new hardware interactions and software optimizations. This makes the pet not just visually interactive on the screen, but also spatially aware and capable of physical movement.

## Hardware Setup
- **Core Controller:** STM32 Minimum System Board.
- **Distance Sensor:** HC-SR04 Ultrasonic Module.
- **Actuators:** DC Motors.
- **Display:** Screen module for rendering desktop pet UI and animations.

## Features & My Contributions
- **Basic Desktop Pet Functions:** Inherited from the original framework.
- **Autonomous Obstacle Avoidance:** Integrated an ultrasonic sensor (HC-SR04) to measure distances in real-time. The pet can now autonomously detect obstacles in its path and execute avoidance maneuvers via motor control.
- **Foreground/Background System Optimization:** Adjusted and optimized the original foreground/background control architecture (Interrupt Service Routines and the main loop). This ensures that the real-time processing of ultrasonic sensor data and motor control **does not block or interfere** with the smooth rendering of the UI animations.

## Acknowledgments & Credits
The basic software framework and UI design of this project are based on the fantastic open-source work by **sngelswyh**:
👉 [Original Project Link on OSHWHub (立创开源硬件平台)](https://oshwhub.com/sngelswyh/stm32-smart-desktop-pet)

Special thanks to the original author. My main contributions lie in the hardware extension, the integration of the autonomous obstacle avoidance system, and the restructuring of the foreground/background control logic.
