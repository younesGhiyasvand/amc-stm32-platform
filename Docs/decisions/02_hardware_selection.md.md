# Hardware Selection

Version: 1.1

Status: Approved

Last Updated: 2026-06-18

---

# Objective

Select the most suitable hardware architecture for implementing a real-world Automatic Modulation Classification (AMC) platform.

---

# Evaluated Hardware Options

## Software Defined Radio (SDR)

Advantages:

- High flexibility
- Professional RF capabilities

Disadvantages:

- High cost
- Increased system complexity
- Reduced hardware design contribution

Decision: Rejected

---

## ESP32

Advantages:

- Wireless communication
- Low cost

Disadvantages:

- Limited processing capability for high-speed signal acquisition
- Less suitable for signal generation and DSP-oriented applications

Decision: Rejected

---

## STM32

Advantages:

- External high-speed ADC support
- External DAC support
- SPI interface
- DMA support
- DSP instructions
- Low cost
- Wide development ecosystem

Decision: Selected

---

# Final Decision

Two STM32F401CEU6 development boards will be used.

One board acts as the transmitter and one board acts as the receiver.

The microcontrollers are responsible for signal generation control, data acquisition, communication, and digital signal processing tasks.

---

# Hardware Architecture

The system consists of:

- STM32F401CEU6 Development Board (Transmitter)
- STM32F401CEU6 Development Board (Receiver)
- Custom Interface Board

The custom interface board is intended to contain:

- External DAC
- External ADC
- Analog signal conditioning circuits
- Signal filtering stages
- Interface connectors

External data converters are selected to provide greater flexibility and higher analog performance than the integrated peripherals available in low-cost microcontrollers.

---

# Development Board Strategy

Instead of designing a custom STM32 development board, commercially available STM32F401CEU6 development boards will be used.

A dedicated interface board will be designed to host the analog front-end circuitry, including ADC, DAC, filtering, and supporting components.

Two identical STM32F401CEU6 boards will be assembled and assigned different roles during experiments.

Board A → Transmitter

Board B → Receiver

This approach reduces development time, lowers hardware risk, and allows greater focus on signal processing, data acquisition, and AMC algorithm development.