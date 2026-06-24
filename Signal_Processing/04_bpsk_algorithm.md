# BPSK Algorithm

Version: 1.0

Status: Draft

Last Updated: 2026-06-21

---

# Objective

Define the software algorithm used to generate a BPSK signal.

---

# Input Data

Binary bit stream.

Example:

10110010

---

# Processing Steps

1. Read one bit.

2. Determine phase.

0 → 0°

1 → 180°

3. Generate carrier samples.

4. Repeat for all samples of the current bit.

5. Send samples to DAC.

6. Continue with the next bit.

---

# High-Level Algorithm

Bit Stream

↓

BPSK Mapper

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

phase = 0°

else

phase = 180°

for each sample

{

sample = A cos(2πfct + phase)

send sample to DAC

}

}

---

# Future Expansion

The same architecture will later support:

- BFSK
- QPSK
- 8PSK
- QAM

Only the modulation block will change.

---

# Final Decision

BPSK will be implemented using phase switching between 0° and 180°.