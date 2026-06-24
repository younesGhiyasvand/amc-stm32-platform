# BFSK Representation

Version: 1.0

Status: Draft

Last Updated: 2026-06-21

---

# Objective

Define the internal representation used for BFSK.

---

# Principle

BFSK carries information using frequency changes.

No phase manipulation is required.

---

# Bit Mapping

| Bit | Frequency |
|-----|-----------|
| 0   | 40 kHz    |
| 1   | 60 kHz    |

---

# Example

Input:

10110010

Output:

60kHz

40kHz

60kHz

60kHz

40kHz

40kHz

60kHz

40kHz

---

# I/Q Discussion

BFSK is not generated using I/Q components.

However, I/Q information can later be extracted at the receiver side for dataset generation and machine learning purposes.

---

# Notes

BFSK generation is frequency-based.

I/Q extraction belongs to the signal processing stage.

---

# Final Decision

No I/Q generator will be used in the BFSK transmitter implementation.