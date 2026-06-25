# Feature Extraction

Version: 1.0

Status: Draft

Last Updated: 2026-06-25

---

# Objective

Extract meaningful signal characteristics for classification.

---

# Input

- Raw Samples
- I/Q Samples

---

# Time-Domain Features

- Mean
- Variance
- RMS
- Signal Energy

---

# Frequency-Domain Features

- FFT
- Power Spectral Density (PSD)
- Peak Frequency

---

# Phase Features

- Instantaneous Phase
- Phase Variance

---

# Output

Feature Vector

Example:

[Energy, Variance, Peak Frequency, Phase Variance]

---

# Notes

Feature extraction is executed on the PC.

---

# Final Decision

Feature vectors will be used as inputs to machine learning models.