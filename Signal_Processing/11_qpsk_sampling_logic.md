# QPSK Sampling Logic

Version: 1.0

Status: Draft

Last Updated: 2026-06-21

---

# Objective

Define the sampling strategy used for QPSK signal generation.

---

# System Parameters

Carrier Frequency:

50 kHz

Sampling Frequency:

500 kS/s

Bit Rate:

10 kbps

---

# Symbol Rate

Each symbol contains:

2 bits

Symbol Rate:

5000 symbols/s

---

# Sampling Period

Tsample = 1 / fs

Tsample = 2 µs

---

# Symbol Duration

Tsymbol = 1 / 5000

Tsymbol = 200 µs

---

# Samples Per Symbol

200 µs / 2 µs

= 100 samples

---

# Carrier Cycles Per Symbol

200 µs / 20 µs

= 10 cycles

---

# Signal Generation Sequence

2 Bits

↓

I/Q Selection

↓

Sample Generation

↓

DAC Transmission

---

# Final Decision

Each transmitted symbol will contain 100 digital samples.