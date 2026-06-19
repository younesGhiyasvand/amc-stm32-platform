# Pin Assignment

Version: 1.0

Status: Approved

Last Updated: 2026-06-18

---

# Objective

Define all STM32F401CEU6 pin assignments used by the AMC hardware platform.

The STM32F401CEU6 communicates with external ADC and DAC devices located on the custom interface board.

---

# STM32F401CEU6 Pin Allocation

## USB Communication

| Function | Pin  |
|----------|------|
| USB_DM   | PA11 |
| USB_DP   | PA12 |

Purpose:

- USB CDC communication
- PC control interface
- Data transfer

---

## SWD Debug Interface

| Function | Pin  |
|----------|------|
| SWDIO    | PA13 |
| SWCLK    | PA14 |

Purpose:

- Firmware programming
- Debugging

---

## External DAC Interface (SPI1)

| Function  | Pin |
|-----------|-----|
| DAC_SCK   | PA5 |
| DAC_MOSI  | PA7 |
| DAC_CS    | PB0 |
| DAC_LDAC  | PB1 |

Purpose:

- DAC configuration
- DAC data transmission
- Signal generation

---

## External ADC Interface (SPI2)

| Function | Pin  |
|----------|------|
| ADC_SCK  | PB13 |
| ADC_MISO | PB14 |
| ADC_CS   | PB12 |
| ADC_DRDY | PB15 |

Purpose:

- ADC control
- ADC data acquisition
- Conversion synchronization

---

## Sample Clock Output

| Function   | Pin |
|------------|-----|
| SAMPLE_CLK | PA8 |

Purpose:

- ADC sampling clock
- DAC update clock
- Timing synchronization

Peripheral:

- TIM1_CH1

---

## Status Indicators

| Function   | Pin  |
|------------|------|
| STATUS_LED | PC13 |

Purpose:

- System status
- Error indication
- Activity indication

---

## Reserved Expansion Pins

| Pin  |
|------|
| PA0  |
| PA1  |
| PA2  |
| PA3  |
| PA4  |
| PA6  |
| PA9  |
| PA10 |
| PB2  |
| PB3  |
| PB4  |
| PB5  |
| PB6  |
| PB7  |
| PB8  |
| PB9  |
| PB10 |

Purpose:

- Future expansion
- Additional sensors
- UART interfaces
- Trigger signals
- Experimental features

---

# Interface Board Connector

## Digital Signals

| Signal       |
|--------------|
| DAC_SCK      |
| DAC_MOSI     |
| DAC_CS       |
| DAC_LDAC     |
| ADC_SCK      |
| ADC_MISO     |
| ADC_CS       |
| ADC_DRDY     |
| SAMPLE_CLK   |
| ACTIVITY_LED |

---

## Power Signals

| Signal   |
|----------|
| +3.3V    |
| GND      |

---

# Notes

- No internal ADC channels are used.
- No internal DAC peripherals are used.
- All analog conversion is performed on the custom interface board.
- SPI communication uses DMA whenever possible.
- Analog and digital grounds must be carefully separated on the interface board.