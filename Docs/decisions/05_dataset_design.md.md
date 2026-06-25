# Dataset Design

Version: 1.0

Status: Approved

Last Updated: 2026-06-25

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

# Dataset Strategy

Two datasets will be used.

## Standard Dataset

A publicly available AMC dataset will be used for model development and benchmarking.

Examples:

- RadioML XXXX.XX
- RadioML XXXX.XX
- RadioML XXXX.XX

Applications:

- Model training
- Performance comparison
- Baseline evaluation

---

## Hardware Dataset

A custom dataset will be generated using the developed AMC hardware platform.

Applications:

- Real-world validation
- Hardware verification
- Performance evaluation under practical conditions

---

# Final Decision

Model development will be performed using a standard AMC dataset.

The hardware-generated dataset will be used for validation and comparison.

---

# Final Decision

The dataset will be generated from physical experiments instead of simulations.