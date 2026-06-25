# RX Data Acquisition

Version: 1.0

Status: Draft

Last Updated: 2026-06-25

---

# Objective

Define the signal acquisition process performed by the receiver hardware.

---

# Signal Flow

Analog Signal

↓

RX Board

↓

ADC

↓

STM32 RX

↓

PC

---

# ADC Responsibilities

- Analog-to-Digital Conversion
- Signal Sampling
- Digital Sample Generation

---

# STM32 RX Responsibilities

- DMA Data Acquisition
- Sample Buffering
- Packet Formation
- Communication with PC

---

# Sampling Parameters

Sampling Frequency:

500 kS/s

ADC Resolution:

To Be Determined

---

# Output Data

The receiver produces raw digital samples.

Example:

1205

1432

1788

2101

1940

...

---

# Notes

The receiver does not perform modulation classification.

Its primary purpose is reliable signal acquisition.

---

# Final Decision

STM32 RX will acquire and transfer sampled data to the PC.