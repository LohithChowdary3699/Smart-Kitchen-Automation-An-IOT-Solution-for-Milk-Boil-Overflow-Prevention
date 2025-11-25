# Smart-Kitchen-Automation-An-IOT-Solution-for-Milk-Boil-Overflow-Prevention
Smart Kitchen Automation project that prevents milk boil-over using an ESP32-S3, VL53L0X distance sensor, and SG90 servo. The system detects rising milk levels in real time and automatically reduces heat through servo actuation, ensuring safety, preventing spills, and reducing kitchen waste.
Overview

Milk boil-over is one of the most common kitchen accidents, often resulting in spilling, cleaning effort, waste, and potential stove damage. This project provides a smart, IoT-enabled solution that automatically prevents milk from overflowing using:

VL53L0X Time-of-Flight Distance Sensor

ESP32-S3 T-Display

SG90 Servo Motor for Actuation

Optional Cloud Notifications (Blynk / Firebase)

The system detects rising milk levels in real time and actuates a servo to reduce the stove heat (by turning a knob or triggering a mechanical mechanism), effectively preventing overflow.

Features

Real-time monitoring of milk level using VL53L0X

Hysteresis & filtering to avoid false triggers from steam

Automatic servo actuation to prevent overflow

Local TFT display for status

Optional Blynk/Firebase alerts

Fully open-source, kitchen-safe design

System Architecture
[VL53L0X] --I2C--\
                   \
                    [ESP32-S3 T-Display] --- [TFT UI]
                   /            \
[SG90 Servo] -----/              \--- (Optional Cloud Services)

Hardware Requirements

ESP32-S3 T-Display (LILYGO)

VL53L0X Sensor Module

SG90 Micro Servo

Jumper Wires

USB 5V Power / External Supply (for servo)

3D-Printed or DIY Servo–Knob Coupler

Software Requirements

Arduino IDE or PlatformIO

Libraries:

Adafruit VL53L0X

Servo.h

(optional) Blynk / Firebase / WiFi library
