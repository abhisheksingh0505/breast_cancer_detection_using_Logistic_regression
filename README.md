
# 🧠 Logistic Regression Binary Classification - Breast Cancer Detection

This project demonstrates a complete step-by-step binary classification workflow using **Logistic Regression** on the **Breast Cancer Wisconsin (Diagnostic)** dataset.

---

## 📁 Dataset

- **Source**: `data.csv` (Breast Cancer Wisconsin Diagnostic Dataset)
- **Target Variable**: `diagnosis`
  - `M`: Malignant (cancerous) → encoded as `1`
  - `B`: Benign (non-cancerous) → encoded as `0`

---

## 📊 Steps Followed

### ✅ 1. Load & Prepare Dataset
- Dropped irrelevant columns (`id`, `Unnamed: 32`)
- Encoded target (`diagnosis`) using Label Encoding

### ✅ 2. Train/Test Split & Standardization
- Used `train_test_split()` with 80/20 split
- Standardized features using `StandardScaler`

### ✅ 3. Train Logistic Regression Model
- Model: `LogisticRegression()` from `scikit-learn`
- Trained on standardized training data

### ✅ 4. Evaluate the Model
- **Confusion Matrix**
- **Precision**, **Recall**, **ROC-AUC**
- **ROC Curve** visualization

### ✅ 5. Tune Threshold & Explain Sigmoid
- Identified optimal threshold using **Youden’s J statistic**
- Plotted the **sigmoid function** for interpretability

---

## 📈 Model Performance Metrics

| Metric     | Value |
|------------|-------|
| Precision  | 0.97 |
| Recall     | 0.93 |
| ROC-AUC    | 1.00 |

_Values depend on execution output._

---

## 📦 Requirements

Install dependencies using pip:

```bash
pip install pandas scikit-learn matplotlib
