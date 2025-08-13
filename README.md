IoT Anomaly Detection & Device Identification with Context Awareness
This repository contains the Jupyter Notebook and associated results for my dissertation project on IoT anomaly detection and device identification using the CIC IoT-DIAD 2024 dataset.
The project evaluates multiple Machine Learning and Deep Learning models in two phases:

Anomaly Detection without Context Awareness – Flow-based Anomaly Detection using statistical and temporal features.

Anomaly Detection with Context Awareness – Device identity (from packet-level classification) injected into flow-based anomaly detection.

Device Identification – Predicting the IoT device identity from packet-level features.

Files in This Repository
File Name	Description
Anamolydetectionanddeviceidentification.ipynb	Main Jupyter Notebook with complete code for preprocessing, training, evaluation, and results generation.
1D CNN Confusion Matrix.png	Confusion matrix for 1D CNN – Anomaly Detection without Context Awareness.
1D CNN.png	1D CNN – Anomaly Detection with Context Awareness.
CNN LSTM.png	CNN-LSTM – Anomaly Detection with Context Awareness.
Hybrid CNN LSTM Confusion Matrix.png	Confusion matrix for Hybrid CNN-LSTM – Anomaly Detection without Context Awareness.
LSTM Confusion Matrix.png	Confusion matrix for LSTM – Anomaly Detection without Context Awareness.
LSTM.png	LSTM – Anomaly Detection with Context Awareness.
MLP Confusion Matrix.png	Confusion matrix for MLP – Anomaly Detection without Context Awareness.
MLP.png	MLP – Anomaly Detection with Context Awareness.
RF.png	Random Forest – Device Identification results.
Random Forest Confusion Matrix.png	Confusion matrix for Random Forest – Anomaly Detection without Context Awareness.
XG Boost Confusion Matrix.png	Confusion matrix for XGBoost – Anomaly Detection without Context Awareness.
xgboost.png	XGBoost – Device Identification results.

Dataset
This project uses the CIC IoT-DIAD 2024 dataset provided by the Canadian Institute for Cybersecurity.
The dataset contains packet-based and flow-based files, which are used in different phases:
https://www.unb.ca/cic/datasets/iot-diad-2024.html

Flow-based CSVs → Used for anomaly detection tasks.

Packet-based CSVs → Used for device identification tasks.

📂 Google Drive link to all CSVs used in this project: 
https://drive.google.com/drive/folders/1EnOQKwHTkj6m91qfqFoksvhQJzrF2uwc?usp=sharing

Models Used
Anomaly Detection
Classical ML: Random Forest, XGBoost

Deep Learning: 1D CNN, LSTM, CNN-LSTM, MLP

Device Identification
Classical ML: Random Forest, XGBoost

Results Summary
Device Identification: Achieved up to 99–100% accuracy (macro F1 > 0.90).

Context-Aware Anomaly Detection: Major recall improvements for minority classes:

Mirai: 0.36 → 0.71

Web-based: 0.37 → 0.80

Brute force: 0.22 → 0.84

Edit
jupyter notebook Anamolydetectionanddeviceidentification.ipynb
Make sure you have the dataset CSVs from the Google Drive link and update the file paths in the notebook if needed.
