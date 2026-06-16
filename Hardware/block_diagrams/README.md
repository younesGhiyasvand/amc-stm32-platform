# Block Diagrams

This directory contains the engineering block diagrams of the Automatic Modulation Classification (AMC) system.

These diagrams serve as the architectural reference of the project and will be used during hardware design, firmware development, signal processing implementation and system documentation.

Each diagram is stored in two formats:

- `.drawio` : Editable source file
- `.svg` : Exported vector graphic for reports, presentations and documentation

---

## Diagram List

### 01_system_overview

High-level representation of the complete AMC system architecture, including power distribution, transmitter, receiver and PC processing unit.

---

### 02_tx_subsystem

Internal architecture of the STM32-based transmitter.

Functions:

- Configuration management
- Bit generation
- Digital modulation
- I/Q generation
- Carrier generation
- Digital-to-Analog conversion
- Signal filtering

---

### 03_channel

Analog transmission channel between transmitter and receiver.

The first implementation uses a wired channel to ensure stable and repeatable experiments.

---

### 04_rx_subsystem

Internal architecture of the STM32-based receiver.

Functions:

- Signal acquisition
- Anti-alias filtering
- Analog-to-Digital conversion
- DMA transfer
- Circular buffering
- Data transmission to the PC

---

### 05_pc_processing

Signal processing and machine learning pipeline executed on the PC.

Functions:

- Data acquisition
- Preprocessing
- Dataset generation
- Feature extraction
- Classification
- Prediction

---

### 06_complete_system

Complete end-to-end architecture of the project.

This diagram combines all subsystems and represents the reference architecture of the entire AMC platform.

It includes:

- STM32 transmitter
- Analog transmission channel
- STM32 receiver
- PC processing pipeline
- User application
- Control interface

---

## Architecture Baseline

The `06_complete_system` diagram is considered the Architecture Baseline (v1.0) of the project.

Any future modification of the system architecture must be reflected in this diagram before implementation.
