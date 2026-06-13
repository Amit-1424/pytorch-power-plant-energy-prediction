# Power Plant Energy Prediction using ANN (PyTorch)

## Project Overview

This project uses an Artificial Neural Network (ANN) built with PyTorch to predict the electrical energy output (PE) of a power plant based on environmental conditions.

The model is trained on features like:

* Temperature (AT)
* Exhaust Vacuum (V)
* Ambient Pressure (AP)
* Relative Humidity (RH)

This is a regression problem where the goal is to predict continuous numerical values.

---

## Technologies Used

* Python
* PyTorch
* NumPy
* Pandas
* Matplotlib
* Scikit-learn

---

## Workflow

1. Load and preprocess dataset
2. Split data into training and testing sets
3. Standardize input features
4. Convert data into PyTorch tensors
5. Create TensorDataset and DataLoader
6. Build ANN model using `nn.Sequential`
7. Train model using mini-batch gradient descent
8. Validate model during training
9. Save best model using validation loss
10. Evaluate using MSE Loss and R² Score

---

## ANN Architecture

Input Layer → 6 Neurons → ReLU
Hidden Layer → 6 Neurons → ReLU
Output Layer → 1 Neuron

---

## Loss Function and Optimizer

* Loss Function: Mean Squared Error (MSELoss)
* Optimizer: Adam

---

## Features Implemented

* Data preprocessing
* Feature scaling using StandardScaler
* Tensor conversion
* Mini-batch training using DataLoader
* Validation loss tracking
* Best model checkpoint saving
* Training vs Validation loss visualization
* R² score evaluation

---

## Results

The model successfully predicts power plant energy output with low MSE loss and good regression performance.

---

## Future Improvements

* Add dropout layers
* Experiment with deeper architectures
* Add learning rate scheduling
* Hyperparameter tuning
* Deploy using Streamlit or Flask

---

## How to Run

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the notebook or Python file.

---

## Dataset

Dataset used: Combined Cycle Power Plant Dataset

---
