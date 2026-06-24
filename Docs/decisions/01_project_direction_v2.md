# Project Direction

Version: 2.0

Status: Approved

Last Updated: 2026-06-21

---

# Objective

The objective of this project is to design and implement a standalone Automatic Modulation Classification (AMC) platform using real-world transmitted signals instead of simulation-only datasets.

The system aims to provide a practical framework for generating, transmitting, receiving and classifying digitally modulated signals without requiring a permanent PC connection for operation.

---

# Motivation For Revision

The initial architecture required a direct communication link between the PC and the transmitter board.

After evaluation, this approach introduced unnecessary system dependency.

The architecture was redesigned to increase portability and system autonomy.

---

# New Project Direction

The AMC platform will operate as a standalone embedded system.

The transmitter board will contain its own user interface, allowing users to configure experiments directly from the hardware.

The PC will only be used for data processing and machine learning tasks.

---

# Main System Components

- STM32F401CEU6 Transmitter Board
- STM32F401CEU6 Receiver Board
- TX Analog Board
- RX Analog Board
- User Interface Module
- PC Processing Unit

---

# Long-Term Vision

This platform is intended to become a research infrastructure that can later support:

- Advanced machine learning models
- Spiking Neural Networks (SNN)
- Unsupervised learning approaches
- Scientific publications

---

# Final Decision

The AMC platform will operate as a standalone embedded system.

Signal generation and experiment configuration will be performed directly from the transmitter board without requiring a permanent PC connection.