# 3-finger-bionic-arm

A 3-finger bionic/prosthetic arm designed as an affordable and modular assistive device, combining mechanical design, 3D-printed components, servo-based actuation, and embedded control.
**Team Size:** 5 Members  
**My Role:** Mechanical Design

## Project Overview

The **Bionic Arm** is a mechanically actuated prosthetic hand developed to demonstrate coordinated finger movement and gripping using a compact electromechanical system.

The arm uses a **3-finger mechanism with 4-bar-driven actuation**, designed to provide coordinated and controlled finger motion while keeping the mechanical structure lightweight and relatively simple to manufacture.

The complete system integrates:

- CAD-based mechanical design
- 3D-printed structural components
- Servo-based finger actuation
- Embedded control using ESP32-S3
- Servo motor driver for multi-actuator control
- Mechanical linkage and 4-bar mechanisms
- Multiple control modes for operation

## Key Features

- 3-finger prosthetic hand mechanism
- 4-bar-driven finger actuation
- CAD-designed mechanical structure
- 3D-printed components
- Multiple servo motors for finger movement
- ESP32-S3 based embedded control
- Modular mechanical and electronic architecture
- Lightweight and compact design
- Designed for controlled gripping and assistive applications

## Mechanical Design

The mechanical structure was developed using CAD to design and integrate the palm, fingers, linkages, mounting components, and wrist/forearm structure.

A **4-bar linkage mechanism** is used for finger actuation to achieve coordinated motion while maintaining a compact mechanism.

The components were designed with consideration for:

- Mechanical strength
- Weight reduction
- Ease of assembly
- Joint and linkage motion
- Servo mounting
- 3D-printability
- Modular component replacement

## Manufacturing

The structural components were manufactured using **3D printing**.

### Materials Used

- ASA Filament
- PETG-CF

The selection of materials was based on the required mechanical strength, stiffness, dimensional stability, and suitability for functional 3D-printed components.

## Electronics & Actuation

The arm uses servo motors controlled through a dedicated servo driver and an ESP32-S3 development board.

### Main Electronics

| Component | Quantity |
|-----------|----------|
| ESP32-S3 Xiao Board | 1 |
| Waveshare Servo Motor Driver | 1 |
| Waveshare SC09 Servo Motor | 3 |
| Waveshare SC3235 Servo Motor | 1 |
| LiPo 2000 mAh Battery | 2 |
| Bucket Module | 1 |

### Mechanical / Manufacturing Materials

| Component | Quantity |
|-----------|----------|
| ASA Filament | 1 |
| PETG-CF | 2 |

## System Architecture

```text
             ┌─────────────────────┐
             │     ESP32-S3        │
             │  Embedded Control   │
             └──────────┬──────────┘
                        │
                        ▼
             ┌─────────────────────┐
             │ Servo Motor Driver  │
             └──────────┬──────────┘
                        │
             ┌──────────┴──────────┐
             │                     │
             ▼                     ▼
       SC09 Servo Motors      SC3235 Servo
             │                     │
             └──────────┬──────────┘
                        ▼
             ┌─────────────────────┐
             │ Mechanical Linkage  │
             │   & 4-Bar System    │
             └──────────┬──────────┘
                        ▼
             ┌─────────────────────┐
             │   3-Finger Hand     │
             │  Gripping Mechanism │
             └─────────────────────┘
