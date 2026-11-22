# EV-CORE
### Embedded Multi-ECU Data Acquisition, Communication & Monitoring System for Electric Vehicles

EV-CORE is an academic embedded systems project focused on designing a distributed architecture for collecting, processing, communicating and monitoring data within an electric vehicle.

The system integrates multiple STM32 microcontrollers, CAN bus communication, UART transmission and a Raspberry Pi 5 hosting an MQTT broker to support vehicle data monitoring and visualization.

---

## System Architecture

The architecture is based on distributed data acquisition and centralized processing.

- **STM32 ECU 1:** Vehicle speed data acquisition.
- **STM32 ECU 2:** Battery State of Charge (SoC) estimation and data acquisition.
- **STM32 ECU 3 – Central Unit:** Receives, validates and aggregates information transmitted by the other ECUs over CAN.
- **Raspberry Pi 5:** Receives aggregated data from the central STM32 through UART and hosts the MQTT broker.
- **MQTT Broker:** Handles message distribution to connected monitoring clients.
- **Dashboard:** Displays collected vehicle information.

---

## Architecture Overview

```text
       STM32 ECU 1                 STM32 ECU 2
     Speed Acquisition           Battery SoC
             |                         |
             +----------- CAN ----------+
                          |
                          v
                  STM32 ECU 3
                  Central Unit
           Data Validation & Aggregation
                          |
                        UART
                          |
                          v
                   Raspberry Pi 5
                    MQTT Broker
                          |
                          v
                    EV Dashboard
```

---

## Technologies

- STM32 Microcontrollers
- Embedded C / C++
- CAN Bus
- UART
- Raspberry Pi 5
- MQTT
- Dashboard Development

---

## Project Objectives

- Design a distributed embedded architecture.
- Implement communication between multiple microcontrollers.
- Exchange information using CAN bus.
- Validate and aggregate incoming data.
- Establish UART communication between the central STM32 and Raspberry Pi 5.
- Deploy an MQTT broker on the Raspberry Pi 5.
- Transmit vehicle data through MQTT.
- Develop a monitoring dashboard for vehicle information.

---

## Project Status

**Status: In Development**

This project is currently under development as part of an academic engineering project. Components and functionalities are progressively implemented, tested and integrated.

---

## Academic Project

Developed as part of an engineering project in Automotive Engineering and Digital Solutions.

---

*EV-CORE — Connecting embedded ECUs to intelligent vehicle monitoring.*
