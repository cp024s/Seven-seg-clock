# Mechanical 7 Segment Display Clock using an Arduino

This project involves creating a mechanical 7-segment display clock using an Arduino and 28 servos. 

## Table of Contents
1. [Introduction](#introduction)
2. [Components Required](#components-required)
3. [Tools Required](#tools-required)
4. [Circuit Diagram](#circuit-diagram)
5. [Assembly Instructions](#assembly-instructions)
6. [Programming the Arduino](#programming-the-arduino)
7. [Testing and Calibration](#testing-and-calibration)
8. [Troubleshooting](#troubleshooting)
9. [Acknowledgements](#acknowledgements)

## Introduction
This project demonstrates how to build a mechanical clock using an Arduino, which controls 28 servos to form the digits on a 7-segment display. This unique approach provides a visually engaging way to display the time. By following these instructions, you will create a functional and eye-catching clock that can be a great addition to any room or a fun project to enhance your electronics and programming skills.

## Components Required
To build the mechanical 7-segment display clock, you will need the following components:

- **Arduino (e.g., Arduino Uno)**: This microcontroller will be the brain of the project, controlling the servos and processing the time data from the RTC module.
- **28 Micro Servos (e.g., SG90)**: These servos will be used to move the segments of the display to form the digits.
- **Real-Time Clock (RTC) Module (e.g., DS3231)**: This module keeps track of the current time, providing accurate time data to the Arduino.
- **Power Supply for Servos**: A separate power supply is necessary to ensure the servos receive sufficient power without overloading the Arduino.
- **Jumper Wires**: These wires will be used to connect the components together.
- **Breadboard or PCB**: Useful for organizing and connecting the electronic components.
- **3D Printed Parts for the Clock**: The frame and segment holders need to be 3D printed to hold the servos and segments in place.

## Tools Required
To assemble and complete this project, you will need the following tools:

- **Soldering Iron and Solder**: Used for making secure electrical connections between components.
- **3D Printer**: Required to print the frame and segment holders that will house the servos and create the mechanical structure of the clock.
- **Screwdrivers**: Necessary for mounting the servos and assembling the 3D printed parts.
- **Hot Glue Gun (optional)**: Can be used to provide additional support and security for the components if needed.

## Circuit Diagram
Connect the servos to the Arduino following the schematic below:

- **Power**: Connect all servo power lines to an external 5V power supply to ensure they receive adequate power.
- **Ground**: Connect all servo grounds to the external power supply ground, and ensure this is also connected to the Arduino ground to maintain a common reference point.
- **Signal Pins**: Connect the signal wire of each servo to a digital pin on the Arduino, assigning each servo a unique pin.

Ensure the RTC module is connected to the I2C pins on the Arduino (typically A4 and A5 for SDA and SCL respectively on the Arduino Uno).

## Assembly Instructions
1. **3D Printing**: Use a 3D printer to print the frame and segment holders. The design files for these parts can be found on the project page.
2. **Mounting Servos**: Attach each of the 28 micro servos to the segment holders. Ensure that each servo is securely mounted and can move freely.
3. **Wiring**: Connect each servo to the appropriate pins on the Arduino and the external power supply. Follow the circuit diagram closely to avoid miswiring.
4. **RTC Module**: Connect the RTC module to the Arduino’s I2C pins. Ensure proper connection to enable accurate timekeeping.

## Programming the Arduino
1. **Install the necessary libraries**: Ensure you have the Servo library (pre-installed with the Arduino IDE) and the RTClib library (available through the Arduino Library Manager) installed.
2. **Upload the Code**: Use the code provided on the DIY Life website, which includes logic for controlling the servos and reading the time from the RTC module. Upload this code to the Arduino using the Arduino IDE.

## Testing and Calibration
After assembling and programming, follow these steps to test and calibrate your clock:

1. **Power On**: Turn on the power supply for the servos and the Arduino.
2. **Initial Test**: Observe the initial movements of the servos to ensure they are responding correctly.
3. **Calibration**: Adjust the positions of the servos if necessary to ensure that each segment aligns correctly to form the digits. This may require modifying the servo angles in the code or physically adjusting the servo mounts.
4. **Time Setting**: Ensure the RTC module is set to the correct time. This can typically be done through the code or using an additional program to set the RTC.

## Troubleshooting
If you encounter any issues, consider the following troubleshooting steps:

- **Servo Movement Issues**: Check the connections and power supply to ensure the servos are receiving adequate power.
- **Incorrect Time Display**: Verify the connections and code for the RTC module. Ensure it is properly initialized and communicating with the Arduino.
- **Calibration Problems**: Revisit the calibration process, ensuring the servos are correctly aligned and the angles in the code are accurate.

## Acknowledgements
This project is inspired and guided by the detailed instructions provided by The DIY Life. For further information, additional resources, and community support, visit the project page on The DIY Life website.

Thank you for following this guide. Enjoy building and showcasing your mechanical 7-segment display clock!
