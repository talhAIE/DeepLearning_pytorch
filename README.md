# Deep Learning with PyTorch

A practical, notebook-based guide to core PyTorch and deep-learning workflows, from tensors and autograd to CNNs, hyperparameter tuning, and transfer learning.

## Overview

This repository is a hands-on learning collection of Jupyter notebooks. The notebooks build progressively: starting with PyTorch fundamentals, then moving through data pipelines and neural-network training, before applying those ideas to classification tasks with Fashion-MNIST and other datasets.

## Features

- PyTorch tensor operations, GPU usage, reproducibility, and automatic differentiation
- End-to-end model workflow: data preparation, model creation, training, evaluation, and saving/loading
- Custom `Dataset` and `DataLoader` implementations
- ANN and CNN image-classification examples using Fashion-MNIST
- Device-agnostic CPU/GPU training code and overfitting-reduction techniques
- Hyperparameter optimization with Optuna, including Bayesian search
- Transfer learning with a pretrained VGG16 model

## Technologies

- Python
- PyTorch and Torchvision
- Jupyter Notebook
- NumPy, Pandas, Matplotlib, and scikit-learn
- Optuna for hyperparameter optimization

## Installation

1. Clone the repository and open its folder:

   ```bash
   git clone https://github.com/talhAIE/DeepLearning_pytorch.git
   cd DeepLearning_pytorch
   ```

2. Create and activate a virtual environment (optional but recommended), then install the dependencies:

   ```bash
   pip install torch torchvision jupyter numpy pandas matplotlib scikit-learn optuna pillow requests
   ```

3. Launch Jupyter and run the notebooks in order, beginning with `PytorchDL/01_PytorchFundamentals.ipynb`:

   ```bash
   jupyter notebook
   ```

Several Fashion-MNIST notebooks expect the dataset to be downloaded from Kaggle. Review the data-loading cells before running them locally, as some paths were written for Google Colab.

## Results

The notebooks train and evaluate regression and classification models, printing metrics such as loss and accuracy and visualizing predictions or decision boundaries where relevant. They show how model design, GPU acceleration, data augmentation, and tuning affect performance, rather than presenting a single fixed benchmark.

## Future Improvements

- Add a `requirements.txt` file with pinned dependency versions
- Make dataset download and local paths consistent across all notebooks
- Record final metrics and example outputs in a results summary
- Refactor repeated training code into reusable Python modules
- Add tests and a small command-line training example
