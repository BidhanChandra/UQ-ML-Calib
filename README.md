# UQ-ML-Calib

## Enhancing Uncertainty Quantification in Molecular Machine Learning

This repository contains code and data for the paper:
**"Enhancing Uncertainty Quantification in Molecular Machine Learning: A Comparative Study of Deep Evidential Regression and Ensembles, with Post-Hoc Calibration."**

The repository is structured into two folders, each corresponding to a specific uncertainty quantification (UQ) approach used in the study.

---

## Directory Structure

### 1. `EGNN-DER_QM9/` – Deep Evidential Regression for UQ on QM9
This directory contains code for training an **E(n)-equivariant Graph Neural Network (EGNN)** with **Deep Evidential Regression (DER)** to estimate uncertainty in predicting electronic spatial extent on the **QM9 dataset**. It also includes scripts for post-hoc calibration and analysis.

#### **Files:**
- `DER_EGNN_QM9_0.01.ipynb` – Trains the EGNN-DER model on the QM9 dataset and generates uncertainty estimates. Outputs:
  - `DER_QM9_val_0.01.npz` – Contains target values, predicted values, aleatoric and epistemic uncertainty, and total uncertainty for the validation dataset.
  - `DER_QM9_test_0.01.npz` – Same as above, but for the test dataset.
- `QM9_DER_analysis.ipynb` – Performs **post-hoc calibration** and **data analysis** on the DER predictions.


---


