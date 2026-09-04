# repeat-hackathon
Spaceship Accident — Data Science Challenge

**Project Overview**

This repository contains the group work for the Data Science Challenge / Repeat Hackathon project.

The objective is to build and compare machine-learning models that predict whether a passenger was Transported in the Spaceship Accident dataset.

Problem type: Binary classification

Target: Transported

Training rows: 5,798

Testing rows: 2,895

Training columns: 14 including the target

Testing columns: 13

Dataset Features

The dataset contains:

PassengerId

HomePlanet

CryoSleep

Cabin

Destination

Age

VIP

RoomService

FoodCourt

ShoppingMall

Spa

VRDeck

Name

Transported — target variable in the training dataset

Group Workflow

**The project was developed progressively by six group members.
**
23069871 — Initial EDA
23081838-Advanced EDA
23111190-Feature Engineering, Preprocessing and Baseline Modelling
23099463-Model Evaluation and Tuning
23082277-Ensemble and Final Ranking
23068870-final predictions
Candidate Models

The final comparison contains six unique approaches:

Logistic Regression

svm

Random Forest

HistGradientBoosting

XGBoost

Weighted Ensemble

Current Top Five Prediction Approaches

The corrected ranking used for the current submission is:

HistGradientBoosting

Weighted Ensemble

XGBoost

Random Forest

Logistic Regression



Prediction Files

The final prediction files are:

order_1.csv
order_2.csv
order_3.csv
order_4.csv
order_5.csv

Each file contains:

PassengerId,Transported

The Transported prediction is stored as 0 or 1.

Each file contains predictions for all 2,895 test passengers in the original test-set order.

Repository Structure

Suggested structure:

.
├── dataset_Repeat_training.csv
├── dataset_Repeat_testing.csv
├── Initial_EDA.ipynb
├── Advanced_EDA.ipynb
├── Modelling.ipynb
├── Tuning_Evaluation.ipynb
├── Ensemble_Ranking.ipynb
├── Final_Predictions.ipynb
├── order_1.csv
├── order_2.csv
├── order_3.csv
├── order_4.csv
├── order_5.csv
├── model_ranking.csv
├── README.md
└── LICENSE

How to Run

Open the notebook in Google Colab.

Upload:

dataset_Repeat_training.csv

dataset_Repeat_testing.csv

Run the notebook from top to bottom.

Allow the XGBoost package installation if prompted.

Run the final ranking section.

Run the final prediction section.

Download the five generated CSV files.

Validation Strategy

The workflow uses:

Stratified train/validation splitting

Five-fold stratified cross-validation

Multiple classification metrics

Hold-out validation

Hyperparameter tuning

Comparison of individual models and an ensemble

Validation metrics are used to rank the models before generating predictions for the hidden test dataset.

Explainable AI

Explainable AI is intentionally not included in the hackathon version.

XAI can be added later as a separate post-hackathon section using techniques such as feature importance, permutation importance and SHAP, if required.

Collaboration

The repository should be used together with the team's GitHub and Google Colab version history to demonstrate genuine contributions from all six members.

Each team member should understand the full modelling workflow and be able to explain their own contribution as well as the overall project.

GitHub and Colab Links

Add the group's final links here before submission:

GitHub Repository: https://github.com/repeat-hackathon

Google Colab: https://colab.research.google.com/drive/1QpTftUXU5-IAGmNXBcz74NVOpwrrcV65?usp=sharing

Licence

This project is released under the MIT License. See the LICENSE file for details.

Academic Use

This repository was prepared for the University Data Science Challenge group assignment. Any submitted work should reflect the group's genuine collaborative development, execution history and understanding of the code.
 Post-Hackathon Explainable AI

Explainable AI was applied after model development to understand which features influenced predictions and how they affected model decisions. SHAP was used for XGBoost to provide global and local explanations, while permutation importance was applied to HistGradientBoosting for comparison.

The final version keeps the original modelling workflow but includes improved figure presentation and Explainable AI (XAI). The visualisations were refined to make model performance easier to compare, including clearer performance plots and ROC curves. XAI was added using SHAP for XGBoost and permutation importance for HistGradientBoosting to identify important features and explain how they influence predictions.
