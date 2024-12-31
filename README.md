# **S2 Controller Board**
![IMG_2460 2](https://github.com/user-attachments/assets/6cf9a933-7dae-4a53-ab7a-b865757b496b)# 

## **Overview**
The S2 Controller Board is a custom-designed PCB created for our university's Competitive Robotics team. It serves as a compact and efficient solution to streamline our robot's control systems. This board is a core component of the new drivetrain we've been developing.

## **Problem Statement**
Previously, our robots relied on circuits made up of several interconnected perfboards, resulting in a messy and inefficient setup. The S2 Controller Board consolidates these individual modules into a single PCB, providing a cleaner, more organized, and reliable solution for our robots. 


## **Features**
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


## **Technical Specifications**
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

## **Bill of Materials (BOM)**

| ID  | Name         | Designator     | Footprint                           | Quantity | Manufacturer Part         |
|-----|--------------|----------------|-------------------------------------|----------|---------------------------|
| 1   | BUZZER       | BUZZER1        | BUZ-TH_BD12.0-P6.00-D0.9-RD         | 1        | buzzer                    |
| 2   | 10uF         | C1             | CAP-TH_BD4.0-P1.50-D0.8-FD          | 1        | KS106M050C07RR0VH2FP0     |
| 3   | 22uF         | C2             | CAP-TH_BD4.0-P1.50-D0.8-FD          | 1        | KS106M050C07RR0VH2FP0     |
| 4   | MPU-6050     | IMU1           | MPU-6050                            | 1        |                           |
| 5   | 5VPWR        | LED1           | LED-5MM-5MM                         | 1        |                           |
| 6   | 3V3VPWR      | LED2           | LED-5MM-5MM                         | 1        |                           |
| 7   | I2C_1        | P5             | CONN-TH_4P-P2.50-XH2.54-4P          | 1        | XH-2.54-4P                |
| 8   | I2C_2        | P6             | CONN-TH_4P-P2.50-XH2.54-4P          | 1        | XH-2.54-4P                |
| 9   | I2C_4        | P7             | CONN-TH_4P-P2.50-XH2.54-4P          | 1        | XH-2.54-4P                |
| 10  | I2C_3        | P8             | CONN-TH_4P-P2.50-XH2.54-4P          | 1        | XH-2.54-4P                |
| 11  | 220Ω         | R1,R2,R3,R4,R5 | R_AXIAL-0.4                         | 5        |                           |
| 12  | ESP32        | U1             | COMM-TH_NODEMCU-32SLUA              | 1        | NodeMCU-32SLua            |
| 13  | OLED Display | U2             | OLED-TH_OLED0.96-I2C                | 1        | ZJY096S0700BG01蓝色       |
| 14  | MCP2515      | U3             | MCP2515                             | 1        |                           |
| 15  | RGB-LED      | U4             | LED-TH_4P-BD5.8-P1.30               | 1        | LED-RGB 共阴 插件 直径5mm |
| 16  | POWER-JACK   | U5             | DC-IN-TH_POWER-JACK                 | 1        | POWER-JACK                |
| 17  | PWR_SWITCH   | U6             | HDR-TH_2P-P2.54-V-F                 | 1        | KH-2.54FH-1X2P-H8.5       |
| 18  | LD33CV       | U7             | TO-220                              | 1        | LD33CV                    |
| 19  | ESP_HEADER   | U8,U9          | HDR-TH_19P-P2.54-V-F                | 2        | KH-2.54FH-1X19P-H8.5      |
| 20  | SPI_4        | U10            | JST_XH_B06B-XH-A_06X2.50MM_STRAIGHT | 1        | JST_XH CONNECTOR          |
| 21  | SPI_3        | U11            | JST_XH_B06B-XH-A_06X2.50MM_STRAIGHT | 1        | JST_XH CONNECTOR          |
| 22  | SPI_2        | U12            | JST_XH_B06B-XH-A_06X2.50MM_STRAIGHT | 1        | JST_XH CONNECTOR          |
| 23  | SPI_1        | U13            | JST_XH_B06B-XH-A_06X2.50MM_STRAIGHT | 1        | JST_XH CONNECTOR          |
| 24  | I2C_Selector | U14            | HDR-TH_2P-P2.54-V-F                 | 1        | KH-2.54FH-1X2P-H8.5       |
| 25  | AUX          | U15            | HDR-TH_2P-P2.54-V-F                 | 1        | KH-2.54FH-1X2P-H8.5       |
| 26  | 5v_TP        | U16            | HDR-TH_2P-P2.54-V-F                 | 1        | KH-2.54FH-1X2P-H8.5       |
| 27  | 3v3_TP       | U17            | HDR-TH_2P-P2.54-V-F                 | 1        | KH-2.54FH-1X2P-H8.5       |


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

