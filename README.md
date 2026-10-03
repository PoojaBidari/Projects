# Projects Portfolio

This repository contains a collection of machine learning, deep learning, and AI-focused projects covering time-series analysis, natural language processing, and fundamental concepts in recurrent neural networks. Each project is implemented as a standalone notebook and serves as a learning and experimentation workspace.

---

## Repository Overview

This portfolio includes the following projects:

- ECG Anomaly Detection using Attention-based Bi-GRU Autoencoder
- Template-Based NLP
- Vanishing Gradient Problem in RNN

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

## 2. Template-Based NLP

This project explores template-based natural language processing techniques for structured text understanding and generation. It demonstrates how rules, patterns, and predefined templates can be used to process language-based tasks in a controlled and interpretable way.

### Highlights
- Rule-based NLP approach
- Template-driven text processing
- Simple structured language interpretation
- Useful for deterministic workflows and lightweight NLP systems

Template-based NLP is particularly useful when interpretability, control, and low computational cost are important.

---

## 3. Vanishing Gradient Problem in RNN

This project investigates one of the major challenges in recurrent neural networks: the vanishing gradient problem. It explains why training deep or long-sequence RNNs becomes difficult and how this issue impacts learning over time.

### Topics Covered
- Why gradients vanish in sequential models
- Effect on long-term dependencies
- Limitations of standard RNNs
- Alternative architectures such as LSTMs and GRUs
- Practical strategies for improved training

This notebook is a valuable resource for understanding the behavior of sequence models and the motivation behind modern recurrent architectures.

---

## Tech Stack

This repository primarily uses:

- Python
- Jupyter Notebook
- PyTorch
- NumPy
- Pandas
- Matplotlib
- scikit-learn
- Captum (for explainability in ECG project)
