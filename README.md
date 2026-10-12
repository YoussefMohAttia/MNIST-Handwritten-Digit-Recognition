<div align="center">

# MNIST Handwritten Digit Recognition

### Deep Learning Experiments for Classifying 28 x 28 Handwritten Digits

[![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-EE4C2C?logo=pytorch&logoColor=white)](https://pytorch.org/)

</div>

## Overview

This project trains and evaluates neural-network classifiers on the MNIST handwritten-digit dataset. The main notebook reads the included IDX image and label files, prepares train/validation data, trains models with PyTorch, and reports classification results with visual diagnostics.

## What Is Included

- GPU-aware PyTorch workflow that falls back to CPU when CUDA is unavailable
- Neural-network training and evaluation for digits `0` through `9`
- Confusion matrix and classification-report analysis
- The original MNIST IDX data files used by the notebook
- Reproducible dataset-backed experiment in a single notebook

## Repository Structure

```text
.
├── notebook_GPU.ipynb                # Training and evaluation workflow
├── train-images.idx3-ubyte           # MNIST training images
├── train-labels.idx1-ubyte           # MNIST training labels
├── t10k-images.idx3-ubyte            # MNIST test images
├── t10k-labels.idx1-ubyte            # MNIST test labels
└── README.md
```

## Getting Started

```bash
python -m venv .venv
source .venv/bin/activate
pip install jupyter numpy idx2numpy scikit-learn matplotlib seaborn torch
jupyter notebook notebook_GPU.ipynb
```

In Windows PowerShell, activate with `.\.venv\Scripts\Activate.ps1`.

Keep the IDX files in the repository root when running the notebook, since it loads them using relative paths.

## Author

**Youssef Mohamed Attia**  
[GitHub](https://github.com/YoussefMohAttia) · [LinkedIn](https://www.linkedin.com/in/youssefmohattia/)
