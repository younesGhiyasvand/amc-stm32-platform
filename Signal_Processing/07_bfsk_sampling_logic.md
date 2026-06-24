# BFSK Sampling Logic

Version: 1.0

Status: Draft

Last Updated: 2026-06-21

---

# Objective

Define the sampling strategy used for BFSK signal generation.

---

# System Parameters

Low Frequency:

40 kHz

High Frequency:

60 kHz

Sampling Frequency:

500 kS/s

Bit Rate:

10 kbps

---

# Sampling Period

Tsample = 1 / fs

Tsample = 2 µs

---

# Bit Duration

Tbit = 1 / Bit Rate

Tbit = 100 µs

---

# Samples Per Bit

100 µs / 2 µs

= 50 samples

---

# Carrier Cycles Per Bit

For 40 kHz:

100 µs / 25 µs

= 4 cycles

For 60 kHz:

100 µs / 16.67 µs

≈ 6 cycles

---

# Signal Generation Sequence

Bit

↓

Frequency Selection

↓

Sample Generation

↓

DAC Transmission

---

# Final Decision

Each transmitted bit will contain 50 digital samples.