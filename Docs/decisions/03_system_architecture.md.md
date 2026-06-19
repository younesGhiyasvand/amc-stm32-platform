# System Architecture

Version: 1.1

Status: Approved

Last Updated: 2026-06-18

---

# Objective

Define the overall architecture of the AMC platform.

---

# System Components

The system consists of six main subsystems:

- Power System
- STM32F401CEU6 Board A (Transmitter)
- Custom Interface Board
- Analog Transmission Channel
- STM32F401CEU6 Board B (Receiver)
- PC Processing Unit

---

# Data Path

STM32 TX

↓

External DAC

↓

Reconstruction Filter

↓

Analog Transmission Channel

↓

Anti-Aliasing Filter

↓

External ADC

↓

STM32 RX

↓

PC Processing Unit

---

# Control Path

User Application

↓

Control Interface (USB CDC)

↓

Configuration Manager

↓

STM32 Firmware

---

# PC Responsibilities

- Data acquisition
- Signal visualization
- Preprocessing
- Dataset generation
- Feature extraction
- Classification
- Prediction
- Performance evaluation

---

# STM32 Responsibilities

## Transmitter Board

- Modulated signal generation
- DAC data streaming
- Timing control
- Communication with PC

## Receiver Board

- ADC data acquisition
- Data buffering using DMA
- Communication with PC
- Experiment control

---

# Interface Board Responsibilities

- Digital-to-Analog Conversion (DAC)
- Analog-to-Digital Conversion (ADC)
- Signal conditioning
- Reconstruction filtering
- Anti-aliasing filtering
- Analog signal routing

---

# Final Decision

Real-time signal generation and acquisition will be handled by the STM32-based hardware platform.

Signal processing, dataset generation, feature extraction, and machine learning tasks will be executed on the PC.