# Line Follower Robot with ATmega328

The **Line Follower Robot with ATmega328** is a high-performance, feature-rich robot designed to autonomously follow a line path with precision. Equipped with advanced sensors, motor drivers, and intelligent control algorithms, this robot is ideal for educational, research, and competition purposes.

Built around the ATmega328PU microcontroller, it integrates several cutting-edge features such as auto-calibration, path planning, and PID control. The system is powered by a 12V inbuilt rechargeable battery and offers an intuitive interface via a 16x2 LCD display for data monitoring and setting adjustments.

# Line Follower ATmega328

## Images

| **Image 1**                                                               | **Image 2**                                                               |
|----------------------------------------------------------------------------|----------------------------------------------------------------------------|
| ![Image 1](https://github.com/karthirilla/LINE_Follower_ATMEGA328/blob/main/LINE_FOLLOWER_AMTEGA328PU_1.jpg) | ![Image 2](https://github.com/karthirilla/LINE_Follower_ATMEGA328/blob/main/LINE_FOLLOWER_AMTEGA328PU_2.jpg) |

| **Image 3**                                                               | **Image 4**                                                               |
|----------------------------------------------------------------------------|----------------------------------------------------------------------------|
| ![Image 3](https://github.com/karthirilla/LINE_Follower_ATMEGA328/blob/main/LINE_FOLLOWER_AMTEGA328PU_3.jpg) | ![Image 4](https://github.com/karthirilla/LINE_Follower_ATMEGA328/blob/main/LINE_FOLLOWER_AMTEGA328PU_4.jpg) |

## Design
![Design](https://github.com/karthirilla/LINE_Follower_ATMEGA328/blob/main/LINE_FOLLOWER_AMTEGA328PU_DESIGN.jpg)


## Features

### 1. Hardware
- **Microcontroller**: ATmega328PU
- **Sensors**: 14 Photodiode/IR-based sensors for precise black-and-white line detection
- **Motor Driver**: L293D Motor Driver IC
- **Motors**: DC Motor (24mm, 13,000 RPM)
- **Battery**: Inbuilt 12V rechargeable battery for autonomous operation
- **Display**: 16x2 LCD for displaying data and settings
- **Motor Driver MOSFET**: High-efficiency motor control

### 2. Software Features
- **Auto Calibration**: Automatically adjusts the sensors for varying lighting and track conditions
- **Advanced Path Planning**: Optimized for complex curves and intersections
- **Memory Management**: 
  - Dual External EEPROM (256 Kbit each) for memory storage
  - 31 Memory Slots for storing track plans
  - Features to Copy, Insert, Mirror, Delete between memory tracks
  - Auto/Manual Mirror Memory for creating mirrored paths easily
- **Control System**:
  - PID Control for smooth and precise movements
  - Plug and Play Mode: Supports Wireless Manual Control via Bluetooth

## System Architecture

### Components
| Component        | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| **Microcontroller** | ATmega328PU                                                                  |
| **Sensors**         | 14 Photodiodes/IR sensors for black/white detection                          |
| **Motor Driver**    | L293D + MOSFET Driver for efficient motor control                            |
| **Motors**          | 24mm DC Motors, 13,000 RPM                                                   |
| **Display**         | 16x2 LCD                                                                     |
| **Battery**         | 12V rechargeable battery                                                     |
| **External Memory** | Dual 256Kbit EEPROM                                                          |
| **Wireless Control** | Bluetooth module for manual wireless control                                |

### Software Tools
- **Arduino IDE**: Programming the ATmega328PU microcontroller
- **CodeVision AVR**: Advanced AVR programming and debugging
- **AVRDUDESS**: Flashing firmware onto the ATmega328 microcontroller
- **DipTrace**: PCB design software for schematic and layout
- **Proteus**: Circuit simulation for testing and validation

## Features Breakdown

### Sensors
- **14 Photodiodes/IR Sensors**: Provides high accuracy for detecting black and white lines, even in challenging lighting conditions.

### Calibration
- **Auto Calibration**: Automatically adjusts sensitivity based on track conditions to ensure consistent performance.

### Memory Management
- **Dual EEPROM**: Stores up to 31 track paths with features to copy, insert, mirror, delete, and manage memory tracks.
- **Auto/Manual Mirror Mode**: Allows quick creation of mirrored paths.

### Path Control
- **PID Controller**: Ensures smooth and precise line-following by dynamically adjusting motor speed and direction.
- **Advanced Path Planning**: Handles sharp turns, curves, and intersections efficiently.

### Motor and Driver
- **L293D Motor Driver**: Controls the high-speed DC motors with additional MOSFET-based driver for improved efficiency.
- **Motors**: 24mm DC motors with a speed of 13,000 RPM, providing excellent maneuverability.

### Display and Wireless
- **16x2 LCD**: Displays runtime parameters, settings, and calibration data.
- **Bluetooth Control**: Allows wireless manual control using a mobile app or Bluetooth terminal.

## Circuit Design and Simulation
- **PCB Design**: Created using DipTrace for the ATmega328PU and L293D-based circuit.
- **Simulation**: Simulated in Proteus to test the logic and hardware.

## Getting Started

### Prerequisites
Before starting, make sure to install the following software:
- **Arduino IDE**
- **CodeVision AVR**
- **AVRDUDESS**
- **DipTrace**
- **Proteus**

### Hardware Setup
Assemble the hardware components as per the provided PCB design.

### Steps to Run
1. **Clone the Repository**:
    ```bash
    git clone https://github.com/your-username/Line-Follower-ATmega328.git
    ```
2. **Upload Code**: 
   - Upload the firmware to the ATmega328PU using Arduino IDE or CodeVision AVR.
3. **Calibrate Sensors**:
   - Use the auto-calibration feature to set up the robot for the specific track.
4. **Run the Robot**:
   - Place the robot on the track and let it follow the line autonomously.

## Future Enhancements
- Add **Obstacle Detection** using ultrasonic sensors.
- Implement **Speed Optimization** algorithms for racing competitions.
- Integrate **Wi-Fi Control** for enhanced remote monitoring and control.
- Expand memory capabilities for more track storage.
- Add **Voice Commands** using advanced Bluetooth modules.

## License
This project is licensed under the **MIT License**. See the LICENSE file for details.

## Acknowledgments
- Special thanks to the open-source community for the libraries and tools used in this project.
- Inspired by academic projects and robotics competitions.

## Contact
For any inquiries, feel free to reach out:

- Email: [karthikrilla@gmail.com](mailto:karthikrilla@gmail.com)
- LinkedIn: [Karthi C](https://www.linkedin.com/in/karthic)
