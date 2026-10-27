# EMG Embedded System

A surface electromyography (EMG) acquisition and monitoring system built around an STM32 microcontroller, with a C++ application on Linux and Python tools for analysis.

## Overview

This is a personal project designed to help me learn embedded firmware, DSP, Linux application development and general hardware-software integration. 

## Planned Architecture

The system will have four parts:

1. An EMG sensor 
2. An STM32 microcontroller that samples the signal and applies some signal processing
3. A serial link between the microcontroller and the host computer
4. A C++ application on the host that receives the measurements, applies some signal processing and performs visualisation and analysis.

A commercial EMG sensor is the easiest to implement and the safest option here. I may explore designing my own in the future if I have time.

## Technologies

- C for the embedded firmware on the STM32
- C++ for the Linux application
- Potentially python for additional signal analysis
- Linux and command-line development tools
- Git and GitHub for version control

## Repository Structure

- `docs/`: architecture, design notes and project planning
- `firmware/`: STM32 firmware
- `software/`: Linux-side C++ application
- `tests/`: testing and verification
- `hardware/`: hardware documentation and circuit designs

## Project Status

**Right now this is at the planning and repository setup stage.**

I haven't bought any hardware yet, and nothing has been implemented or tested. 
