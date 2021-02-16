# Numerical experiments on Wasserstein Eigenvectors

This repository contains Jupyter notebooks to replicate the experiments from our paper "Unsupervised Ground Metric Learning Using Wasserstein Eigenvectors" (Huizing, Cantini, Peyré 2021). https://arxiv.org/abs/2102.06278

## Notebooks

- `1D_synthetic.ipynb`: Wasserstein Eigenvectors of synthetic datasets of translated histograms on the 1D torus. Figures 1 and 3 of the paper.
- `2D_synthetic.ipynb`: Wasserstein Eigenvectors of synthetic datasets of translated histograms on the 2D torus. Figure 2 of the paper.
- `MNIST.ipynb`: Wasserstein Singular Vectors of a subset of the MNIST dataset (see Sample Data). Figures 5 and 6 of the paper.
- `scRNA_seq.ipynb`: Wasserstein Singular Vectors with entropic regularization of a single-cell RNA-seq dataset (see Sample Data). Figures 7, 8 and 9 of the paper.

## Sample Data

- `mnist_train_small.csv`: Subset of the MNIST dataset of handwritten digits.
- `rna_preprocessed.csv.gz`: Log-transformed scRNA-seq counts of 206 cells from 3 cell lines, with only the most varying genes. From Liu et al. (https://www.nature.com/articles/s41467-018-08205-7).

## Dependencies

These notebooks have been run on Python 3.6.9. GPU is required in `scRNA_seq.ipynb`. Dependencies include:
- pot (https://pythonot.github.io/)
- pandas
- numpy
- matplotlib
- sklearn
- cupy
- scipy
