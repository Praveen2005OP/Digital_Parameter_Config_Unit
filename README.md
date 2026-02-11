# Arduino UNO R4 OLED Display Project

## Overview
This project demonstrates how to interface an OLED display with Arduino UNO R4 using I2C communication. The display shows a welcome message with text rendered on a 128x64 OLED screen.

## IDE Information
- **IDE**: CLion 2025.3.2
- **Platform**: PlatformIO for Arduino development
- **Language**: C++ (Arduino Framework)

## Code Overview
The project initializes an SSD1306 OLED display connected via I2C and displays a simple welcome message. The code:
- Configures serial communication at 9600 baud
- Initializes the OLED display at I2C address `0x3C`
- Displays three lines of text: "Arduino UNO R4", "OLED with I2C", and "Hello Students!"
- Handles initialization errors by halting execution if the display is not found

## Libraries Used
- `Arduino.h` - Arduino core library
- `Wire.h` - I2C communication library
- `Adafruit_GFX.h` - Graphics library for drawing primitives
- `Adafruit_SSD1306.h` - SSD1306 OLED display driver

## Dependencies
Install the following libraries via PlatformIO Library Manager or Arduino Library Manager:
- Adafruit GFX Library
- Adafruit SSD1306 Library

## Hardware Components
- **Microcontroller**: Arduino UNO R4
- **Display**: SSD1306 OLED Display (128x64 pixels)
- **Communication Protocol**: I2C
