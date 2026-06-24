# BFSK Theory

Version: 1.0

Status: Draft

Last Updated: 2026-06-21

---

# Objective

Understand the operating principle of Binary Frequency Shift Keying (BFSK).

The goal is to understand how binary information is converted into an analog signal by changing the carrier frequency.

---

# Definition

BFSK stands for:

Binary Frequency Shift Keying

BFSK is a digital modulation technique that transmits information by changing the carrier frequency.

Only two frequencies are used.

---

# Bit Mapping

| Bit | Frequency |
|-----|-----------|
| 0   | 40 kHz    |
| 1   | 60 kHz    |

---

# Carrier Signals

For bit 0:

s(t) = A cos(2π × 40k × t)

For bit 1:

s(t) = A cos(2π × 60k × t)

---

# Characteristics

Constant amplitude

Constant phase

Variable frequency

---

# Project Parameters

Low Frequency:

40 kHz

High Frequency:

60 kHz

Bit Rate:

10 kbps

Sampling Frequency:

500 kS/s

---

# Signal Generation Flow

Bits

↓

Frequency Selection

↓

Sample Generation

↓

DAC

↓

Analog Signal

---

# Notes

BFSK does not require an I/Q generator.

The transmitted information is carried by frequency changes.

---

# Final Decision

BFSK will be implemented as the second modulation scheme in the AMC platform.