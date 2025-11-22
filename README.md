# E-Bike Passive Cell Balancer (4S Prototype)

## Overview
Prototype passive cell balancer for a 4S e-bike battery. The Arduino reads each cell voltage (via voltage dividers) and activates bleed MOSFETs to lower over-voltage cells, helping equalize the pack and protect against imbalance.

## Features
- Monitors 4 series cell voltages in real time
- Enables bleed MOSFETs when a cell exceeds the target voltage
- Hysteresis-based control to prevent chatter
- Simple, low-cost balancing suitable for lab/testing

## Hardware Required
- Arduino UNO (or compatible)
- Voltage divider network for each cell tap (ensure proper isolation and safety)
- N-channel MOSFETs or P-MOSFETs with gate driver for bleed resistors
- Bleed resistors (power-rated)
- Safe connections and isolation for battery testing

## Notes & Safety
- This is a **prototype**. Real BMS designs require isolation, cell balancing ICs, temperature monitoring, and high-voltage safety.
- Do not test with high-capacity packs without proper fusing and safety equipment.
- Calibrate `scaleFactor` and divider resistors for your exact hardware.

---

👨‍💻 **Author:** K. Viswanadh
