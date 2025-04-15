---
title: "Yatsa Asset Tracking – IoT Data Pipeline"
excerpt: "Real-time vehicle tracking and fleet management system developed for Web, Android (Kotlin) & iOS (SwiftUI).<br/><img src='/images/yatsa.png'>"
collection: portfolio
---

## Overview

The Yatsa Asset Tracking project is a cutting-edge IoT solution designed to deliver real-time asset monitoring and improve operational efficiency for logistics and transportation. By standardizing communications across diverse tracking devices and reconstructing trips in real time, this platform ensures timely, context-aware compliance notifications and operational visibility.

## Technical Approach

- **IoT Gateway Development:**
  Engineered an IoT gateway using **Azure IoT Hub** to standardize data collection from various third-party tracking devices. The gateway automates protocol translation across a wide range of communication protocols, including:
  - **Gt06, TkStar, GPS103, GT02, TK103, HTTP, MQTT, AMQP, CoAP, Mictrack, Teltonika, Meitrack, and Huabao.**
  This automation drastically reduced device onboarding time and simplified integration.

- **Real-Time Asset Tracking:**

  Developed a real-time asset tracking system that reconstructs trips on the fly. Key techniques include:
  - **Reverse Geocoding & Route Snapping:** Utilized Google APIs to convert raw GPS coordinates into human-readable locations and align routes with actual roadways.
  - **Automated Alerts:** Integrated notifications for curfew violations, speeding, and geofence breaches, ensuring stakeholders receive timely, context-aware alerts via push notifications.

## Implementation Details

- **Data Ingestion:**
  The IoT gateway securely ingests telemetry data from tracking devices using a standardized set of protocols, ensuring a consistent data format for downstream processing.

- **Digital Trip Reconstruction:**
  Leveraged Google’s Geocoding and Directions APIs to create accurate trip trajectories and inform operational decision-making through dynamic route mapping.

- **Alerting System:**
  Built a configurable rules engine that triggers push notifications when specific conditions—such as curfew violations or geofence breaches—are detected, enhancing compliance and operational control.

## Business Impact

- **Enhanced Operational Efficiency:**
  Standardizing communication across various tracking protocols has significantly reduced onboarding times and integration complexities.
- **Improved Compliance & Safety:**
  Real-time reconstruction of asset trips and automated alerting improves safety, ensuring timely intervention in case of violations or anomalies.
- **Actionable Insights:**
  The platform provides a centralized dashboard with actionable insights, enabling logistics teams to optimize asset utilization and ensure adherence to regulatory standards.
