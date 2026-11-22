# CAN Bus Communication

## Overview

The Controller Area Network (CAN) bus is used as the communication medium between the STM32 microcontrollers in the EV-CORE architecture.

It enables the distributed ECUs to exchange vehicle-related information with the central processing unit.

## Communication Role

CAN communication is intended to connect the data acquisition ECUs to the central ECU.

- **STM32 ECU 1:** Transmits vehicle speed information.
- **STM32 ECU 2:** Transmits battery-related information, including State of Charge (SoC).
- **STM32 ECU 3:** Receives and processes information transmitted by the other ECUs.

## Communication Workflow

1. Data is acquired or estimated by the dedicated ECU.
2. The ECU prepares the information for transmission over CAN.
3. CAN frames are exchanged between the ECUs.
4. The central ECU receives and validates the frames.
5. Validated information is aggregated for further transmission.

## CAN Frame Definition

The CAN frame identifiers, data fields, encoding, transmission periods and validation rules will be documented as the communication implementation progresses.

| Parameter | Description |
|---|---|
| CAN Protocol | CAN |
| Transmitting Nodes | Data acquisition ECUs |
| Receiving Node | Central ECU |
| Data | Vehicle speed and battery-related information |
| Frame IDs | To be defined |
| Transmission Period | To be defined |

## Implementation Status

CAN communication design and implementation are progressively developed and tested as part of the EV-CORE project.

---

*This documentation will be updated as the CAN communication implementation evolves.*
