# ECU Speed — Vehicle Speed Acquisition Module

## Overview

This module is dedicated to the development of the vehicle speed acquisition ECU within the EV-CORE project.

Its purpose is to acquire, process and prepare vehicle speed information for transmission to the central ECU through the CAN bus.

This module represents my individual contribution to the EV-CORE embedded system project.

## Functional Role

The ECU Speed module is responsible for:

- Acquiring the speed-related signal.
- Processing the acquired information to determine vehicle speed.
- Preparing the speed data for CAN transmission.
- Transmitting speed information to the central ECU.
- Supporting integration into the distributed EV-CORE architecture.

## Embedded Development

The module is developed around an STM32 microcontroller using STM32 embedded development tools.

The implementation, peripheral configuration, signal processing and communication logic will be documented as the development progresses.

## System Integration

The ECU Speed module is part of a distributed architecture composed of multiple STM32 ECUs.

Its processed speed information is intended to be transmitted through CAN to the central ECU, which validates and aggregates information from the different modules.

## Development Scope

My work focuses on the vehicle speed acquisition ECU, including:

- STM32 configuration and firmware development.
- Speed signal acquisition.
- Speed calculation and processing.
- CAN communication integration.
- Module testing and validation.

## Status

**In Development**

This module is currently under development as part of the EV-CORE academic engineering project.

---

*Individual contribution — Vehicle Speed Acquisition ECU for EV-CORE.*
