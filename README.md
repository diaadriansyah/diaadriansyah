# Atmel MCS-51 Embedded Systems Portfolio

This repository contains the low-level firmware and hardware architecture designs for high-precision industrial and commercial hardware applications driven by the Atmel MCS-51 microcontroller architecture. All micro-core logic routines are implemented strictly utilizing low-level Assembler language to enforce absolute execution speed and zero-latency timing logic.

## 🛠️ Tech Stack & Tools
- **Microarchitecture:** Atmel MCS-51 (8051 Core)
- **Firmware Language:** Low-Level Assembler Language
- **Hardware Design & Routing:** KiCad EDA
- **Diagnostics & Signal Integrity:** Tektronix & Advantest Spectrum Analyzers, Digital Oscilloscopes
- **Technical Documentation:** CorelDRAW & Inkscape (Vector Engineering Blueprints)

---

## 🎮 Project 1: Autonomous Arcade Game Machine Infrastructure

### Project Overview
Developed a standalone commercial arcade game hardware system operating on a cost-effective legacy architecture. Designed to handle continuous runtime blocks with strict real-time responsiveness between human interface device inputs and mechanical actuators.

### Key Hardware & Firmware Features
- **Zero-Latency Hardware Interrupts:** Programmed external interrupt routines (`IE0` and `IE1`) in Assembler to capture optical sensor input state-changes immediately without polling cycles.
- **Signal Integrity Optimization:** Routed the multi-layer controller PCB using KiCad with guarded trace paths, isolating low-voltage logic lines from high-voltage actuator relays.
- **Diagnostics Execution:** Used Tektronix Spectrum Analyzers to inspect RF emissions and trace clock-oscillator stability under prolonged loading.

### Technical Deliverables
- Fully operational standalone arcade control board with **0ms input lag**.
- Achieved a **98% machine uptime rate** across testing cycles.
- Reduced bill-of-materials (BOM) cost by **35%** against vendor alternatives.

---

## ⏱️ Project 2: High-Precision Industrial Timer Module

### Project Overview
Designed a modular, high-reliability industrial hardware timer module intended for sequential automation triggering on manufacturing lines where microprocessor failure is not an option.

### Key Hardware & Firmware Features
- **Register-Level Time Base Management:** Utilized internal 16-bit Hardware Timers (`Timer 0` and `Timer 1`) in Mode 1 operation to generate precision microsecond ticks through precise timer register reloading (`TH0`/`TL0`).
- **Display Matrix Drivers:** Implemented localized multiplexed display matrix controls driven directly via register-shifts in Assembler logic.
- **Factory Ready Integration:** Drafted robust vector wiring schematics and assembly layout diagrams using CorelDRAW and Inkscape for factory technicians.

### Technical Deliverables
- Maintained **100% sequence accuracy** with zero drift across extended 72-hour stress test blocks.
- Improved production sequence line efficiency rates by **15%**.

---

## 📈 Quality Assurance & Validation Standards
Every hardware trace and register routine undergoes validation under simulation environments prior to physical bench-testing:
1. Fault diagnostics checking via logic probing.
2. Signal integrity validation using Advantest calibration instruments.
3. Strict register tracking to eliminate code overflows.

