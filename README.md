# brainage_pred
# Brain Age Prediction from MRI

A deep learning project exploring age-group classification from structural brain MRI scans using 3D and 2D convolutional neural network architectures.

## Overview

Brain age prediction explores the relationship between structural brain characteristics and chronological age. This project investigates the use of deep learning models to classify brain MRI scans into three age groups.

The work involved developing and benchmarking different architectures and MRI representations to examine how volumetric and 2D image-based approaches perform on the classification task.

## Objectives

- Develop deep learning models for age-group classification from T1-weighted brain MRI scans.
- Explore volumetric learning using 3D convolutional neural networks.
- Investigate 2D MRI representations using axial and sagittal views.
- Compare architectural approaches in terms of predictive performance and computational requirements.

## Models and Approaches

| Architecture | MRI representation |
|---|---|
| 3D ResNet-50 | Volumetric MRI |
| 2D DenseNet-121 | Axial slices |
| 2D DenseNet-121 | Sagittal slices |

### Experimental Workflow

1. **MRI preprocessing:** Standardisation of image orientation, intensity and resolution.
2. **Data preparation:** Organisation of MRI scans and age-group labels.
3. **Model development:** Implementation of 3D ResNet-50 and 2D DenseNet-121 architectures using PyTorch.
4. **Evaluation:** Comparison of model performance across different MRI representations.

## Results

The 3D ResNet-50 model achieved **88% test accuracy** on the three-class age-group classification task.

The experiments also explored 2D axial and sagittal representations using DenseNet-121, providing a basis for examining the trade-offs between volumetric and slice-based learning.

## Repository Structure

```text
brainage_pred/
│
├── brain-age-classificaiton.ipynb
├── densenet_axial.ipynb
├── densenet_sagittal.ipynb
└── README.md
```

## Technologies Used

- Python
- PyTorch
- 3D ResNet-50
- DenseNet-121
- Medical Image Processing
- Deep Learning
- Jupyter Notebook

## Getting Started

Clone the repository:

```bash
git clone https://github.com/keertish05/brainage_pred.git
cd brainage_pred
```

Install the required libraries used in the notebooks, then open the notebooks using Jupyter Notebook or JupyterLab.

```bash
pip install torch torchvision numpy pandas matplotlib scikit-learn nibabel jupyter
```

**Note:** Dataset access and preprocessing paths may need to be configured according to your local environment. The MRI dataset is not included in this repository.

## Project Context

This work was carried out as part of a research internship at the LNM Institute of Information Technology (LNMIIT), where different deep learning architectures were explored for MRI-based brain age classification.

---

*This repository documents the experimental notebooks and model development work undertaken during the project.*
