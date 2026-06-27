# MNIST Digit Recognition - Neural Network from Scratch

A neural network built entirely from scratch using only **NumPy**. Every forward pass, backpropagation step, and gradient update is implemented manually to demonstrate a deep understanding of how neural networks actually work under the hood.

## Why Build from Scratch?

Most machine learning courses teach you to call `model.fit()`. This project goes deeper by implementing the mathematics behind neural networks to truly understand what happens during training.

## Results

| Metric | Value |
|---|---|
| Dataset | MNIST (70,000 handwritten digit images) |
| Architecture | 784 -> 128 -> 64 -> 10 |
| Final Test Accuracy | 97%+ |
| Hardest digit pairs | 5/3, 5/8, 4/9 |

## Tech Stack

- **Language:** Python
- **Libraries:** NumPy only (no ML frameworks)
- **Visualisation:** Matplotlib

## What is Implemented from Scratch

| Component | Description |
|---|---|
| Forward pass | Matrix multiplications through each layer |
| Activation functions | ReLU (hidden layers), Softmax (output layer) |
| Loss function | Cross-entropy loss |
| Backpropagation | Full gradient computation through all layers |
| Optimiser | Stochastic Gradient Descent with mini-batches |
| Regularisation | L2 weight decay to prevent overfitting |
| Hyperparameter search | Systematic search on a data subset before full training |

## Key Insights

- Data leakage prevention: normalisation statistics computed on training set only, then applied to test set
- Shorter, wider networks generalised better than deep narrow ones on this dataset
- Per-digit accuracy analysis revealed that visually similar digits (5/3, 5/8, 4/9) are the hardest to distinguish
- Mini-batch SGD converged significantly faster than full-batch gradient descent

## Getting Started

**1. Clone the repository**
```bash
git clone git@github.com:claudia-moliner/neural-network-from-scratch.git
cd neural-network-from-scratch
```

**2. Install dependencies**
```bash
pip install -r requirements.txt
```

**3. Run the notebook**
```bash
jupyter notebook notebooks/mnist_neural_network.ipynb
```

## Author

**Claudia Moliner** - Data Analyst
[GitHub](https://github.com/claudia-moliner) · [Email](mailto:cmolinercalvet@gmail.com)
