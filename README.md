# EV-CORE
### Embedded Multi-ECU Data Acquisition, Communication & Monitoring System for Electric Vehicles

EV-CORE is an academic embedded systems project focused on designing a distributed architecture for collecting, processing, communicating and monitoring data within an electric vehicle.

The system integrates multiple STM32 microcontrollers, CAN bus communication, UART transmission, an ESP32 connectivity module and an MQTT-based monitoring architecture.

## System Architecture

The architecture is based on distributed data acquisition and centralized processing.

- **STM32 ECU 1:** Vehicle speed data acquisition.
- **STM32 ECU 2:** Battery State of Charge (SoC) data acquisition and estimation.
- **STM32 ECU 3 – Central Unit:** Receives, validates and aggregates information transmitted by the other ECUs over CAN.
- **ESP32:** Communication gateway between the STM32 central unit and the MQTT infrastructure through UART.
- **MQTT Broker:** Handles message distribution.
- **Dashboard:** Displays collected vehicle information.

## Architecture Overview

```text
 STM32 ECU 1             STM32 ECU 2
 Speed Acquisition       Battery SoC
       |                     |
       +--------- CAN --------+
                 |
                 v
          STM32 ECU 3
          Central Unit
     Data Validation & Aggregation
                 |
               UART
                 |
                 v
              ESP32
           Wi-Fi / MQTT
                 |
                 v
           MQTT Broker
                 |
                 v
          EV Dashboard
```

## Technologies

- STM32
- Embedded C / C++
- CAN Bus
- UART
- ESP32
- Wi-Fi
- MQTT

## Objectives

- Design a distributed embedded architecture.
- Implement communication between multiple microcontrollers.
- Exchange information using CAN bus.
- Validate and aggregate incoming data.
- Establish UART communication between STM32 and ESP32.
- Transmit vehicle data using MQTT.
- Develop a dashboard for monitoring vehicle information.

## Project Status

**In Development**

This project is currently under development as part of an academic engineering project. Components and functionalities are progressively implemented, tested and integrated.

## Academic Project

Developed as part of an engineering project in Automotive Engineering and Digital Solutions.

---

*EV-CORE — Connecting embedded ECUs to intelligent vehicle monitoring.*
