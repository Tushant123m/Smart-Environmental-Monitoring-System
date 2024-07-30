# Smart Environmental Monitoring System

## Overview

The Smart Environmental Monitoring System is designed to measure and report various environmental parameters such as air quality, temperature, humidity, and light intensity. This project utilizes the STM32F401RE microcontroller along with several sensors to provide real-time data. The system is built using HAL libraries and STM Cube MX, ensuring simplicity and ease of use with affordable components.

## Hardware Used

- **STM32F401RE**: The main microcontroller that handles data acquisition and processing.
- **MQ135**: Air quality sensor for detecting various gases.
- **DHT11**: Sensor for measuring temperature and humidity.
- **LDR**: Light-dependent resistor for measuring light intensity.
- **LCD Display (Additional)**: For displaying sensor readings. (Is implemented in current version)

## Software Used

- **STM32CubeMX**: For initializing the STM32F401RE peripherals.
- **HAL Libraries**: For hardware abstraction and easier coding.

## Features

- Measures and reports air quality, temperature, humidity, and light intensity.
- Uses affordable and easy-to-build methods.
- Code is centralized in a single `main.c` file for simplicity, though this might affect performance.

## Setup Instructions

1. **Hardware Connections:**
   - Connect the MQ135 sensor to the STM32F401RE.
   - Connect the DHT11 sensor to the STM32F401RE.
   - Connect the LDR to the STM32F401RE.
   - (Optional) Connect an LCD display to the STM32F401RE.

2. **Software Configuration:**
   - Open STM32CubeMX and configure the peripherals.
   - Generate the initialization code using STM32CubeMX.
   - Import the generated code into your IDE.
   - Implement sensor reading and data processing in the `main.c` file.

## Usage

- Upload the code to your STM32F401RE.
- Open the Serial Monitor to view the sensor readings.
- Use the sensor data for your specific applications.

## Acknowledgements

- Thanks to the creators of STM32CubeMX and HAL libraries for providing the tools needed to simplify development.
