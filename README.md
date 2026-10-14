# Projects Portfolio

This repository contains a collection of machine learning, deep learning, and AI-focused projects covering time-series analysis, natural language processing, and fundamental concepts in recurrent neural networks. Each project is implemented as a standalone notebook and serves as a learning and experimentation workspace.

---

## Repository Overview

This portfolio includes the following projects:

- ECG Anomaly Detection using Attention-based Bi-GRU Autoencoder


These projects reflect a range of topics in modern AI and data science, from healthcare signal analysis to NLP pipelines and deep learning theory.

---

## 1. ECG Anomaly Detection using Attention-based Bi-GRU Autoencoder

This project focuses on detecting anomalies in ECG signals using a semi-supervised deep learning approach. The model is trained primarily on normal heartbeats and learns the normal structure of ECG sequences. It then identifies abnormal patterns based on reconstruction error.

### Key Features
- Semi-supervised learning using only normal ECG data
- Bidirectional GRU-based autoencoder
- Attention mechanism to focus on important time steps
- Explainable AI using Integrated Gradients
- Performance evaluation on ECG5000 dataset

### Dataset
The project uses the ECG5000 time-series dataset from the UCR Time Series Classification Archive.

### Evaluation
The model is evaluated using standard classification metrics such as:
- Accuracy
- Precision
- Recall
- F1-score

This project demonstrates how deep learning can be applied to health monitoring and anomaly detection in biomedical data.

---


