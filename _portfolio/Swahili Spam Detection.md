---
title: "Swahili SMS Spam Detection."
excerpt: "NLP-powered system to detect Mobile Money scams targeting East African users by analyzing SMS messages written in a mix of Swahili and informal or misspelled English — a common linguistic pattern in the region"
collection: portfolio
---

## Swahili SMS Spam Detection System

This project focuses on detecting Mobile Money scams in East African SMS messages that combine Swahili with informal or misspelled English — a linguistic blend common in real-world communications.

## 🔍 Problem Statement

SMS scams in East Africa often target victims via Mobile Money fraud. These messages are not only written in Swahili but frequently include English words with informal or misspelled phrasing, making traditional spam classifiers less effective.

## 💡 Solution Overview

- Built a spam detection system using **BERT-based embeddings** to understand the semantic context of mixed-language messages.
- Developed a FastAPI web service for serving predictions in real time.
- Leveraged **LLMs** including **GPT, LLaMA, Gemma, and Qwen** for:
  - Zero-shot classification
  - Model explainability
  - Topic modeling to uncover common scam themes
- Implemented **MLOps with DVC** to version control datasets, models, and experiments.
- Tracked experiments with **MLFlow**.

## 🛠️ Tech Stack

- Python, FastAPI
- BERT (LaBSE)
- GPT, LLaMA, Gemma, Qwen
- DVC for experiment tracking and reproducibility

## 🚀 Key Outcomes

- Successfully detected scam patterns in highly code-mixed text messages
- Demonstrated zero-shot capabilities using multiple LLMs for both classification and interpretability
- Ensured reproducibility with end-to-end MLOps practices

## 📂 GitHub Repository

[Access it here](https://github.com/kennethmugo/Swahili-SMS-Spam-Detection)
