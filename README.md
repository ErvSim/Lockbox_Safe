# Lockbox Safe (In Progress)

This is an in-progress smart lockbox project using the Raspberry Pi Pico, a fingerprint scanner, an OLED display, and a servo motor to control access. The project is designed for security applications where access is granted only upon fingerprint approval.

## Overview

- A fingerprint scanner is used to verify a user's identity.
- If the fingerprint is **approved**, the OLED displays **"Approved"**, and the servo rotates to unlock the 3D-printed lock.
- If the fingerprint is **not approved**, the OLED displays **"Not Approved, Try Again"**, and the servo remains inactive.
- The entire system is powered via micro-USB and designed to activate only after power is plugged in, adding a simple hardware safeguard.
- Once the lid is closed, another fingerprint scan is required to **lock** the box.

This repository is currently under development. More updates will follow as the physical components (3D printer, servo integration) are added and tested.

## Schematic

The following schematic shows the flow of data between the Raspberry Pi Pico, fingerprint sensor, OLED display, and servo motor:

[schematic/lockbox_schematic.png](https://github.com/ErvSim/Lockbox_Safe/blob/main/schematic/Lockbox.png)

You can also open and explore the project logic using the Logisim file:

- [Download Lockbox.circ](schematic/Lockbox.circ)

## In Progress Features

- [x] Logisim schematic created
- [x] OLED & fingerprint scanner integrated logically
- [ ] Fingerprint validation code
- [ ] Servo lock control
- [ ] 3D-printed lockbox structure
- [ ] Final integration and testing

## Tools & Components

- Raspberry Pi Pico
- UART Fingerprint Scanner
- 0.96" I2C OLED Display (SSD1306)
- SG90 Micro Servo  
- Logisim Evolution for schematic design

---

**Status:** 🚧 Work in Progress  

