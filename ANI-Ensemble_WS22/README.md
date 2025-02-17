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
1. Extract `ANI_ensemble_Force.zip` into the current directory.
2. Each ensemble model (DE1 to DE8) is trained separately. The corresponding training notebooks are included in the respective folders.
3. Use the trained models to predict energy and forces for different geometric configurations.
