# 🚗 Car Black Box (CBB)

## 📌 Project Overview
The **Car Black Box (CBB)** is a microcontroller-based embedded system designed to continuously monitor and log critical driving events for post-incident analysis. Inspired by black boxes used in aviation, this system is tailored for automotive environments to track anomalies such as **over-speeding**, **sudden braking**, or **system faults**.

The project uses a **PIC microcontroller (e.g., PIC16F877A)** and peripherals like potentiometers (as analog input sources), and stores event data into **EEPROM** for non-volatile logging.

---

## 🚦 Key Features
- Real-time monitoring of driving conditions
- Detection and logging of events like over-speeding
- Event logging in EEPROM with timestamps (if RTC is added)
- Peripheral interaction using ADC (e.g., speed simulation via potentiometer)
- Efficient interrupt-based system design
- Can be extended for GPS, crash sensor, or communication modules

---

## 🧠 Pre-requisites
To work on or understand this project, knowledge in the following areas is essential:
- **PIC microcontroller programming** (e.g., PIC16F877A)
- **Microcontroller schematics and interfacing**
- **Peripheral handling** using ADC (e.g., potentiometer)
- **Interrupt service routines (ISR)**
- Familiarity with **MPLAB X IDE** and **XC8 compiler**

---

## 🔧 Tools & Technologies
- **Microcontroller**: PIC16F877A
- **Software**: MPLAB X IDE, XC8 Compiler
- **Communication**: UART (optional for debug)
- **Storage**: EEPROM (internal or external)
- **Peripheral Simulations**: Potentiometer (speed sensor), LEDs, etc.

---

## 🧰 File Structure 
```
car_black_box_project.X/
│
├── main.c          → Main program, super loop, state machine
├── main.h          → All header includes and flag definitions
├── car_black_box.c → Core logic (dashboard, login, menu, logs)
├── adc.c / adc.h   → ADC configuration for speed reading
├── clcd.c / clcd.h → Character LCD display functions
├── keypad.c        → Digital keypad (5 push buttons)
├── ds1307.c        → RTC (Real Time Clock) functions
├── eeprom.c        → External EEPROM read/write functions
├── i2c.c           → I2C communication protocol
├── timers.c        → Timer2 configuration (login timeout)
└── uart.c          → UART serial communication
---

---------
## 👨‍💻 Author
**Oruganti Lalasa Yadav**
Embedded Systems Project — Car Black Box
PIC16F877A | MPLAB XC8 | PICSimLab
----------
