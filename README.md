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


Here are key sections tailored specifically to highlight this dashboard interface in your repository's **README.md**:

---

## 🖥 System Interface & Feature Overview

The interactive **TWRI Search-and-Rescue Mission Control Dashboard** offers real-time visualization, telemetry tuning, and target analysis:

* **Live Live Plot & Sector Scan:** Displays live target tracking across designated scan zones (e.g., *Room 1*, *Room 2*), showing target locks (*Survivor Alpha*, *Beta*, *Gamma*) along with spatial coordinates.
* **Scan Modes & Control Operations:** Allows real-time toggling between operational modes (**Sector Mode**, **Linear Mode**, **Thermal Mode**, **Deep Mode**) and adjustable scan speeds ($1\times$ to $4\times$).
* **Obstacle & Medium Tuning:** Real-time parameter adjustment for different wall materials (**Drywall**, **Brick**, **Concrete**) to account for material absorption, pulse velocity, and penetration loss.
* **Biometric Life-Signs Analysis:** Monitors target statistics, occupancy status per room, individual confidence scores, estimated depth, and real-time respiratory rate waveforms (BPM).
* **B-Scan Waterfall History & A-Scan Oscilloscope:** Tracks time-integrated signal returns and real-time wave amplitude (Raw, Filtered, and Adaptive Noise Floor) with background clutter suppression.

---

## 📂 System Architecture & Modules

```text
├── Dashboard UI /
│   ├── MissionControl.py       # Main GUI dashboard & control panel
│   ├── RadarPlotter.py         # Sector plot & target position engine
│   └── BiometricTracker.py     # Respiration signal telemetry & target scoring
├── Signal Processing /
│   ├── WaveformGenerator.py    # Gaussian pulse wave propagation & attenuation
│   └── ClutterFilter.py        # Static rejection & adaptive noise filtering
└── README.md

```

---

## 📸 Simulation Screenshots & Demonstration

Add a section to display your simulation visual outputs or feature walkthrough:

```markdown
### Live Radar Mission Control Interface
![TWRI Dashboard Overview](path/to/screenshot_or_gif.gif)
*Figure: Real-time mission control interface performing deep-mode scanning across structural obstacles.*

```

