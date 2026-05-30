<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/1850b79f-9989-4140-b4c5-e574b55a5ebe" /># GPS Location Tracking using ESP32 and TinyGPS++

## Overview

This project demonstrates how to interface a GPS module with an ESP32 microcontroller using the TinyGPS++ library. The system continuously reads NMEA data from the GPS module through UART communication and extracts real-time latitude and longitude coordinates.

The coordinates are displayed on the Serial Monitor for location tracking applications.

## Features

* Real-time GPS location tracking
* Latitude and Longitude extraction
* Serial Monitor output
* GPS validity checking
* Automatic GPS connection detection
* Easy integration with ESP32

## Hardware Requirements

* ESP32 Development Board
* NEO-6M GPS Module (or compatible GPS module)
* Jumper Wires
* USB Cable

## Software Requirements

* Arduino IDE
* ESP32 Board Package
* TinyGPS++ Library

## Library Installation

1. Open Arduino IDE.
2. Navigate to:
   Sketch → Include Library → Manage Libraries
3. Search for:
   TinyGPS++
4. Install:
   TinyGPSPlus by Mikal Hart

## Connections

| GPS Module | ESP32        |
| ---------- | ------------ |
| VCC        | 3.3V         |
| GND        | GND          |
| TX         | RX2 (GPIO16) |
| RX         | TX2 (GPIO17) |

## Working Principle

1. GPS module receives satellite signals.
2. NMEA sentences are transmitted through UART.
3. ESP32 reads NMEA data using Serial2.
4. TinyGPS++ parses the received data.
5. Latitude and longitude are extracted.
6. Coordinates are displayed on the Serial Monitor.

## Serial Output

Location: Lat: 12.971598, Lng: 77.594566

## Safety Check

If no GPS data is received within 5 seconds, the system displays:

No GPS detected: check wiring.

and stops execution.

## Applications

* Vehicle Tracking
* Asset Tracking
* Smart Transportation
* Navigation Systems!
* IoT Location Monitoring
* Emergency Tracking Systems

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/789a3a59-4d69-4054-92c2-0362a3a8b197" />


## Author

Hariharan Balakrishnan

Electronics and Communication Engineering
ESP32 | Embedded Systems | IoT | Zephyr RTOS
