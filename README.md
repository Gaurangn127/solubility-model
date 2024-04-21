# Linear Regression Model for Predicting Solubility (logS)

## Overview
This repository contains a linear regression model built to predict the solubility (logS) of chemical compounds based on several molecular descriptors. 
The model is trained on a dataset consisting of various molecular properties and their corresponding 'experimental' solubility values.

## Dataset
The dataset used for training the model comprises the following molecular descriptors:
- MolLogP: Molecule's octanol-water partition coefficient.
- MolWt: Molecular weight of the molecule.
- NumRotatableBonds: Number of rotatable bonds in the molecule.
- AromaticProportion: Proportion of aromatic atoms in the molecule.
- logS: Experimental solubility value (log-scale).

A snippet of the dataset:
| MolLogP | MolWt  | NumRotatableBonds | AromaticProportion | logS  |
|---------|--------|-------------------|--------------------|-------|
| 2.59540 | 167.850| 0.0               | 0.000000           | -2.180|
| 2.37650 | 133.405| 0.0               | 0.000000           | -2.000|
| 2.59380 | 167.850| 1.0               | 0.000000           | -1.740|
| ...     | ...    | ...               | ...                | ...   |

## Model Training
- The linear regression model is trained to predict the solubility (logS) using the molecular descriptors mentioned above. 
- During training, the model learns the relationship between these descriptors and the experimental solubility values.

## Evaluation
- The model's performance is evaluated based on various metrics such as mean squared error, R-squared score, etc. 
- Visualization techniques like scatter plots have been used to assess how accurately the model predictions align with the experimental solubility values.

## Results
Upon evaluation, the trained model demonstrates a reasonable level of accuracy in predicting solubility values based on the given molecular descriptors. 
The README file includes a scatter plot illustrating the relationship between predicted and experimental logS values.

## Repository Contents
- `model.ipynb`: Jupyter Notebook containing the code for model training, evaluation, and visualization.
- `dataset.csv`: CSV file containing the dataset used for training the model.
- `README.md`: This file providing an overview of the project and its contents.

## Requirements
To run the Jupyter Notebook and reproduce the results, the following dependencies are required:
- Python 3.x
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## Usage
1. Clone the repository to your local machine.
2. Install the required dependencies.
3. Open and run the `model.ipynb` notebook using Jupyter Notebook.

## License
This project is licensed under the [MIT License](https://www.mit.edu/~amini/LICENSE.md).
