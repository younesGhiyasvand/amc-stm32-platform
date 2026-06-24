# TX User Interface

Version: 1.0

Status: Approved

Last Updated: 2026-06-21

---

# Objective

Define the onboard user interface implemented on the transmitter board.

---

# User Interface Components

The transmitter board will include:

- 16x2 LCD
- UP button
- DOWN button
- LEFT button
- RIGHT button
- OK button

---

# LCD Responsibilities

The LCD will display:

- Current modulation
- Carrier frequency
- Bit rate
- System status

---

# Navigation Structure

Main Menu

↓

Select Modulation

↓

Carrier Frequency

↓

Bit Rate

↓

Start Transmission

---

# Button Functions

| Button | Function |
|--------|----------|
| UP | Move up |
| DOWN | Move down |
| LEFT | Go back |
| RIGHT | Move forward |
| OK | Confirm selection |

---

# Example Screen

Running

BPSK

fc = 50 kHz

---

# Design Goals

The user interface should be:

- Simple
- Standalone
- Easy to use
- Independent from external computers

---

# Final Decision

The transmitter board will provide a complete standalone user interface using a 16x2 LCD and navigation buttons.