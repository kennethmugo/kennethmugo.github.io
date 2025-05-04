---
title: "Falu Platform"
excerpt: "Unified Identity, Messaging, and Payments Solution<br/><img src='/images/falu.png'>"
collection: portfolio
---

## Overview

Falu Platform is an integrated, AI-powered solution that streamlines identity verification, fraud prevention, payments, and messaging. Designed for resource-constrained environments, it delivers rapid, secure verifications while processing high-volume financial transactions and facilitating efficient communications. This unified platform has enhanced lender trust, ensured regulatory compliance, and driven revenue growth.

## Falu Identity

**Overview:**
An AI-driven identity verification and fraud detection system designed to process 50,000+ secure verifications by analyzing documents and biometric data.

**Key Contributions:**

- **Document Detection & Optimization:**
  Developed a real-time identity document detection model using SSDLite, optimized for mobile via INT8 quantization (across TFLite, TF.js, CoreML with palettization, and ONNX) to compress the model to under 3MB. Deployed via Azure CDN for fast, scalable access.
- **Identity Validation Pipeline:**
  Built a FastAPI-powered pipeline leveraging transfer learning with EfficientNetB0 for classification and OCR-based MRZ checks, achieving 98% accuracy while minimizing data requirements.
- **Tax ID Verification:**
  Engineered an automated tax ID verification solution for Kenyan clients by using Puppeteer to simulate browser interactions on the [KRA portal](https://itax.kra.go.ke/KRA-Portal/pinChecker.htm). The system inputs tax IDs, employs OCR to extract and solve an algorithmic puzzle that unlocks taxpayer details, which are then cross-validated against identity documents to ensure compliance and prevent fraud.
- **Active Learning:**
  Led the development of a model-driven active learning pipeline that flagged uncertain predictions for automated labeling and retraining, reducing manual annotation by 90%.
- **Data Enrichment:**
  Developed a Random Forest model with n-gram TF-IDF features to infer missing gender details in a 15M+ dataset (with over 90% unlabeled), transforming incomplete data into a structured, high-quality dataset for stricter cross-validation of identity documents—significantly enhancing fraud detection.
- **Face Verification Pipeline:**
  Built a multi-stage face verification pipeline using MediaPipe’s FaceLandmarker models for landmark extraction and a custom SVR (Support Vector Regressor) model for head pose estimation, supplemented by MediaPipe Blendshape for expression validation—enhancing matching accuracy and compliance with global identity standards.
- **Fraud Detection:**
  Developed an AI-powered fraud detection system using FaceNet embeddings and MongoDB Atlas Vector Search to detect duplicate accounts by matching submitted selfies via ANN search, thereby preventing identity fraud.

## Falu Money

**Overview:**
A high-throughput payments gateway that processed over KES 4B+ in transactions, ensuring real-time financial operations and secure monetary transfers.

**Key Contributions:**

- **Payments Gateway:**
  Engineered a robust payments gateway by integrating M-Pesa APIs (Broker and Daraja) and leveraging auto-scaling and asynchronous processing. This allowed for dynamic adaptation to traffic spikes, ensuring reliable processing of high-volume transactions.

## Falu Messaging

**Overview:**
A high-scale messaging system that supports critical communications for financial services, enhancing system efficiency and load management.

**Key Contributions:**

- **Scheduled Messaging:**
  Designed scheduled messaging with Azure Service Bus deferred queues, allowing clients to prepare messages during off-peak periods for seamless dispatch during peak times.
- **Dynamic Templating:**
  Implemented dynamic message templating with Mustachio to reduce server-side payload processing by storing static content on the server and sending only variable data—boosting throughput.
- **Background Ingestion Pipeline:**
  Optimized a high-throughput messaging gateway by implementing a background ingestion pipeline that temporarily stored messages on Azure Files. This approach immediately returned HTTP 202 status responses to clients and deferred batch processing offline, eliminating database timeouts and ensuring seamless delivery of 1M+ daily messages.

## 🧰 SDK Development & Maintenance

- **Falu .NET SDK Maintenance:**
  Actively maintained the official [Falu SDK for .NET](https://github.com/faluapp/falu-dotnet), ensuring robust, developer-friendly integration across all Falu services—including Identity, Messaging, and Money. Provided consistent API abstractions, streamlined authentication, and improved developer experience through thorough documentation and rigorous CI/CD pipelines.

## Business Impact

- Delivered a comprehensive, scalable solution that handles 50,000+ identity verifications and processes KES 4B+ in transactions.
- Streamlined loan origination and credit risk assessment to scale user bases, drive revenue growth, and secure investments.
- Enhanced fraud prevention and regulatory compliance through multi-layered AI-driven validation and automated tax ID verification.
- Enabled efficient business communications and operational visibility that directly contributed to new revenue streams and improved asset utilization.
