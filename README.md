Experiment Overview
Goal: Compare performance of Matrix Product State (MPS) models under different feature-map configurations.
Datasets:
MNIST
FashionMNIST
Input preprocessing:
Images resized from 28×28 → 14×14
Flattened into vectors of size 196
Output: 10-class classification
TorchMPS Model Details
TorchMPS is a PyTorch-based implementation of Matrix Product State (MPS) models for machine learning.
It represents inputs as a chain of local feature vectors and contracts them through a tensor network.
Key parameters used:
Number of training data was 1000 and test data 500 throughout the experiments

input_dim: Number of input sites (196)
output_dim: Number of classes (10)
bond_dim: Controls model capacity (higher = more expressive)
feature_dim: Size of local feature embedding
adaptive_mode=False: Fixed bond dimension
periodic_bc=False: Open boundary MPS
