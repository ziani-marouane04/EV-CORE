# ECU 1 — Vehicle Speed Acquisition

## Role

This ECU is responsible for acquiring vehicle speed data and preparing it for transmission to the central ECU through the CAN bus.

## Intended Responsibilities

- Acquire vehicle speed information.
- Process the acquired signal.
- Prepare speed data for CAN transmission.
- Communicate with the central ECU through CAN.

## Hardware

- STM32 microcontroller
- Speed sensing interface (implementation to be documented)

## Communication

The speed information is intended to be transmitted to the central ECU through CAN.

Frame identifiers, data encoding, transmission frequency and implementation details will be documented as development progresses.

## Status

**In Development**

This module is part of the EV-CORE distributed embedded architecture.
