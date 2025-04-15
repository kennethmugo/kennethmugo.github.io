---
title: "Falu Identity – Identity Verification"
excerpt: "AI-Powered Identity Verification & Fraud Prevention Platform<br/><img src='/images/falu.png'>"
collection: portfolio
---

## Overview

Falu Identity is an AI-powered platform that streamlines identity verification and enhances fraud prevention across diverse document types. Designed for environments with limited connectivity, the system delivers rapid, accurate verifications—processing 50,000+ secure validations—while also integrating advanced biometric and tax ID checks to ensure regulatory compliance and prevent duplicate identities.

## Technical Approach

- **Document Detection & Optimization:**
  Developed a real-time identity document detection model using SSDLite, optimized for mobile via INT8 quantization (across TFLite, TF.js, CoreML with palettization, and ONNX) to reduce the model size to under 3MB. Deployed via Azure CDN for fast, scalable access.

- **Identity Validation Pipeline:**
  Built a FastAPI-powered pipeline that leverages transfer learning with EfficientNetB0 for document classification and integrates OCR-based MRZ checks for tampering detection. This method minimizes data requirements, speeds up development, and achieves 98% classification accuracy—ensuring rapid, reliable verification.

- **Tax ID Verification:**
  Engineered an automated tax ID verification solution for Kenyan clients by using Puppeteer to simulate browser interactions on the [KRA portal](https://itax.kra.go.ke/KRA-Portal/pinChecker.htm). The system inputs tax IDs, employs OCR to extract and solve an algorithmic puzzle that unlocks taxpayer details, which are then cross-validated against identity documents to ensure compliance and prevent fraud.

- **Active Learning for Continuous Improvement:**
  Led the development of a model-driven active learning pipeline that automatically flags uncertain predictions for further labeling and retraining, reducing manual annotation by 90% and adapting to evolving document formats.

- **Data Enrichment for Fraud Detection:**
  Developed a Random Forest model with n-gram TF-IDF features to infer missing gender details in a 15M+ dataset (with over 90% unlabeled), transforming incomplete data into a structured, high-quality dataset for stricter cross-validation of identity documents—significantly enhancing fraud detection.

- **Face Verification Pipeline:**
  Built a multi-stage face verification pipeline utilizing [MediaPipe’s FaceLandmarker models](https://ai.google.dev/edge/mediapipe/solutions/vision/face_landmarker) to extract facial landmarks and a custom SVR model for head pose estimation. Integrated MediaPipe Blendshape for expression validation to improve matching accuracy and ensure compliance with global identity verification standards.

- **AI-Powered Fraud Detection:**
  Developed a system using FaceNet embeddings and MongoDB Atlas Vector Search to detect duplicate accounts. The solution leverages submitted selfies for cross-document identity matching via Approximate Nearest Neighbors search, effectively preventing fraud and bolstering platform security.

## Business Impact

- Enabled 50,000+ secure identity verifications in challenging environments.
- Achieved 98% accuracy in document validation, significantly reducing fraud.
- Reduced manual labeling efforts by 90% with active learning.
- Enhanced regulatory compliance and streamlined onboarding through automated tax ID checks.
- Delivered a comprehensive, scalable system combining biometric verification and document analysis to build trust and mitigate risk.
