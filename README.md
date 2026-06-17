# CO₂ Monitoring and Health Risk Assessment System

## Overview

The CO₂ Monitoring and Health Risk Assessment System is an IoT-based solution designed to monitor indoor carbon dioxide (CO₂) levels in real time and assess potential health risks caused by poor air quality. The system integrates IoT sensors, cloud-based data processing, a backend API, a web dashboard, and a mobile application to provide continuous monitoring, location tracking, alerts, and historical data analysis.

This project was developed as a final-year research project for the Bachelor of Science in Software Engineering.

## Objectives

* Monitor indoor CO₂ concentration levels in real time.
* Track sensor locations using GPS technology.
* Store environmental data securely in the cloud.
* Provide real-time alerts when CO₂ levels exceed safe thresholds.
* Visualize historical air quality trends through dashboards.
* Support decision-making for healthier indoor environments.

## System Architecture

The system consists of four main layers:

### 1. IoT Device Layer

* SGP30 Air Quality Sensor
* ESP32 / ESP8266 / ATmega2560 Microcontroller
* NEO-6M GPS Module
* Wi-Fi / GSM Communication Module

### 2. Communication Layer

* HTTP/HTTPS Protocol
* MQTT (Optional)

### 3. Backend & Cloud Layer

* Spring Boot REST API
* JWT Authentication
* MySQL Database
* Firebase Services

### 4. Presentation Layer

* React Web Dashboard
* Flutter Mobile Application

## Features

### Real-Time Monitoring

* Live CO₂ concentration measurements (PPM)
* Continuous sensor data collection

### GPS Location Tracking

* Real-time device location monitoring
* Google Maps integration

### Alert System

* High CO₂ threshold notifications
* Health risk warnings

### Historical Data Analysis

* Daily, weekly, and monthly trends
* Statistical reports and charts

### User Management

* User registration and login
* Role-based access control (Admin/User)

### Device Management

* Register and manage multiple IoT devices
* Track device activity and status

## Technology Stack

### Hardware

* SGP30 CO₂ Sensor
* ESP32 / ESP8266
* ATmega2560
* NEO-6M GPS Module

### Backend

* Java Spring Boot
* Spring Security
* JWT Authentication
* REST API

### Frontend

* React.js
* HTML5
* CSS3
* JavaScript

### Mobile Application

* Flutter
* Dart

### Database

* MySQL
* Firebase

### Tools

* Arduino IDE
* Postman
* Git
* GitHub

## Project Structure

```text
CO2-Monitoring-System/
│
├── backend/
│   ├── src/
│   └── pom.xml
│
├── frontend/
│   ├── src/
│   └── package.json
│
├── mobile-app/
│   ├── lib/
│   └── pubspec.yaml
│
├── arduino/
│   ├── sensor_code.ino
│   └── libraries/
│
├── database/
│   └── schema.sql
│
├── screenshots/
│
└── README.md
```

## Installation Guide

### Backend Setup

```bash
git clone https://github.com/yourusername/co2-monitoring-system.git

cd backend

mvn clean install

mvn spring-boot:run
```

### Frontend Setup

```bash
cd frontend

npm install

npm start
```

### Mobile Application Setup

```bash
cd mobile-app

flutter pub get

flutter run
```

### Arduino Setup

1. Install Arduino IDE.
2. Connect ESP32/ESP8266 board.
3. Install required sensor libraries.
4. Upload the Arduino sketch.
5. Configure Wi-Fi credentials and API endpoint.

## Database Schema

Main Tables:

* Users
* Roles
* Devices
* CO2_Measurements

Each measurement contains:

* Device ID
* CO₂ Value (PPM)
* Latitude
* Longitude
* Timestamp

## Testing

### Functional Testing

* User Authentication
* Device Registration
* CO₂ Data Upload
* GPS Tracking
* Alert Generation

### Non-Functional Testing

* Performance Testing
* Security Testing
* Load Testing
* Reliability Testing

### Load Testing Results

| Test Scenario              | Result      |
| -------------------------- | ----------- |
| 100 Concurrent Users       | Pass        |
| 5000 Records/Minute Upload | Pass        |
| Dashboard Response         | < 3 Seconds |
| 24-Hour Continuous Stream  | Pass        |

## Research Contribution

This research demonstrates how IoT technologies can be applied to improve indoor air quality monitoring and reduce health risks associated with elevated carbon dioxide concentrations. The system provides a scalable and cost-effective solution suitable for offices, educational institutions, healthcare facilities, and industrial environments.

## Future Improvements

* AI-based air quality prediction
* HVAC integration
* iOS mobile application
* Advanced analytics dashboard
* Cloud deployment using AWS

## Screenshots


### Mobile Application

#### Login Screen
images/Picture1.png

#### Dashboard

#### Historical CO₂ Trends

### Admin Dashboard

#### System Overview

#### Device Monitoring

#### Live Map Tracking

## Authors

**Sumedha Eranda**

BSc (Hons) Software Engineering

Final Year Research Project

## License

This project is developed for academic and research purposes.

Copyright © 2026 Sumedha Eranda
