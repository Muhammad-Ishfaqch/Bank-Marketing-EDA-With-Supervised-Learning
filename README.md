#  Bank Marketing EDA with Supervised Learning

A comprehensive exploratory data analysis (EDA) and supervised learning implementation for the **UCI Bank Marketing dataset**, helping to predict whether a bank client will subscribe to a term deposit.

---

##  Project Overview

This repository contains a Jupyter Notebook (`BankMarketing.ipynb`) where the dataset is explored, preprocessed, visualized, and leveraged to train supervised classification models. The goal is to understand feature relationships and build predictive models for customer subscription likelihood.

---

##  Dataset: Bank Marketing (UCI)

The dataset originates from the UCI Machine Learning Repository and pertains to phone-based marketing campaigns conducted by a Portuguese bank between 2008 and 2010 :contentReference[oaicite:0]{index=0}.

- **Instances**: ~41,188 to 45,211 records depending on which version is used :contentReference[oaicite:1]{index=1}.
- **Features**:
  - **Client Data (Demographics & Finance)**:
    - `age`, `job`, `marital`, `education`, `default`, `balance`, `housing`, `loan` :contentReference[oaicite:2]{index=2}.
  - **Campaign-related**:
    - `contact` (cellular/telephone), `day_of_week`, `month`, `duration` (last contact in seconds), `campaign`, `pdays`, `previous`, `poutcome` :contentReference[oaicite:3]{index=3}.
    - Note: `duration` is highly predictive but not realistic for real-time prediction, as it's only known post-call outcome :contentReference[oaicite:4]{index=4}.
  - **Target Variable**:
    - `y`: Indicates whether the client subscribed to a term deposit (“yes”/“no”) :contentReference[oaicite:5]{index=5}.
- **Notes**:
  - Multiple dataset versions exist: full and subset variants for computational efficiency :contentReference[oaicite:6]{index=6}.
  - No missing values in typical versions :contentReference[oaicite:7]{index=7}.
  - The dataset is known to be **imbalanced**, with fewer positive (`yes`) instances :contentReference[oaicite:8]{index=8}.

---

---

##  Notebook Highlights

You can expect the following steps within `BankMarketing.ipynb`:

1. **Data Loading & Overview**
   - Load dataset (e.g., via pandas or `fetch_bank_marketing()` from Fairlearn) :contentReference[oaicite:9]{index=9}.
2. **Preprocessing**
   - Encode categorical features, handle class imbalance, remove or evaluate `duration`.
3. **Exploratory Data Analysis (EDA)**
   - Visualize feature distributions (e.g., age, job), correlation with target, imbalance analysis.
4. **Modeling**
   - Fit models like Logistic Regression, Decision Trees, Random Forests, etc.
   - Evaluate using accuracy, ROC AUC, confusion matrix, precision/recall.
5. **Interpretation**
   - Identify top predictors (e.g., contact duration, month, job type).

---

##  Installation & Usage

### Prerequisites

- Python 3.8+
- Jupyter Notebook

### Setup

```bash
git clone https://github.com/Muhammad-Ishfaqch/Bank-Marketing-EDA-With-Supervised-Learning.git
cd Bank-Marketing-EDA-With-Supervised-Learning


