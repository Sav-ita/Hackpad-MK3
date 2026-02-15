# Hackpad MK2

This repository contains all files for the **Hackpad MK2** project, a custom 9-key macro pad designed for productivity and customization.

It features:
- 3x3 mechanical keys (9 total)
- 0.91" OLED display (SSD1306)
- Powered by an RP2040 microcontroller (compatible with CircuitPython)

---

## 📸 Hackpad Overview

The Hackpad MK2 is designed with a sleek and compact form factor, perfect for desktop shortcuts and macros.

<img src="Images/1.png" alt="Hackpad Overview" width="600">

---

## 🔌 Schematic
![Schematic Screenshot](Images/4.png) 

The schematic, designed in KiCad, shows the wiring for the 9 independent keys and the I2C OLED display. Each key is connected to a dedicated GPIO on the RP2040, and the OLED follows the GND-VCC-SCL-SDA pinout.

---

## 🖥️ PCB Layout
The PCB was designed focusing on a clean layout and easy assembly. It includes custom silkscreen labeling and broad copper traces for reliability.

<img src="Images/5.png" alt="PCB Layout" width="500">

---

## 🧩 Case Design

The case consists of two main parts: the base and the top cover, designed to be 3D printed and fit perfectly with the PCB.

<img src="Images/2.png" alt="Case Base" width="400">
<img src="Images/3.png" alt="Case Cover" width="400">

---

## 📦 Bill of Materials (BOM)
List of all components used in this project:

| Part | Quantity | Description | 
|------|----------|-------------|
| Mechanical Key Switches | 9 | MX-style switches |
| Keycaps | 9 | Compatible with MX switches | 
| RP2040 Microcontroller | 1 | e.g., Seeed XIAO RP2040 | 
| OLED Display 0.91" | 1 | 128x32 I2C interface | 
| Custom PCB | 1 | Hackpad MK2 Design | 
| 3D Printed Case | 1 | Base + Cover | 

---

## Firmware Instructions

1. Download and install the latest **CircuitPython** .uf2 for your board.
2. Connect the RP2040 via USB and copy the firmware files.
3. Ensure the following libraries are in the `lib` folder:
   - `adafruit_display_text`
   - `adafruit_ssd1306`
   - `adafruit_hid`
4. Copy `main.py` (or rename to `code.py`) to the device.

## 📝 License
This project is open-source and created by **Saverio Martino**.
