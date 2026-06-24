# BFSK Algorithm

Version: 1.0

Status: Draft

Last Updated: 2026-06-21

---

# Objective

Define the software algorithm used to generate a BFSK signal.

---

# Input Data

Binary bit stream.

Example:

10110010

---

# Processing Steps

1. Read one bit.

2. Select frequency.

0 → 40 kHz

1 → 60 kHz

3. Generate carrier samples.

4. Repeat for all samples of the current bit.

5. Send samples to DAC.

6. Continue with the next bit.

---

# High-Level Algorithm

Bit Stream

↓

Frequency Selector

↓

Sample Generator

↓

DAC

↓

Analog Signal

---

# Pseudo Code

for each bit

{

if bit == 0

f = 40kHz

else

f = 60kHz

for each sample

{

sample = A cos(2πft)

send sample to DAC

}

}

---

# Future Expansion

The same architecture will later support:

- QPSK
- 8PSK
- QAM

Only the modulation block will change.

---

# Final Decision

BFSK will be implemented using frequency switching between 40 kHz and 60 kHz.