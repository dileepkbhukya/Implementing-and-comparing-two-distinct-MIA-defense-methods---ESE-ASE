
CIS 545 Final Project
This repository contains the code for the final Project, focusing on assessing the privacy risks associated with machine learning models. The project utilizes a dataset related to bank marketing and implements a membership inference attack on both a base logistic regression model and an ensemble model trained on disjoint datasets. There are two notebooks: ESE_Final_Project and ASE_Oracle_Group_2_CIS_545

Getting Started
To run the code, follow these steps:

Open the Jupyter Notebook ESE_Final_Project.ipynb or ASE_Oracle_Group_2_CIS_545.ipynb using Google Colab.

Install necessary packages by running the following commands:
Python Copy code
!pip install adversarial-robustness-toolbox
!pip hash
!pip install datasketch

Mount Google Drive to access the dataset:
Python Copy code:
from google.colab import drive
drive.mount('/content/drive')

Note: Update the file path in the code to point to the location of bank-full.csv on your Google Drive.
'/content/drive/MyDrive/yourfolderpath/bank-full.csv'

Execute the notebook cells to run the analysis.

Overview
The project includes the following key components:

Data Preprocessing: Loading the dataset, converting categorical columns, and performing one-hot encoding.

Model Training: Constructing logistic regression models, creating an ensemble model, and evaluating their performance.

Membership Inference Attack: Implementing a membership inference attack on both the base model and the ensemble model.

Ensemble Construction: Building an ensemble model using logistic regression models trained on disjoint datasets.

Evaluation: Assessing the accuracy of the membership inference attack on the ensemble model.

Visualization: Plotting the results to visualize the trade-off between model accuracy and attack accuracy.

Membership Inference Attack
The project demonstrates the vulnerability of machine learning models to membership inference attacks. The attack assesses whether an individual's data point was part of the training set based on the model's predictions.

Results
The code provides insights into the accuracy of the membership inference attack on both the base logistic regression model and the ensemble model. The results are visualized to understand the trade-offs between model accuracy and privacy risks.

Note
The code is designed to be run on Google Colab.
Ensure that the dataset (bank-full.csv) is available in the specified Google Drive location.
Some code sections may require adjustment based on your specific environment.
Both files start from the same base code until the sections for data perturbation, oracles, and MIA attacks.  Both files attempt to finish their evaluation in a similar fashion.
Feel free to explore, experiment, and adapt the code for further analysis or to apply it to different datasets.
