# High-Voltage Op-Amp PCB & Red Pitaya Feedback System

**Role:** Undergraduate Research Assistant | Space-time Optics and Photonics Lab (UCF)

This repository contains the hardware design, fabrication files, and signal manipulation logic for a custom 2-layer high-voltage amplifier PCB and real-time feedback system used in a particle levitation experiment.

## ⚡ Power & Hardware Design Highlights
*   **Voltage Amplification:** Designed an op-amp circuit to step a 1V FPGA signal up to 10V to successfully drive a piezoelectric device.
*   **Power Delivery & Stability:** Integrated bulk capacitors into the PCB layout to stabilize the 15V power supplies during high-frequency operation.
*   **Validation:** Verified a 1 MHz bandwidth using an oscilloscope and validated I/O with signal generators.
*   **Real-Time Feedback:** Implemented quadrant position sensing and low-pass filtering on a Red Pitaya STEMlab 125-14 (Zynq Z-7010).

## 🗂️ Repository Structure

*   **`/OpAMP`**: Contains the complete KiCad project files (`.kicad_pcb`, `.kicad_sch`, `.kicad_pro`) for the 2-layer board.
    *   **`/gerber - OpAMP`**: Complete fabrication packet, including copper layers (`_Cu.gbr`), masks (`_Mask.gbr`), silkscreen, and drill files (`.drl`) ready for manufacturing[cite: 7].
    *   **`/OpAMP LTspice`**: Contains the theoretical circuit simulation files (`Draft3.asc`) and transient analysis data.
*   **`/Test 1 (Signal Manipulation)`**: Contains the low-pass filter logic and signal amplifier testing parameters[cite: 3].
