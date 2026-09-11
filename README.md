# Solar IQ — AI-Powered Solar Panel Monitoring & Predictive Maintenance

An AI-assisted solar panel monitoring system that combines IoT sensors, computer vision, cloud data, and predictive maintenance to monitor photovoltaic panel health and performance.

## Project Overview

Solar IQ is designed to continuously monitor solar panel operating conditions and identify potential problems such as:

- Dust accumulation
- Shading
- Bird droppings
- Physical damage
- Abnormal operating conditions
- Temperature-related performance changes

The system combines sensor measurements with AI-based image analysis to provide a more complete view of solar panel health.

## System Architecture

```text
                    Solar Panel
                         |
          +--------------+--------------+
          |              |              |
       Voltage       Temperature      Camera
       Sensor          Sensors           |
          |              |               |
          +--------------+---------------+
                         |
                       ESP32
                         |
                         v
                   Firebase Cloud
                         |
              +----------+----------+
              |                     |
              v                     v
       Sensor Analytics       AI Image Analysis
                                    |
                                    v
                         Panel Condition
                           Classification
                                    |
                                    v
                         Maintenance Alert
