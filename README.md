# FedSHAP-IDS

**Privacy-Preserving IoT Intrusion Detection via Federated Ensemble Learning with Server-Side SHAP Matrix Aggregation**

**Author:** Utsho Kumar Dey — Dept. of CSE, NUBTK
**Submitted to:** IEEE Access

K=5 IoT edge clients train local LightGBM models on a non-IID (Dirichlet, α=0.5) split. Each client sends only a 180-byte SHAP vector to the server — no raw data ever leaves the client. The server fuses these into one globally consistent feature ranking and prediction.

## Results

| Dataset | Accuracy | F1-Macro | AUC-ROC |
|---|---|---|---|
| CICIoT2023 | 0.9826 | 0.6452 | 0.9056 |
| UNSW-NB15 | 0.7264 | 0.4071 | 0.9067 |

Outperforms a centralized LightGBM baseline on every metric, on both datasets, while transmitting **17× less data** (7.8 MB vs. 133.9 MB).

## Requirements

- Python 3.10+
- lightgbm, shap, scikit-learn
- pandas, numpy, scipy

## Datasets

- CICIoT2023: https://www.kaggle.com/datasets/ciciot2023
- UNSW-NB15: https://www.kaggle.com/datasets/mrwellsdavid/unsw-nb15

## How to Run

1. Open `fedshap-ids.ipynb` in Kaggle or Jupyter
2. Attach both datasets
3. Run all cells sequentially

## Contact

utsho.cse@nubtkhulna.ac.bd
