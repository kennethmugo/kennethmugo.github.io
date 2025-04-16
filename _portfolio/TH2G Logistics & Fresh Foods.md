---
title: "TH2G Logistics & Fresh Foods – IoT Data Pipeline & Digital Twin Project"
excerpt: "Developed logistics & IoT apps for real-time container tracking, sensor monitoring, and diagnostics for Makupa Transit, contributing to innovative technical solutions.<br/><img src='/images/th2g.png'><img src='/images/th2g_ff.png'>"
collection: portfolio
---

## Overview

This project was focused on developing a robust IoT solution for real-time tracking and monitoring of shipping containers. The solution not only ensured granular telemetry for asset management but also directly enabled a new revenue stream by facilitating the launch of TH2G Fresh Foods, a fish-selling business generating over KES 100K daily. The project combined advanced backend engineering with innovative IoT and cloud-native technologies.

## Technical Approach

- **Real-Time IoT Data Ingestion:**
  - Built an IoT data pipeline using **Azure IoT Hub** to aggregate sensor data from BLE-enabled container controllers.
  - Utilized **MQTT** for efficient, low-latency communication, with device authentication secured via **TPM**.

- **Digital Twin System:**

  - Designed and implemented a digital twin system using [**Microsoft Orleans Virtual Actors**](https://learn.microsoft.com/en-us/dotnet/orleans/overview).
  - Each container was modeled as an independent virtual actor, enabling scalable, real-time data processing while optimizing cloud compute costs.

- **Backend API:**
  - Developed a GraphQL endpoint to serve real-time data from the IoT pipeline and digital twin system.

- **Cloud Data Processing & Dashboarding:**

  - Optimized cloud data ingestion to feed a centralized dashboard, providing real-time logistics insights.
  - This dashboard allowed for actionable decision-making and early detection of operational issues.

## Implementation Details

- **Sensor Data:**
  - Monitored key parameters including temperature, humidity, weight, location, internal imaging, and door activity.
- **Communication & Security:**
  - Employed **MQTT** for data transmission and **TPM** for securing device authentication.
- **Digital Twin & Processing**
  - Leveraged **Microsoft Orleans** to create virtual representations of each container, facilitating high-throughput processing.
- **Scalable Architecture:**
  - Designed the solution for deployment on Azure, ensuring both scalability and cost-efficiency.

## Business Impact

- **Enhanced Operational Visibility:**
  - Real-time monitoring enabled proactive management of container conditions, reducing downtime and improving asset utilization.
- **Revenue Generation:**
  - The data-driven approach directly contributed to the launch of TH2G Fresh Foods ([@TH2G_FreshFoods](https://www.instagram.com/th2g_freshfoods.ke/)), generating over **KES 100K+ in daily sales** as an additional revenue stream.
- **Scalability & Reliability:**
  - The digital twin system and optimized data pipeline significantly lowered operating costs, ensuring reliable asset tracking across diverse and resource-constrained environments.
