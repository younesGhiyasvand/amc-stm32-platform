# BPSK Theory

Version: 1.0

Status: Draft

Last Updated: 2026-06-21

---

# Objective

Understand the operating principle of Binary Phase Shift Keying (BPSK).

The goal is to understand how binary information is converted into an analog signal.

---

# Definition

BPSK stands for:

Binary Phase Shift Keying

BPSK is a digital modulation technique that transmits information by changing the phase of a carrier signal.

Only two phases are used.

---

# Bit Mapping

| Bit | Phase |
|-----|-------|
| 0   | 0°    |
| 1   | 180°  |

---

# Carrier Signal

The carrier signal is defined as:

s(t) = A cos(2πfct)

where:

A = amplitude

fc = carrier frequency

t = time

---

# BPSK Signal

For bit 0:

s(t) = A cos(2πfct)

For bit 1:

s(t) = -A cos(2πfct)

The information is carried by phase changes.

Amplitude and carrier frequency remain constant.

---

# Project Parameters

Carrier Frequency:

50 kHz

Initial Bit Rate:

10 kbps

---

# Signal Generation Flow

Bits

↓

BPSK Mapping

↓

Carrier Modulation

↓

Digital Samples

↓

DAC

↓

Analog Signal

---

# Notes

BPSK is the simplest digital modulation technique.

It will be used as the first implementation before BFSK and QPSK.

---

# Final Decision

BPSK will be implemented as the first modulation scheme in the AMC platform.