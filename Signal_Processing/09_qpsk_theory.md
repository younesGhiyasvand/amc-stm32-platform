# QPSK Theory

Version: 1.0

Status: Draft

Last Updated: 2026-06-21

---

# Objective

Understand the operating principle of Quadrature Phase Shift Keying (QPSK).

The goal is to understand how two bits are transmitted using a single symbol.

---

# Definition

QPSK stands for:

Quadrature Phase Shift Keying

QPSK is a digital modulation technique that transmits information by changing the phase of the carrier signal.

Four different phases are used.

---

# Bit Mapping

| Bits | Phase |
|------|-------|
| 00   | 45°   |
| 01   | 135°  |
| 11   | 225°  |
| 10   | 315°  |

---

# Symbol Representation

Each symbol carries:

2 bits

---

# Characteristics

Constant amplitude

Constant carrier frequency

Variable phase

---

# Project Parameters

Carrier Frequency:

50 kHz

Bit Rate:

10 kbps

Sampling Frequency:

500 kS/s

---

# Signal Generation Flow

Bits

↓

Symbol Mapper

↓

I/Q Generator

↓

Sample Generator

↓

DAC

↓

Analog Signal

---

# Notes

QPSK doubles the amount of information transmitted compared to BPSK.

---

# Final Decision

QPSK will be implemented as the third modulation scheme in the AMC platform.