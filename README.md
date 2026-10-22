# PLC-Based Sequential Control of Three Mixing Devices Using Timers

## Project Overview

This project demonstrates a PLC-based sequential control system for three mixing devices using ladder logic and timer instructions.

The system starts the mixers at predefined intervals and switches all outputs OFF when the stop condition is activated.

## Objectives

- Understand PLC-based industrial automation.
- Develop ladder logic for sequential control.
- Configure timers for different starting delays.
- Control three mixing device outputs.
- Implement a common stop and reset operation.

## Operating Sequence

| Device | PLC Output | Delay from Process Start |
|---|---|---:|
| Mixer A | Y0 | 7 seconds |
| Mixer B | Y1 | 10.6 seconds |
| Mixer C | Y2 | 15.6 seconds |

Mixer B starts 3.6 seconds after Mixer A, and Mixer C starts 5 seconds after Mixer B.

## PLC Input/Output Assignment

| Address | Function |
|---|---|
| X0 | Process Start |
| X1 | Process Stop |
| M0 | Sequence Enable |
| T0 | Timer for Mixer A |
| T1 | Timer for Mixer B |
| T2 | Timer for Mixer C |
| Y0 | Mixer A |
| Y1 | Mixer B |
| Y2 | Mixer C |

## Hardware and Software

- PLC: Mitsubishi FX5U or an equivalent PLC
- PLC programming software compatible with the selected controller
- Start and Stop push buttons
- Three mixing devices or simulated outputs
- Suitable contactors, motor protection, and power supply for hardware implementation

## Project Files

- `report/` — Project documentation
- `ladder-diagram/` — Ladder logic diagram
- `diagrams/` — Block diagram and flow diagram
- `screenshots/` — PLC programming and simulation screenshots
- `docs/` — Tag database and supporting documentation

## Applications

- Industrial mixing systems
- Food processing
- Chemical processing
- Batch processing
- Industrial automation education

## Future Scope

- HMI integration
- Sensor-based control
- Adjustable timer settings
- Fault detection and alarms
- SCADA monitoring
- Data logging

## Verification Note

The stated timing sequence describes the intended operation. Actual timing, timer presets, stop/reset behavior, and output operation must be verified using the selected PLC and its programming software before hardware implementation.

## Author

Kaushik Mali  
Electronics and Computer Science  
St. John College of Engineering & Management
