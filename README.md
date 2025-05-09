# BioScan‑AD5941 Two‑Layer PCB Module

A compact, high‑precision bioimpedance front‑end PCB based on the Analog Devices AD5941—designed as a two‑layer board for low‑cost fabrication.

---

## 📋 Table of Contents

1. [Project Purpose](#project-purpose)  
2. [Features & Functionality](#features--functionality)  
3. [Technologies Used](#technologies-used)  
4. [Installation Instructions](#installation-instructions)  
5. [Usage Examples](#usage-examples)  
6. [Dependencies](#dependencies)  
7. [System Requirements](#system-requirements)  
8. [Project Structure](#project-structure)  
9. [License](#license)  

---

## 🎯 Project Purpose

The **BioScan‑AD5941 Two‑Layer PCB** is a mixed‑signal board that implements the AD5941 bioimpedance AFE in a two‑layer form factor. It provides precise impedance sensing, simple electrode hookups, and SPI connectivity—optimized for low‑cost fabrication at JLCPCB or similar services.

---

## 🌟 Features & Functionality

- **Two‑Layer Stackup**  
  - Top: components & signal routing  
  - Bottom: ground pour & power  
- **Bioimpedance Calibration**  
  - On‑board 1 kΩ precision resistor between RCAL0/RCAL1  
- **Electrode Interface**  
  - 4‑pin screw terminal block for excitation (+/–) and sensing (+/–)  
- **SPI Connector**  
  - 6‑pin shrouded header: 3.3 V, GND, MOSI, MISO, SCLK, CS  
- **Local Decoupling**  
  - 0.1 µF + 1 µF per supply/reference pin, placed within 1 mm  
- **Exposed‑Pad Thermal Via**  
  - Under QFN for AGND thermal‑ground connection  
- **DFM‑Friendly**  
  - ≥ 6 mil trace/space, 0.3 mm vias, 0402/0603 passives  

---

## 🛠 Technologies Used

- **CAD Software:** Altium Designer  
- **Fabrication:** JLCPCB two‑layer FR‑4, 1 oz copper, 0.6 mm thickness  
- **Key IC:** AD5941BCPZ (Analog Devices)  
- **Connectors:** 4‑pin screw terminal, 6‑pin 2.54 mm header  
- **Passives:** Standard 0402/0603 capacitors & resistors  

---

## ⚙️ Installation Instructions

1. **Export Outputs**  
   - In Altium:  
     - **File → Fabrication Outputs → Gerber X2**  
     - **File → Reports → Bill of Materials**  
2. **Order PCBs**  
   - Upload Gerbers to JLCPCB  
   - Select two‑layer FR‑4, 1 oz copper, 0.6 mm board thickness  
   - Set min. track/space = 6 mil, via drill = 0.3 mm  
3. **Assembly**  
   - Solder SMD parts via reflow or hot‑air  
   - Hand‑solder screw terminals & headers  
4. **Power‑Up**  
   - Apply 3.3 V to VIN pin or via USB‑to‑3.3 V adapter  
   - Verify stable AVDD/DVDD and reference voltages at test points  

---

💻 System Requirements
Development Machine: Windows or Linux with Altium Designer v20+

Fabrication Constraints:

6 mil min. trace/space

0.3 mm via drill

0402/0603 SMD compatible

Assembly Tools: Reflow oven or hot‑air station, solder paste, microscope (for QFN)


GNU GENERAL PUBLIC LICENSE
Version 3, 29 June 2007

Copyright (C) 2025 [Your Name]

This PCB design is free software: you can redistribute it and/or modify it
under the terms of the GNU General Public License as published by the Free
Software Foundation, either version 3 of the License, or (at your option)
any later version, **with the following additional restriction**:

1. Commercial use of this PCB design is prohibited without the express
   written consent of the author.

This design is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this design. If not, see <https://www.gnu.org/licenses/>.

Author Contact: your.email@example.com
