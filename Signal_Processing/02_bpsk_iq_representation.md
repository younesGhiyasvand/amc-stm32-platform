# I/Q Representation

Version: 1.0

Status: Draft

Last Updated: 2026-06-21

---

# Objective

Understand I/Q representation and its relationship with BPSK.

---

# Definition

Any modulated signal can be represented using two orthogonal components:

- In-Phase (I)
- Quadrature (Q)

The general equation is:

s(t) = I(t)cos(2πfct) - Q(t)sin(2πfct)

---

# BPSK Representation

For BPSK:

Q = 0

Only the I component changes.

---

# Bit Mapping

| Bit | I  | Q |
|-----|----|---|
| 0   | +1 | 0 |
| 1   | -1 | 0 |

---

# Signal Equation

For BPSK:

s(t) = I(t)cos(2πfct)

---

# Constellation Diagram

BPSK uses only one axis.

(-1) -------- (0) -------- (+1)

The signal moves only along the I axis.

---

# Why Use I/Q?

Advantages:

- Simplifies modulation algorithms
- Simplifies classification
- Standard representation in communication systems

---

# Final Decision

The AMC platform will internally represent all modulation schemes using I/Q notation.