# EEG Resting-State Classification

This project demonstrates how to classify EEG signals (eyes open vs. eyes closed) using covariance-based methods and traditional machine learning classifiers.

## Dataset
We use the **AlphaWaves** dataset, which contains EEG recordings from multiple subjects under resting-state conditions:
- **Condition 0**: Eyes Open
- **Condition 1**: Eyes Closed

## Project Structure:
- Data Loading: Fetches EEG signals and labels from AlphaWaves.
- Visualization: Plots sample EEG signals.
- Feature Extraction: Uses covariance matrices as features (pyriemann).
- Classification:
  - Minimum Distance to Mean (MDM)
  - Support Vector Machine (SVM)
  - Random Forest
  - Logistic Regression
- Cross-Validation:
  - Overall classification accuracy with 5-fold CV
  - Subject-wise performance analysis

## Results
- MDM (Riemannian classifier) typically outperforms standard classifiers.
- Subject-wise results shows signs of variability, highlighting possibe inter-individual EEG differences.
