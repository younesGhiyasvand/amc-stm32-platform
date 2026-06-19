# Dataset Design

Version: 1.0

Status: Approved

Last Updated: 2026-06-17

---

# Objective

Define the dataset generation strategy.

---

# Dataset Source

Real-world transmitted signals.

---

# Stored Information

Each sample will contain:

- Modulation type
- Carrier frequency
- Sampling frequency
- SNR
- Timestamp
- Raw I/Q samples

---

# Storage Format

CSV

NumPy

MAT files

---

#Hardware Metadata

- ADC model
- ADC resolution
- ADC sampling rate

- DAC model
- DAC resolution
- DAC update rate

- Interface board revision

---

# Final Decision

The dataset will be generated from physical experiments instead of simulations.