# System Architecture

Version: 2.0

Status: Approved

Last Updated: 2026-06-21

---

# Objective

Define the overall architecture of the standalone AMC platform.

---

# System Components

The system consists of seven main subsystems:

- User Interface Module
- STM32F401CEU6 Transmitter Board
- TX Analog Board
- Analog Transmission Channel
- RX Analog Board
- STM32F401CEU6 Receiver Board
- PC Processing Unit

---

# Data Path

STM32 TX

↓

TX Analog Board

↓

Analog Transmission Channel

↓

RX Analog Board

↓

STM32 RX

↓

PC Processing Unit

---

# User Control Path

User

↓

Buttons

↓

LCD Interface

↓

Configuration Manager

↓

STM32 TX

---

# PC Responsibilities

- Data acquisition
- Signal visualization
- Dataset generation
- Feature extraction
- Classification
- Prediction
- Performance evaluation

---

# STM32 TX Responsibilities

- User interface management
- Modulation selection
- Signal generation
- DAC data streaming
- Experiment control

---

# STM32 RX Responsibilities

- ADC acquisition
- DMA buffering
- Data transfer to PC

---

# Final Decision

The transmitter board will operate independently using its onboard user interface.

The PC will only perform signal processing and machine learning tasks.