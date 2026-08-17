 # FedSHAP-IDS
**Paper:** FedSHAP-IDS: Privacy-Preserving IoT Intrusion Detection 
via Federated Ensemble Learning with Server-Side SHAP Matrix Aggregation

**Submitted to:** IEEE Access

## Requirements
- Python 3.10+
- lightgbm
- shap
- scikit-learn
- pandas, numpy, scipy

## Datasets
- CICIoT2023: https://www.kaggle.com/datasets/ciciot2023
- UNSW-NB15: https://www.kaggle.com/datasets/mrwellsdavid/unsw-nb15

## How to Run
1. Open FedSHAP_IDS.ipynb in Kaggle or Jupyter
2. Attach both datasets
3. Run all cells sequentially

## Results
| Dataset    | Accuracy | F1-Macro | AUC-ROC |
|------------|----------|----------|---------|
| CICIoT2023 | 0.9826   | 0.6452   | 0.9056  |
| UNSW-NB15  | 0.7264   | 0.4071   | 0.9067  |
