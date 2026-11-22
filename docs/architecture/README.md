# System Architecture Documentation

This directory contains the architectural documentation of EV-CORE.

## System Overview

EV-CORE is designed around a distributed multi-ECU architecture. Individual microcontrollers handle dedicated data acquisition tasks, while a central ECU validates and aggregates the data.

The aggregated information is transmitted to an ESP32 through UART. The ESP32 acts as the connectivity gateway and publishes the data through MQTT for dashboard visualization.

## Architecture Components

| Component | Role |
|---|---|
| STM32 ECU 1 | Vehicle speed data acquisition |
| STM32 ECU 2 | Battery State of Charge data acquisition and estimation |
| STM32 ECU 3 | Central data validation and aggregation |
| CAN Bus | Communication between STM32 ECUs |
| UART | Communication between central STM32 and ESP32 |
| ESP32 | Wi-Fi and MQTT connectivity gateway |
| MQTT Broker | Message distribution |
| Dashboard | Data visualization and monitoring |

## Architecture Diagram

The system architecture diagram will be added here as the design documentation progresses.

## Documentation Status

Architecture documentation is progressively being developed alongside the implementation.
