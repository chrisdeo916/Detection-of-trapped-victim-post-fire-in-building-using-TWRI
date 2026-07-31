# Detection-of-trapped-victim-post-fire-in-building-using-TWRI
# Through-the-Wall Radar Imaging (TWRI) - Victim Detection Prototype

![Project Status](https://img.shields.io/badge/Status-Completed-success)
![Platform](https://img.shields.io/badge/Platform-Arduino%20%7C%20Python%20%7C%20Processing-blue)
![Academic Year](https://img.shields.io/badge/Academic%20Year-2025%2F2026-orange)

## 📌 Overview
This repository contains the software, firmware, and simulation models for a low-cost **Through-the-Wall Radar Imaging (TWRI)** prototype designed for post-fire disaster search and rescue operations. The system models time-of-flight wave interactions in Python, controls a motorized sweeping transducer assembly via an **Arduino Uno**, and renders real-time distance-profile graphs on a **Processing IDE** canvas.

---

## 🛠 Tech Stack & Tools
* **Hardware:** Arduino Uno (ATmega328P), HC-SR04 Ultrasonic Sensor, SG90 Servo Motor, Piezo Buzzer, Status/Alert LEDs.
* **Firmware:** Embedded C++ (Arduino Core).
* **Simulation:** Python 3.x (`numpy`, `matplotlib`, `scipy`).
* **Visualization:** Processing IDE v4.x (`processing.serial.*`).

---

## 📂 Repository Structure

```text
├── Firmware/
│   └── twri_radar_scanner.ino      # Arduino C++ script (Servo sweep & echo sensor capture)
├── Simulation/
│   └── twri_signal_sim.py          # Python script (Waveform simulation & clutter filtering)
├── Visualization/
│   └── twri_radar_canvas.pde       # Processing sketch (Real-time graphical radar canvas)
├── Schematics/
│   └── circuit_diagram.png         # Hardware pin connections & breadboard wiring layout
└── README.md                       # Documentation and usage guide
