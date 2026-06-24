# QPSK I/Q Representation

Version: 1.0

Status: Draft

Last Updated: 2026-06-21

---

# Objective

Define the I/Q representation used by QPSK.

---

# Principle

QPSK uses two orthogonal components:

- In-Phase (I)
- Quadrature (Q)

---

# Bit Mapping

| Bits | I  | Q  |
|------|----|----|
| 00   | +1 | +1 |
| 01   | -1 | +1 |
| 11   | -1 | -1 |
| 10   | +1 | -1 |

---

# Signal Equation

s(t) = I(t)cos(2πfct) - Q(t)sin(2πfct)

---

# Constellation Diagram

          Q

          ↑

   01     |     00

          |

----------+----------→ I

          |

   11     |     10

          |

---

# Advantages

- Higher spectral efficiency

- Standard communication representation

- Simplifies signal classification

---

# Final Decision

QPSK will use an I/Q-based implementation.