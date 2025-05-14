# System Threat Forecaster
## 🛡️ Malware Detection with Telemetry Data

This project uses machine learning to predict if a Windows machine is infected by malware, based on anonymized system telemetry from antivirus logs.

### 📌 Problem

Given system properties (hardware, OS, AV config, etc.), predict the likelihood of malware infection (`target` = 1 if infected, else 0).

### ⚙️ Tech Stack

* Python 3.9+
* `pandas`, `numpy`, `scikit-learn`, `xgboost`, `lightgbm`, `matplotlib`, `seaborn`

### 🚧 Limitations

* Uses only built-in or open-source libraries.
* No deep learning frameworks (like PyTorch or TensorFlow).
* Dataset anonymized—some columns (e.g. `AntivirusConfigID`) lack real-world interpretability.
* Model trained on provided data only (no external augmentation).

### 📊 Output

Binary classification with metrics like accuracy, AUC, precision, recall.
