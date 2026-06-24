# Sampling Logic

Version: 1.0

Status: Draft

Last Updated: 2026-06-21

---

# Objective

Define the sampling strategy used for BPSK signal generation.

---

# System Parameters

Carrier Frequency:

50 kHz

Sampling Frequency:

500 kS/s

Bit Rate:

10 kbps

---

# Carrier Period

Tcarrier = 1 / fc

Tcarrier = 20 µs

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

Samples Per Bit = Tbit / Tsample

100 µs / 2 µs

= 50 samples

---

# Carrier Cycles Per Bit

100 µs / 20 µs

= 5 carrier cycles

---

# Signal Generation Sequence

Bit

↓

Phase Selection

↓

Carrier Generation

↓

Sampling

↓

DAC Transmission

---

# Final Decision

Each transmitted bit will contain 50 digital samples.