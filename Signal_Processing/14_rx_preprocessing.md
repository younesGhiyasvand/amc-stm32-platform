# RX Preprocessing

Version: 1.0

Status: Draft

Last Updated: 2026-06-25

---

# Objective

Define preprocessing operations executed on STM32 RX before transferring data to the PC.

---

# Processing Stages

ADC Samples

↓

DC Offset Removal

↓

Normalization

↓

Buffering

↓

PC Transfer

---

# DC Offset Removal

Purpose:

Remove ADC baseline offset.

Benefits:

- Improved signal quality
- Better feature extraction

---

# Normalization

Purpose:

Scale samples to a common range.

Benefits:

- Consistent dataset generation
- Improved classifier performance

---

# Buffering

DMA buffers are used for continuous acquisition.

Benefits:

- Reduced CPU load
- Reliable sampling

---

# Notes

Only lightweight preprocessing operations are performed on STM32 RX.

Computationally intensive algorithms are executed on the PC.

---

# Final Decision

STM32 RX performs basic preprocessing before data transfer.