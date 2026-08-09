# ❤️ Analog ECG Monitor

**Team Technonigs**
Department of Electronic and Telecommunication Engineering, University of Moratuwa
Module: **EN2091 — Laboratory Practice and Projects**

A fully functional analog front end (AFE) for an electrocardiogram (ECG) monitor, designed and developed using exclusively analog electronics for signal acquisition, amplification, and filtering. The device captures cardiac electrical activity through three electrodes and outputs a clean ECG waveform for real-time monitoring — no microcontroller, no DSP, purely analog signal chain design.

---

## 🔬 Overview

This project demonstrates the design and implementation of a 3-lead ECG monitoring system built entirely with analog components. The device safely extracts weak bioelectric signals from the human body, amplifies them, and filters noise to produce a diagnostic-quality ECG waveform suitable for cardiac monitoring.

### Key Specifications

| Parameter | Value |
|---|---|
| Signal Range | [e.g., 10 μV – 5 mV input amplitude] |
| Frequency Range | [e.g., 0.5 Hz – 100 Hz (cardiac signal bandwidth)] |
| Electrode Configuration | [e.g., 3-lead setup (LA, RA, RL) following Einthoven's Triangle] |
| Power Supply | [e.g., Dual 7.4 V Li-Ion battery, isolated from mains for patient safety] |
| Output | [e.g., Analog signal for oscilloscope display] |

---

## ✨ Features

- **High-Precision Instrumentation Amplifier** — [e.g., OP07-based] differential amplifier with adjustable gain and high CMRR.
- **Multi-Stage Filtering:**
  - **High-Pass Filter** — [e.g., 2nd Order Butterworth (0.5 Hz cutoff)] to remove baseline wander.
  - **Low-Pass Filter** — [e.g., 4th Order Butterworth (100 Hz cutoff)] to eliminate high-frequency noise.
  - **Notch Filter** — [e.g., Wien-Robinson (50 Hz / 60 Hz)] to suppress powerline interference.
- **Right Leg Drive (RLD) Circuit** — Active common-mode rejection for enhanced noise immunity.
- **Safety-First Design** — Battery-powered operation ensures patient isolation and safety.
- **Custom PCB** — Professional layout optimized for low-noise analog signal processing.
- **Custom Enclosure** — Ergonomic, portable design with proper electrode connections.

### Signal Processing Chain

1. **Instrumentation Amplifier** — Extracts differential voltage between LA and RA electrodes with variable gain.
2. **High-Pass Filter** — Removes DC offset and baseline wander.
3. **Low-Pass Filter** — Eliminates muscle artifacts and high-frequency interference.
4. **Notch Filter** — Attenuates powerline noise.
5. **Right Leg Drive** — Inverts and feeds back common-mode signal for active noise cancellation.

---

## 🔨 Hardware Implementation

### PCB Design

- **Software:** [e.g., KiCad / EasyEDA / Altium]
- **Component Type:** [e.g., Through-hole / SMD] for cost-effectiveness and ease of assembly.
- **Layout:** [e.g., 2-Layer], optimized for minimal noise coupling and proper analog grounding.

### Enclosure

- **Manufacturing:** [e.g., 3D printed PLA/PETG]
- **Design:** Custom enclosure with cutouts for:
  - Output probes
  - Power switch
  - ECG lead connectors
  - Potentiometer access for gain adjustment

---

## 📊 Testing Results

### Breadboard Prototype

- [ ] Successfully captured function generator ECG signals
- [ ] Verified with real human ECG signals
- [ ] Clean waveform with identifiable P, QRS, and T waves

### Final PCB Device

- [ ] Improved signal quality over breadboard implementation
- [ ] Reduced noise and interference
- [ ] Portable and user-friendly operation

---

## 📁 Repository Structure

```text
├── schematics/          # Circuit diagrams and design files
├── simulations/         # LTspice/Proteus simulation files and results
├── pcb_design/           # KiCAD/Altium files, Gerber files, BoM
├── enclosure_design/     # 3D CAD models (.STL, .STEP files)
├── documentation/        # Project report, datasheets, calculations
├── testing/              # Test results, oscilloscope data
└── README.md             # This file
```

---

## 👥 Team Technonigs

| Index No. | Name |
|---|---|
| [240657J] | [Thennakoon U.I.D] |
| [240518K] | [Pitiduwa S.M.] |
| [240695X] | [Wanninayaka W.M.I.R] |
| [240054H] | [Bandara A.H.M.H.N.] |

---

## 🎓 Academic Context

This project was developed as part of **EN2091 — Laboratory Practice and Projects**, offered by the **Department of Electronic and Telecommunication Engineering, University of Moratuwa**.

---

## 📜 License

[e.g., MIT License — see LICENSE file for details]
