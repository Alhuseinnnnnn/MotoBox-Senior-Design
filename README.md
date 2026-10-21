# MotoBox — Intelligent Motorcycle Event Data Recorder

**Senior Design Project | Hamad Bin Khalifa University (HBKU)**

**Field:** Computer Engineering | Embedded Systems | Sensor Technology

**Status:** In Development — Hardware Prototyping

## Project Overview

MotoBox is a senior design project focused on developing an intelligent event data recorder for motorcycles.

The idea is to build a small embedded system that monitors motorcycle movement, detects unusual events such as crashes and potholes, and records sensor data for later analysis.

The project aims to make it easier to understand what happened during a motorcycle incident by collecting motion data before and during an event.

## Project Objectives

- Monitor motorcycle movement using an Inertial Measurement Unit (IMU).
- Identify unusual acceleration and motion patterns.
- Develop a system for detecting possible crashes and potholes.
- Record sensor data for later analysis.
- Design and test a compact hardware prototype suitable for motorcycles.

## Hardware and Technologies

**Microcontroller:** STM32

**Programming Language:** Embedded C

**Development Environment:** STM32CubeIDE

**Communication Protocol:** I2C

**Planned Components:**
- IMU sensor for motion measurements
- MicroSD or external flash storage
- Power regulation and protection circuitry
- Breadboard, connecting wires, and hardware enclosure

## Current Development Progress

### STM32 Firmware

Created an initial STM32 firmware program for scanning the I2C bus and checking whether connected devices respond.

The program:
- Initializes the STM32 microcontroller and I2C interface.
- Scans I2C addresses for connected devices.
- Uses LED blinking patterns to indicate the number of detected devices.
- Reinitializes the I2C interface when no devices respond.

This firmware is an early diagnostic tool used during hardware integration. It does not yet perform crash detection.

### Hardware Prototyping

Currently working on connecting the STM32 microcontroller with external sensors and testing communication between components.

## Repository Structure

```text
MotoBox-Senior-Design/
├── README.md
└── firmware/
    └── i2c_scanner.c
```

**Firmware:** `firmware/i2c_scanner.c`

## Next Development Steps

1. Complete hardware and sensor integration.
2. Read acceleration and gyroscope measurements from the IMU.
3. Develop a system for recording sensor data.
4. Implement and evaluate crash and pothole detection logic.
5. Test the prototype under different movement conditions.

## About the Project

MotoBox is being developed as part of a Computer Engineering senior design project at Hamad Bin Khalifa University.

The project combines embedded programming, hardware prototyping, sensor communication, and engineering problem-solving.

**Note:** This repository documents an ongoing academic project. Features described as planned are not yet completed or validated.
