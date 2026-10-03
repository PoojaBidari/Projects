```markdown
# ECG Anomaly Detection using Attention-based Bi-GRU Autoencoder

This project implements an advanced deep learning framework for electrocardiogram (ECG) anomaly detection on the benchmark **ECG5000** dataset. It leverages an **Attention-guided Bidirectional Gated Recurrent Unit (Bi-GRU) Autoencoder** to capture temporal dynamics in physiological signals and uses modern XAI (Explainable AI) techniques to provide feature-level and step-level attribution.

## 🚀 Features
- **Semi-Supervised Learning**: Trained strictly on normal ECG signals, enabling the network to learn the underlying manifold of healthy cardiac behavior.
- **Bidirectional GRU Architecture**: Processes sequence inputs in both forward and backward directions to robustly learn temporal structures.
- **Global Attention Mechanism**: Dynamically focuses on critical temporal intervals within the heartbeat cycle.
- **Explainable AI (XAI)**: Uses **Captum's Integrated Gradients** to provide pixel/timestep-level attribution showing precisely why an ECG segment is classified as an anomaly.
- **Comprehensive Evaluation**: Best classification threshold search targeting $F_1$-score optimization, producing a final accuracy of **95.24%** and $F_1$-score of **94.50%**.

---

## 📊 Dataset
We utilize the **ECG5000** dataset from the UCR Time Series Classification Archive, consisting of 5,000 ECG sequences (length 140) of cardiac cycles:
- **Train Set**: 500 samples
- **Test Set**: 4,500 samples

**Class Mapping:**
- `1` : Normal (Classified as `0` for Autoencoder training)
- `2`, `3`, `4`, `5` : Abnormal/Anomalies (Classified as `1` for evaluation)

---

## 🛠️ Model Architecture
The Autoencoder utilizes an attention bottleneck:
1. **Encoder**: A 2-layer Bidirectional GRU yielding hidden representations across all 140 timesteps.
2. **Attention Layer**: Learns alignment coefficients over temporal states, producing a single weighted context vector.
3. **Latent Representation**: Projects context into a bottleneck vector representing normal heart cycle behavior.
4. **Decoder**: A 2-layer Bidirectional GRU reconstructs the original signal from the latent space sequence.

---

## 📈 Results

Our trained model achieves outstanding detection statistics on the 4,500 test samples:

| Metric | Score |
| :--- | :--- |
| **Accuracy** | **95.24%** |
| **Precision** | **91.17%** |
| **Recall** | **98.08%** |
| **F1-Score** | **94.50%** |

### Interpretability Outcomes
- **Attention Maps**: Highlights that the model heavily prioritizes the QRS complex and the early T-wave of the heartbeat.
- **Integrated Gradients**: Directly demonstrates that anomalous deviations in the S-T segment or the R-peak drive high reconstruction errors and trigger anomaly alarms.
```
