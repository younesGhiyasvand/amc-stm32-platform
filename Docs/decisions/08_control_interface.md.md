# Control Interface

Version: 1.0

Status: Approved

Last Updated: 2026-06-17

---

# Objective

Define the interaction between the user and the transmitter.

---

# User Application Responsibilities

- Select modulation type
- Set carrier frequency
- Start transmission
- Stop transmission

---

# Communication Protocol

USB CDC

---

# Controlled Parameters

- Modulation type
- Carrier frequency
- Bit rate

---

# Final Decision

A lightweight PC application will control the STM32 transmitter.

---

# Board Configuration

The PC application communicates only with the transmitter board.

The transmitter role is assigned by firmware configuration.