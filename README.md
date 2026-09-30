# Arduino Fingerprint Door Lock 🔐

A fingerprint-controlled electronic door lock built with an **Arduino UNO**, an optical fingerprint sensor, and an **SG90 servo motor**.

This project was originally developed in **2021 as my high school graduation project (maturski rad)** at the Technical High School in Bugojno, Bosnia and Herzegovina.

The goal of the project was to build a physical prototype of an electronic lock that authenticates a user using their fingerprint and controls a mechanical locking mechanism using a servo motor.

![Arduino Fingerprint Door Lock Prototype](prototype.jpg)

## 📌 About the Project

The system uses an optical fingerprint sensor to scan and identify a fingerprint.

When a registered fingerprint is successfully recognized, the Arduino UNO activates the SG90 servo motor. The rotational movement of the servo is transferred to the mechanical locking mechanism, allowing the lock to switch between its locked and unlocked positions.

Each successful fingerprint recognition changes the current state of the lock.

## 🔧 Hardware

The prototype was built using:

- Arduino UNO
- Optical fingerprint sensor
- SG90 servo motor
- Mechanical door latch
- 9V battery
- Wooden prototype board
- Connecting wires

## 💻 Software

The project was programmed using the **Arduino IDE**.

The Arduino sketch uses the following libraries:

- `Adafruit_Fingerprint`
- `Servo`
- `SoftwareSerial`

The fingerprint sensor communicates with the Arduino through serial communication, while the SG90 servo motor controls the physical locking mechanism.

## ⚙️ How It Works

1. The Arduino initializes the fingerprint sensor and servo motor.
2. The fingerprint sensor waits for a fingerprint.
3. The captured fingerprint is converted and compared with fingerprints stored in the sensor.
4. If a matching fingerprint is found, the Arduino activates the servo motor.
5. The servo moves between approximately **0° and 120°**.
6. The servo movement operates the mechanical latch, locking or unlocking the system.

## 📄 Source Code

The reconstructed Arduino source code is available here:

[`fingerprint_door_lock.ino`](fingerprint_door_lock.ino)

### Note about the source code

The original project was created in **2021**.

The original Arduino `.ino` project file was no longer available when this repository was created. The source code in this repository was therefore **reconstructed from the Arduino code preserved in the original graduation thesis**.

The reconstruction follows the code and behavior documented in the thesis. Formatting and structural issues caused by the code being preserved inside the PDF were corrected where necessary.

Because the original `.ino` file is no longer available, this reconstructed version should not be considered a byte-for-byte copy of the original 2021 source file.

## 📚 Original Documentation

The complete original graduation thesis is included in this repository:

[`maturski-rad.pdf`](maturski-rad.pdf)

The thesis contains:

- Introduction to electronic locking systems
- RFID and NFC overview
- Arduino UNO overview
- Arduino IDE overview
- SG90 servo motor description
- Optical fingerprint sensor explanation
- Prototype construction
- Wiring diagram
- Operating principle
- Arduino source code preserved from the original project
- Project conclusion

> **Note:** The original thesis is written in Bosnian.

## 🎓 Project Background

This project was completed in **2021** as my high school graduation project in the field of **Computer Engineering and Automation**.

It was one of my early projects combining software development with electronics and physical hardware.

Through the project, I gained practical experience with:

- Arduino and microcontrollers
- C/C++ programming
- Fingerprint authentication
- Biometric sensors
- Servo motor control
- Serial communication
- Electronic circuit assembly
- Hardware prototyping
- Integrating software with a physical system

## 📅 Year

**2021**
