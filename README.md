# PCAP Analyzer

A Python-based **network security and traffic analysis tool** that analyzes Packet Capture (PCAP) files and applies machine learning to classify network traffic as **normal or anomalous**.

The project combines **Scapy, PyShark, feature extraction, and a trained Random Forest classifier** to support PCAP analysis, anomaly detection, and network security investigation.

---

## 🔎 Overview

PCAP Analyzer is designed to help analyze captured network traffic and identify potentially suspicious or anomalous activity.

The tool processes PCAP files, extracts relevant network traffic information, generates features for analysis, and uses a pre-trained machine learning model to classify traffic.

This project demonstrates practical application of:

- Network traffic analysis
- PCAP analysis
- Feature extraction
- Machine learning for security
- Anomaly detection
- Network security investigation

---

## 🚀 Key Features

### 📡 PCAP File Parsing
Extracts relevant network traffic information from PCAP files for further analysis.

### 🔍 Feature Extraction
Generates traffic-related features such as source/destination information, packet characteristics, and other network metrics used for analysis and classification.

### 🧠 Machine Learning Detection
Uses a trained **Random Forest classifier** to classify network traffic as normal or anomalous.

### 🚨 Anomaly Detection
Analyzes new network traffic and identifies potentially suspicious activity based on the trained model.

### 📊 Model Evaluation
Supports evaluation of the machine learning model using classification performance metrics such as:

- Accuracy
- Precision
- Recall

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| **Python** | Core development |
| **Scapy** | Packet analysis and network traffic processing |
| **PyShark** | PCAP and packet analysis |
| **Pandas** | Data processing and analysis |
| **NumPy** | Numerical processing |
| **Scikit-learn** | Machine learning |
| **Joblib** | Model persistence |
| **PCAP** | Network traffic data |

---

## 🧠 Machine Learning Workflow

```text
              PCAP File
                  │
                  ▼
          Packet / Traffic Parsing
                  │
                  ▼
           Feature Extraction
                  │
                  ▼
           Data Preprocessing
                  │
                  ▼
        Random Forest Classifier
                  │
                  ▼
       ┌──────────┴──────────┐
       │                     │
     Normal              Anomalous
       │                     │
       └──────────┬──────────┘
                  ▼
          Security Analysis
