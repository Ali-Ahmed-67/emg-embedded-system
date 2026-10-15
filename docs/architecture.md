## Hardware and Software Interfaces

### EMG Sensor to STM32

The EMG sensor will provide an analogue output that can be sampled
using the STM32 ADC.

The specific sensor output, voltage range, ADC configuration and
sampling frequency must be established before implementation.

The selected output must be compatible with the STM32 input range.

### STM32 to Host Computer

The STM32 will transmit measurement data to the host computer over
a serial connection, initially expected to use USB.

The exact transport mechanism and data format will be determined
when the STM32 development board is selected.

The communication interface should support reliable acquisition
and straightforward debugging.

### Host Application

The C++ application will separate data reception from subsequent
processing and visualisation.

This should allow recorded measurements to be analysed independently
of the live acquisition system.

## Initial Design Decisions

| Decision | Initial approach | Status |
|---|---|---|
| EMG analogue front end | MyoWare 2.0 | Planned |
| Microcontroller | STM32 development board | To be selected |
| Firmware language | C | Planned |
| Host operating system | Ubuntu Linux | Available |
| Host application language | C++ | Planned |
| Signal analysis | Python | Planned |
| Communication | Serial over USB | To be verified |
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
