# I/Q Recovery

Version: 1.0

Status: Draft

Last Updated: 2026-06-25

---

# Objective

Recover I and Q components from received signals.

---

# Purpose

Many modulation classification techniques rely on I/Q data.

Recovered I/Q samples provide a standard signal representation.

---

# Signal Flow

Raw Samples

↓

Carrier Recovery

↓

I/Q Extraction

↓

I/Q Samples

---

# Output Format

I Samples:

0.82

0.91

0.65

...

Q Samples:

-0.12

0.08

0.24

...

---

# Applications

- Dataset generation
- Constellation diagrams
- Feature extraction
- Classification

---

# Notes

I/Q recovery is executed on the PC.

---

# Final Decision

Recovered I/Q samples will be used as the primary signal representation for machine learning tasks.