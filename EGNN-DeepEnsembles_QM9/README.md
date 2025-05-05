# EGNN-DeepEnsembles_QM9

## Overview

This directory contains code, trained models, and data for training an E(n)-equivariant Graph Neural Network (EGNN) using a Deep Ensemble strategy to estimate uncertainty in predicting electronic spatial extent on the QM9 dataset. The ensemble consists of 8 independently trained EGNN models. It also includes scripts for analysis and evaluation of uncertainty estimates.

## Directory Structure

### `notebooks/`
Contains training notebooks for each ensemble member:

- `DE_EGNN_1.ipynb` to `DE_EGNN_8.ipynb`  
  Each notebook trains one EGNN model using a different hyperparameters
### `models/`
Contains the saved PyTorch model checkpoints:

- `trained_egnn_DE1.pth` to `trained_egnn_DE8.pth`  
  These files store the weights of the trained EGNN models corresponding to each ensemble member.

### `dataset/`
Contains the prediction results and targets:

- `predictions_and_targets_DE1.npz` to `predictions_and_targets_DE8.npz`  
  Each `.npz` file includes:
  - Ground-truth values
  - Predicted values for training, validation and test dataset

## Additional Notebooks

- `Deep_Ensembles_QM9_analysis.ipynb`  
  Performs the unceratinty quantification along with recalibration
