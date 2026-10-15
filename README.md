# EMG Embedded System

A surface electromyography (EMG) acquisition and monitoring system built around an STM32 microcontroller, with a C++ application on Linux and Python tools for analysis.

## Overview

I'm building this to get hands-on with the full embedded stack: reading muscle-activity signals with a microcontroller, getting that data onto a Linux machine, and then processing and visualising it. It's a learning project, covering embedded firmware, hardware-software integration, digital signal processing and Linux application development.

## Planned Architecture

The system will have five parts:

1. An EMG sensor and analogue front end
2. An STM32 microcontroller that samples the signal
3. A serial link between the microcontroller and the host computer
4. A C++ application on the host that receives and processes the measurements
5. Python tools for analysis and visualisation

I'll start with a commercial EMG sensor module. Designing my own analogue front end is something I may try later as an extension.

## Technologies

- C for the embedded firmware
- STM32 microcontrollers
- C++ for the Linux application
- Python for signal analysis and testing
- Linux and command-line development tools
- Git and GitHub for version control

## Repository Structure

- `docs/`: architecture, design notes and project planning
- `firmware/`: STM32 firmware
- `software/`: Linux-side C++ application
- `analysis/`: Python signal analysis
- `tests/`: testing and verification
- `hardware/`: hardware documentation and circuit designs

## Project Status

**Right now this is at the planning and repository setup stage.**

I haven't bought any hardware yet, and nothing has been implemented or tested. Everything below is a goal, not a finished feature:

- Acquiring EMG signals with an STM32
- Sending data to a Linux computer over serial
- Receiving and logging that data in C++
- Signal processing and visualisation
- Detecting muscle activation
- Testing and verifying the whole system end to end

## What's Next

I'll build this up step by step: first the development environment and some basic microcontroller firmware, then the EMG sensor, and finally the host application.
