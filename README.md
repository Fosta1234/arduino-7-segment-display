# Arduino 1-Digit 7-Segment Display Counter

A numeric counter that cycles from 0 to 9 using a 1-digit 7-segment LED display and an Arduino Uno.

## 📖 Project Overview
This project demonstrates how to control individual LED segments to form numeric characters. It serves as a foundation for digital clocks, scoreboards, and countdown timers.

## ⚙️ Working Principle
*   **Segment Mapping:** A 7-segment display consists of 7 LEDs (segments a-g) and a decimal point (dp). To display a number, the Arduino must pull specific digital pins HIGH or LOW based on the display type.
*   **Common Terminal:**
    *   **Common Cathode (CC):** All negative terminals are tied to GND. Segments light up when a pin is set to `HIGH`.
    *   **Common Anode (CA):** All positive terminals are tied to 5V. Segments light up when a pin is set to `LOW`.
*   **Logic:** The code uses an array (or switch-case) to store the bit-patterns for each digit (0-9) and cycles through them with a delay.

## 🛠️ Components Used
*   **Arduino Uno**
*   **1-Digit 7-Segment Display**
*   **8x 220Ω Resistors** (Essential to prevent burning out the LEDs)
*   **Breadboard & Jumper Wires**

## 🔌 Circuit Connections


| Segment | Arduino Pin |
| :--- | :--- |
| **a** | Pin 2 |
| **b** | Pin 3 |
| **c** | Pin 4 |
| **d** | Pin 5 |
| **e** | Pin 6 |
| **f** | Pin 7 |
| **g** | Pin 8 |
| **COM** | GND (for Common Cathode) or 5V (for Common Anode) |

*Note: Connect a 220Ω resistor between each segment pin and the Arduino.*