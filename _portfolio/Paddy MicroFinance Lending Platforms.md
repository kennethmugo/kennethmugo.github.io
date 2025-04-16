---
title: "Paddy Micro Finance Lending Platforms"
excerpt: "End-to-End Digital Lending & Intelligence Platform<br/><img src='/images/pesapata.png'><img src='/images/scoppe.png'><img src='/images/okoamia.jpg'>"
collection: portfolio
---

## Overview

This project modernized and unified the lending operations for Paddy Micro Finance by migrating legacy lending platforms (Okoa Mia and Pesapata) to Azure Cloud and developing new systems (Pesapata v3 and Scoppe). The integrated platform not only powers peer-to-peer lending and unsecured loans but also drives intelligent, data-driven credit risk assessment, fraud prevention, and dynamic loan pricing. The entire ecosystem is built on a robust microservices architecture with end-to-end integrations and real-time decision-making capabilities.

## Technical Architecture

### Legacy System Migration & Modernization

- **Cloud Migration:**
  Migrated legacy platforms (Okoa Mia and Pesapata) from on-premises to Azure Cloud, enabling scalability from under 100K to over 1M users and supporting KES 60M+ in monthly loans.
- **USSD & API Transitions:**
  Led the transition of USSD and backend APIs, ensuring seamless integration with new cloud services.
- **CI/CD & Containerization:**
  Implemented CI/CD pipelines and deployed containerized applications using Azure Container Apps for seamless, reliable deployments.

### Next-Generation Lending Platforms

- **Pesapata v3 (Peer-to-Peer Lending):**
  Designed a microservices-based platform in .NET applying SOLID principles to engineer ACID-compliant digital wallets and flexible loan issuance. This solution addressed issues such as duplicate lender identities tied to phone numbers, enabling personalized, risk-based lending.
- **Scoppe (Traditional Unsecured Lending):**
  Engineered a scalable backend system for one of Kenya’s pioneering digital lending apps, facilitating millions in loans and growing the user base from zero to 100K+.

### Intelligence & Data-Driven Decision Making

- **Credit Scoring Engine:**
  Developed a real-time credit scoring model using XGBoost combined with K-Means clustering, leveraging alternative credit data to perform borrower segmentation and dynamic risk assessment. This model enabled personalized loan offers and dynamic credit limits, achieving repayment rates between 88% and 93%.
- **Low-Latency Data Pipeline:**
  Designed a data ingestion pipeline optimized with Azure Front Door PoP nodes, reducing upload failures by 80% and enabling real-time analytics via Power BI. This allowed Okoa Mia to refine risk models and raise loan limits 19x, driving several-fold revenue increases.
- **Model Monitoring & Notification:**
  Established a real-time monitoring system using Azure Machine Learning to track model drift and trigger automated retraining, along with an A/B-tested notification system for repayment reminders and delinquency alerts.

### Cross-Platform Integration & Infrastructure Security

- **Unified Configuration & Security:**
  Utilized Azure App Configuration for centralized configuration management, feature flags for controlled feature rollouts, and Azure Key Vault for securing sensitive information such as authentication keys.
- **Inter-Platform Communication:**
  Enabled seamless communication between platforms via gRPC, ensuring a consistent and reliable data flow.
- **Database & Data Consistency:**
  Employed Azure SQL to guarantee ACID compliance for all transaction and loan-related operations.

## Business Impact

- **Scalability & Growth:**
  Successfully scaled lending platforms to over 1M users while processing millions in loans monthly, driving substantial revenue growth and attracting significant investment from tier 1 financial institutions.
- **Operational Efficiency:**
  Reduced loan issuance times from over 5 minutes to seconds, eliminated USSD timeouts, and automated manual processes through event-driven architectures, resulting in streamlined operations and improved user experience.
- **Risk Management & Fraud Prevention:**
  Enabled sophisticated, data-driven credit risk assessment and fraud detection that led to better risk models, dynamic credit limits, and enhanced regulatory compliance—all of which reduced default rates and increased lender profitability.
