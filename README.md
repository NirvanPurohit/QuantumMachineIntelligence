
# Quantum Machine Intelligence for Financial Fraud Detection

This repository contains the code and methodology for a research project on **Quantum Machine Intelligence applied to Financial Fraud Detection**, conducted from **November 2024 to May 2025**.

## Overview

The project explores the use of **hybrid quantum-classical models** for detecting financial fraud, focusing on:

- **Variational Quantum Classifiers (VQC)** implemented using IBM Qiskit.
- **Custom Variational Quantum Circuits** using RY/RZ rotations and full entanglement on Amazon Braket simulators.

## Key Contributions

- Developed a quantum-classical fraud detection pipeline.
- Engineered a custom quantum circuit optimized with **COBYLA**.
- Conducted comparative analysis with classical models (Logistic Regression, SVC, Random Forest, MLP).
- Achieved competitive performance with the custom quantum circuit on simulators.

## Technologies Used

- **Qiskit** – for implementing VQC models.
- **Amazon Braket SDK** – for custom circuit design and simulation.
- **Python (Scikit-learn, NumPy, Pandas)** – for data preprocessing and classical baselines.

## Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/your-username/quantum-fraud-detection.git
    cd quantum-fraud-detection
    ```

2. Create a virtual environment and install dependencies:
    ```bash
    python -m venv qml-env
    source qml-env/bin/activate  # On Windows: qml-env\Scripts\activate
    pip install -r requirements.txt
    ```

## Dataset

Credit card fraud dataset from [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) containing 284,807 transactions.

## Project Structure

- `data/` – Contains the preprocessed and raw dataset.
- `quantum/` – Contains Qiskit and Braket implementations.
- `classical/` – Contains classical ML models for benchmarking.
- `notebooks/` – Jupyter notebooks demonstrating preprocessing and analysis.

## Results

| Model               | Accuracy | Precision | F1-Score | ROC-AUC |
|--------------------|----------|-----------|----------|---------|
| Custom Quantum     | 88.7%    | 88%       | 89%      | 91%     |
| VQC (Qiskit)       | 82%      | 100%      | 79%      | 83%     |
| Random Forest      | 96%      | 98%       | 96%      | 97%     |
| MLP                | 95%      | 98%       | 95%      | 96%     |

