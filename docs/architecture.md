# System Architecture

## Objective

Develop an embedded system that takes surface EMG measurements,
transfers the data to a Linux computer, and processes the measurements
using a C++ application.

## Proposed Data Path

EMG electrodes
    -> EMG analogue front end
    -> STM32 ADC
    -> STM32 firmware
    -> Serial communication
    -> Linux C++ application
    -> Data logging and visualisation

## Component Responsibilities

### EMG Sensor

A commercial EMG sensor module will initially provide the analogue
signal conditioning required for muscle-activity measurements.

The exact output used by the system remains to be decided.

If time allows I could decide to build my own sensor module.

### STM32 Firmware

The firmware will eventually acquire measurements using the
microcontroller's ADC and transmit the measurements to the host.

Sampling behaviour, data representation and communication details
will be decided during implementation.

### Linux Application

The host application will receive and validate incoming data.

Planned capabilities include data logging, signal processing and
visualisation.

### Python Analysis

Python tools will be used to investigate recorded signals, explore
digital filters and validate processing approaches.

## Design Principles

- Implement the system incrementally.
- Keep hardware acquisition separate from host-side processing.
- Test individual components before full integration.
- Document design decisions and measured results.

## Current Limitations

The hardware has not yet been purchased, and no acquisition or
communication performance has been measured.
