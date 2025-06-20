# UART LED Control Interpreter

A simple embedded UART-based command interpreter for controlling onboard LEDs using a PIC32 microcontroller. This project reads a single character from the UART terminal and performs LED control actions like turning on/off individual or all LEDs.

## 🛠️ Hardware & Tools
- **Microcontroller**: PIC32MZ2048EFH144  
- **Toolchain**: MPLAB X IDE, XC32 Compiler  
- **Framework**: MPLAB Harmony v2  
- **Terminal**: Any UART serial terminal (e.g., Tera Term, PuTTY)

## 📋 Features
- Menu displayed over UART
- Accepts single-character commands:
  - `'1'` – LED 1 ON  
  - `'2'` – LED 1 OFF  
  - `'3'` – LED 2 ON  
  - `'4'` – LED 2 OFF  
  - `'5'` – LED 3 ON  
  - `'6'` – LED 3 OFF  
  - `'7'` – All LEDs ON

## 🔧 How to Use
1. Flash the firmware onto the PIC32 board.
2. Open a serial terminal at the appropriate baud rate.
3. Type characters `1` to `7` to control LEDs.
4. The menu automatically reprints after each command.

## 📂 Project Structure
- `app.c` – Contains the UART interpreter logic using a simple state machine.
- `app.h` – Application state definitions.

## ✅ Status
✔️ Functional  
💡 Beginner-friendly  
🔁 Easily extendable to more commands or peripherals
