# ESP32-Based Animal Tracking System

An IoT-based animal tracking and monitoring prototype developed using ESP32, GPS, GSM communication, and environmental sensors.

## Project Overview

The Animal Tracking System is designed to help monitor an animal's location and environmental conditions using Internet of Things (IoT) technology.

The system uses an ESP32 microcontroller to collect and process data from connected modules. GPS provides location coordinates, while GSM communication enables SMS-based location requests. A web-based interface allows users to view the location and sensor information.

This project was developed as part of the B.Tech Electronics and Computer Engineering capstone project at CMR University (2024–2025).

## Features

- GPS-based location tracking.
- Location visualization using Leaflet.js.
- Temperature and humidity monitoring using DHT11.
- GSM-based SMS location requests using SIM800L.
- Web-based monitoring interface hosted by ESP32.
- Remote buzzer control through the web interface.
- Wi-Fi-based communication for web monitoring.

## Hardware Components

| Component | Purpose |
|---|---|
| ESP32 | Main microcontroller |
| GPS Module | Obtains geographical coordinates |
| SIM800L GSM Module | Sends and receives SMS messages |
| DHT11 Sensor | Measures temperature and humidity |
| Pulse Sensor | Used for pulse-monitoring functionality |
| Buzzer | Provides an alert mechanism |

## Software and Technologies

- ESP32 programming environment
- Arduino-compatible libraries
- TinyGPS++ – GPS data parsing
- HTML and CSS – Web interface
- JavaScript – Dynamic data updates
- Leaflet.js – Map visualization
- Wi-Fi and GSM communication

## System Architecture

1. The GPS module obtains the geographical coordinates.
2. The ESP32 receives and processes the GPS data.
3. TinyGPS++ is used to parse GPS information.
4. The ESP32 hosts a web interface that displays location and sensor information.
5. Leaflet.js displays the location on an interactive map.
6. The SIM800L module supports SMS-based location requests.
7. A buzzer can be controlled remotely through the web interface.

## Implementation Details

### GPS Tracking
The GPS module provides latitude and longitude coordinates. The ESP32 processes the incoming data using the TinyGPS++ library.

### Web-Based Monitoring
An ESP32-hosted web interface displays location and sensor information. The interface uses JavaScript and AJAX to refresh displayed information periodically. Leaflet.js is used to visualize the location on a map.

### GSM Communication
The SIM800L module provides GSM-based communication. Users can request location information through SMS, including when internet connectivity is unavailable.

### Environmental Monitoring
The DHT11 sensor is used to obtain temperature and humidity readings.

### Alert Mechanism
A buzzer connected to the system can be activated through the web interface.

## Important Project Limitations

- Pulse sensor readings in the documented prototype were simulated and were not validated as actual animal heart-rate measurements.
- The documented implementation uses Wi-Fi and GSM communication; LoRa communication and Firebase cloud storage are not part of the implementation described in the project report.
- AI-based anomaly detection is a possible future enhancement, not an implemented feature.

## Future Enhancements

- Integration of validated animal health-monitoring sensors.
- GPS tracking improvements and power optimization.
- Cloud-based data storage and remote access.
- AI-based analysis of animal movement and behaviour.
- Mobile application integration.
- Long-range communication technologies such as LoRaWAN.

## Project Contributors

- Rakiba Hussain Z.
- Dhumbi Shree L.

## Academic Details

**Degree:** B.Tech – Electronics and Computer Engineering  
**Institution:** CMR University  
**Academic Year:** 2024–2025
