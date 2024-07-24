# Depression Checker

Depression Checker is an embedded system project designed to monitor behavioral patterns and environmental factors that could indicate symptoms of depression, particularly in Canadian youth aged 15-17.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Hardware Requirements](#hardware-requirements)
- [Software Requirements](#software-requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Scientific Principles](#scientific-principles)
- [Contributing](#contributing)

## Overview

This project aims to support users who may be experiencing symptoms of depression by monitoring behavioral patterns and environmental factors. It uses various sensors to track activity levels, light exposure, and sleep patterns, providing feedback through LEDs and a vibration motor.

## Features

- Motion detection using PIR sensor
- Ambient light sensing
- Real-time clock for time-based analysis
- LED indicators for normal operation and potential depression symptoms
- Vibration alert for user notification
- LCD display for user interaction and information

## Hardware Requirements

- STM32F401RE Nucleo Board
- PIR Motion Sensor
- BH1750 Light Sensor
- DS3231 RTC Module
- Vibration Motor
- LEDs (Red and Green)
- 16x2 LCD Display (HD44780 compatible)
- Breadboard and jumper wires

## Software Requirements

- STM32CubeIDE
- STM32 HAL libraries

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/depression-checker.git
   ```

2. Open the project in STM32CubeIDE.

3. Connect the hardware components according to the circuit diagram (refer to the design document).

4. Build and flash the project to your STM32F401RE Nucleo Board.

## Usage

1. Power on the device.
2. The LCD will display a welcome message.
3. The system will start monitoring the environment and user activity:
   - Green LED indicates normal operation.
   - Red LED and vibration indicate potential depressive behavior.
4. The LCD will display the current status and time of inactivity.
5. If concerning patterns are detected, consider increasing light exposure, activity levels, or engaging in hobbies.

**Note**: This device provides environmental feedback only, not medical advice. Consult a health professional with any concerns.

## Scientific Principles

The project utilizes several scientific and mathematical principles:

1. **Ohm's Law and Kirchhoff's Laws**: Used for circuit analysis and power calculations.
2. **Statistical Distribution**: Analyzes sleep patterns using standard deviation to identify potential depression indicators.
3. **Probability Distribution**: Determines the likelihood of depression based on inactivity periods during different times of the day.

For detailed explanations of these principles, refer to the design document.

## Contributing

Contributions to improve the project are welcome. Please feel free to fork the repository, make changes, and submit pull requests. Some ideas for improvements:

- Implement machine learning algorithms for more accurate detection
- Add cloud connectivity for data logging and analysis
- Develop a companion mobile app for extended functionality

## Disclaimer

This project is for educational and informational purposes only. It is not a substitute for professional medical advice, diagnosis, or treatment. Always seek the advice of your physician or other qualified health provider with any questions you may have regarding a medical condition.
