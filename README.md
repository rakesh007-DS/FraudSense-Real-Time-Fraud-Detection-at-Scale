# FraudSense — Real-Time Fraud Detection at Scale

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat-square)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange?style=flat-square)
![Streamlit](https://img.shields.io/badge/Streamlit-App-red?style=flat-square)
![Status](https://img.shields.io/badge/Status-Live-brightgreen?style=flat-square)

> Trained on 6.3M+ real-world bank transactions. 98% accuracy. Zero code required to use.

![Dashboard Preview](Fraud_Detection.png)

---

## What It Does

FraudSense is a machine learning system that detects fraudulent bank transactions in real time. Trained on a highly imbalanced dataset of over 6.3 million transactions, it identifies fraud patterns with 98% accuracy - and deploys as a no-code Streamlit web app so any analyst can run live predictions without writing a single line of code.

---

## Key Results

| Metric | Result |
|---|---|
| Training dataset | 6.3M+ transactions |
| Model accuracy | 98% |
| Highest-risk types | TRANSFER, CASHOUT |
| Investigation time | Reduced from hours to seconds |

---

## Project Structure

```
FraudSense/
├── Data_Analysis.ipynb                   # EDA, feature engineering & model training
├── fraud_detection.py                    # Streamlit app — real-time prediction UI
├── fraud_detection_model_pipeline.pk2    # Trained Random Forest pipeline (serialized)
├── Fraud_Detection.png                   # Dashboard preview / result visualization
└── README.md
```

---

## How It Works

1. **Explore** — `Data_Analysis.ipynb` walks through EDA, feature importance, and model training on 6.3M+ transactions
2. **Model** — Random Forest classifier serialized as `fraud_detection_model_pipeline.pk2`
3. **Predict** — `fraud_detection.py` loads the pipeline and serves real-time predictions via Streamlit
4. **Insight** — TRANSFER and CASHOUT flagged as highest-risk transaction types through feature importance analysis

---

## Run Locally

```bash
git clone https://github.com/rakeshpallepogu/fraudsense
cd fraudsense
pip install -r requirements.txt
streamlit run fraud_detection.py
```

---

## Tech Stack

- **Language:** Python
- **ML:** scikit-learn · Random Forest
- **Data:** Pandas · NumPy
- **App:** Streamlit
- **Model Serialization:** Pickle (`.pk2`)

---

## Author

**Rakesh Pallepogu**
[LinkedIn](https://www.linkedin.com/in/rakeshpallepogu/) · [GitHub](https://github.com/rakeshpallepogu)
