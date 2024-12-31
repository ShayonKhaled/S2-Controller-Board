#S2 Controller Board 
![IMG_2460 2](https://github.com/user-attachments/assets/6cf9a933-7dae-4a53-ab7a-b865757b496b)# 

## Overview
The S2 Controller Board is a custom-designed PCB created for our university's Competitive Robotics team. It serves as a compact and efficient solution to streamline our robot's control systems. This board is a core component of the new drivetrain we've been developing.

## Problem Statement
Previously, our robots relied on circuits made up of several interconnected perfboards, resulting in a messy and inefficient setup. The S2 Controller Board consolidates these individual modules into a single PCB, providing a cleaner, more organized, and reliable solution for our robots. 


## Features
This ESP32-based controller board is packed with functionality designed to simplify robotics development and enhance performance:

- **Onboard Accelerometer**: Provides positional feedback for precise control.
- **CAN Module**: Enables robust communication via the CAN bus, used to control our motors and auxiliary control modules. 
- **I2C and SPI Peripheral Ports**:
  - 4x I2C ports for sensors and other peripherals.
  - 4x SPI ports for additional connectivity.
- **OLED Screen**: Displays real-time status messages for easy diagnostics and debugging.
- **Status Indicator LEDs**: Visual feedback for board status and activity.
- **Buzzer**: Audio alerts for system events or errors.
- **Expansion Capabilities**: Supports additional modules to extend functionality with the pins of ESP32 broken out. 


## Technical Specifications
- **Microcontroller**: ESP32-S2
- **Accelerometer**: MPU-6050
- **Communication Protocol**: CAN bus using MCP2515 and TJA1050.
- **Peripheral Ports**:
  - 4x I2C
  - 4x SPI
- **Other Components**:
  - Status LEDs
  - OLED Display
  - Buzzer
- **Power Supply**: 5V input via barrel jack or USB port on the ESP32 (switchable).

## Gallery
### PCB Design and Assembly
- **Top View of PCB**  
![Top view](https://github.com/user-attachments/assets/dcca1b2f-410e-47dd-a2b5-7d8abb0a3d0b)


- **Bottom View of PCB**  
![Bottom View](https://github.com/user-attachments/assets/d3f1d739-334a-4a00-a5b4-d4fd9b4b915b)


- **3D Render**  
![3D View](https://github.com/user-attachments/assets/cb0cf08d-590a-4b7e-9a43-aad14ba9c385)


### Fully Assembled Board
- **Assembled PCB**
![Assembled Board](https://github.com/user-attachments/assets/66005bf3-4a97-498f-a421-e182f7a061a9)



### Board in Action
- **Controller Installed in Our Robot**
  ![S2 Board Installed in the Robot](https://github.com/user-attachments/assets/c57f9957-f5b0-4c91-9186-2eaf0f77a473)


---

## License
This project is licensed under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html). You are free to use, modify, and distribute this project under the terms of the GPLv3 license.

---

