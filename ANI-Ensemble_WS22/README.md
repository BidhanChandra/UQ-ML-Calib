# Uncertainty Quantification (UQ) with Ensemble of ANI Models on WS22 Dataset

## Overview

This directory contains code and trained models for uncertainty quantification (UQ) using an ensemble of ANI models on the WS22 dataset. The focus is on estimating uncertainty in energy and force predictions for acrolein, considering different geometric configurations.

## Folder Structure

### **ANI_ensemble_Force/**

- **DE1/** to **DE8/**: Each folder contains a trained ANI model and corresponding predictions.

#### Files in each subfolder:

- **ani_acrolein.pt** – Trained model for the specific ensemble member.
- **cis.npz** – Predicted energies and forces for cis isomer.
- **cis_trans.npz** – Predicted energies and forces for cis-trans isomer.
- **test.npz** – Predicted energies and forces for test data.
- **train.npz** – Predicted energies and forces for training data.
- **For_Acrolein_ANI#.ipynb** - The notebook to train the model.

## Usage

1. Each ensemble model (**DE1** to **DE8**) has been trained separately. The corresponding training notebooks are available in their respective folders.
2. The trained models can be used to predict energies and forces for different geometric configurations of acrolein.
3. The dataset used in this study, **ws22_acrolein.npz**, can be downloaded from [Zenodo](https://zenodo.org/records/7032334).
4. To analyze the results and perform post-hoc calibration of the predicted uncertainties for energies and forces, open and run **DE_Acrolein_analysis.ipynb**.
