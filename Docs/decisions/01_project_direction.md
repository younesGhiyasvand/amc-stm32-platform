# Project Direction

Version: 1.0

Status: Approved

Last Updated: 2026-06-17

---

# Objective

The objective of this project is to design and implement an Automatic Modulation Classification (AMC) platform using real-world transmitted signals instead of simulation-only datasets.

The system aims to provide a practical framework for generating, transmitting, receiving and classifying digitally modulated signals.

---

# Initial Project Idea

The initial idea was to build a software-based AMC system using simulated datasets generated entirely inside MATLAB or Python.

The system would perform:

- Signal generation
- Feature extraction
- Classification

without any physical hardware implementation.

---

# Limitations of a Simulation-Only Approach

Several limitations were identified:

- Limited practical value
- Reduced engineering complexity
- Lower evaluation potential during project defense
- No real-world signal impairments
- No hardware integration

---

# New Project Direction

The project was redesigned as a hardware-assisted AMC platform.

The new architecture includes:

- STM32F401CEU6 development board (Transmitter)
- STM32F401CEU6 development board (Receiver)
- Custom interface board
- Real analog transmission channel
- PC-based signal processing
- Machine learning classification

---

# Long-Term Vision

The developed AMC platform is designed to be extensible and support future research activities.

- Advanced machine learning models
- Spiking Neural Networks (SNN)
- Unsupervised learning approaches
- Scientific publications

---

# Final Decision

The project will focus on building a real-world Automatic Modulation Classification platform rather than a simulation-only implementation.