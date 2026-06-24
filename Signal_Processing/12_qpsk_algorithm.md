# QPSK Algorithm

Version: 1.0

Status: Draft

Last Updated: 2026-06-21

---

# Objective

Define the software algorithm used to generate a QPSK signal.

---

# Input Data

Binary bit stream.

Example:

10110010

---

# Processing Steps

1. Read two bits.

2. Determine I and Q values.

3. Generate carrier samples.

4. Repeat for all samples of the current symbol.

5. Send samples to DAC.

6. Continue with the next symbol.

---

# High-Level Algorithm

Bit Stream

↓

Symbol Mapper

↓

I/Q Generator

↓

Sample Generator

↓

DAC

↓

Analog Signal

---

# Pseudo Code

for each symbol

{

read 2 bits

select I,Q

for each sample

{

sample = I*cos(2πfct)

        -Q*sin(2πfct)

send sample to DAC

}

}

---

# Future Expansion

The same architecture will later support:

- 8PSK
- 16QAM
- 64QAM

Only the symbol mapper will change.

---

# Final Decision

QPSK will be implemented using an I/Q-based architecture.