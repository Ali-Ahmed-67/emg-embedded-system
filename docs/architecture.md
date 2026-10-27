## Hardware and Software Interfaces

### EMG Sensor to STM32

The EMG sensor will provide an analogue output that can be sampled
using the STM32 ADC.

The specific sensor output, voltage range, ADC configuration and
sampling frequency will be established.

I plan to implement some DSP/other algorithms on the STM32 in C. This could also be implemented on the host computer, but I would like to practice programming in C with a low-memory system.

### STM32 to Host Computer

The STM32 will transmit measurement data to the host computer over
a serial connection, initially via USB.

### Host Application

The C++ application will separate data reception from subsequent
processing and visualisation.

This should allow recorded measurements to be analysed independently
of the live acquisition system.

## Initial Design Decisions

| Decision | Initial approach | Status |
|---|---|---|
| EMG analogue front end | MyoWare 2.0 | Planned |
| Microcontroller | NUCLEO-F411RE | Planned |
| Firmware language | C | Planned |
| Host operating system | Ubuntu Linux | Available |
| Host application language | C++ | Planned |
| Communication | Serial over USB | Planned |
| Data logging | CSV | Proposed |
| Live visualisation | To be selected | Undecided |

## Outstanding Engineering Questions

Before implementing the acquisition system, determine:

- Which STM32 development board to use.
- Which MyoWare output to sample.
- Whether the selected output is appropriate for the intended
  sampling and signal-processing requirements.
- The required sampling frequency and ADC configuration.
- How measurements will be represented and transmitted.
- How the complete body-connected electrical setup will be
  made appropriately safe.

These decisions should be documented as the design develops.
