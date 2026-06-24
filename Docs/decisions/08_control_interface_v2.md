# Control Interface

Version: 2.0

Status: Approved

Last Updated: 2026-06-21

---

# Objective

Define the interaction between the user and the standalone AMC platform.

---

# User Interaction Method

The user will interact directly with the transmitter board.

No permanent PC connection is required.

---

# Hardware Interface

The transmitter board will include:

- LCD display
- Navigation buttons
- Confirmation button

---

# User Configurable Parameters

The user can configure:

- Modulation type
- Carrier frequency
- Bit rate
- Start transmission
- Stop transmission

---

# Control Sequence

User

↓

Navigation Buttons

↓

LCD Menu

↓

Configuration Manager

↓

STM32 TX

↓

Signal Generation

---

# Available Modulations

Initial modulations:

- BPSK
- BFSK
- QPSK

Future modulations:

- 8PSK
- ASK
- 16QAM
- 64QAM

---

# Final Decision

The AMC platform will be controlled directly from the transmitter board using an embedded user interface.