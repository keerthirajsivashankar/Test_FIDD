Test.ipynb - Machine Learning Model Training Notebook
This Jupyter Notebook (Test.ipynb) contains Python code for training and evaluating a Machine Learning model, specifically a RandomForestClassifier. It demonstrates a typical workflow for a classification task, including data loading, preprocessing, model training, saving, and evaluation.
Project Description
The primary purpose of this notebook is to:

Load a dataset from a CSV file (data/mydata.csv).
Define features and a target variable for a classification problem.
Preprocess the features using StandardScaler.
Split the data into training and testing sets.
Train a RandomForestClassifier model.
Save the trained model and the scaler for future use.
Evaluate the model's performance based on accuracy.

Features and Target
The model uses the following features from the dataset:

profile pic
nums/length username
fullname words
nums/length fullname
name==username
description length
external URL
private
#posts
#followers
#follows

The target variable for prediction is:

fake

Model Used

Algorithm: RandomForestClassifier
Parameters: n_estimators=100, random_state=42

Dependencies
The following Python libraries are required to run this notebook:

pandas
joblib
sklearn (scikit-learn)
os

You can install these dependencies using pip:
pip install pandas joblib scikit-learn

How to Run

Data Preparation: Ensure you have a CSV file named mydata.csv in a directory named data/ relative to where this notebook is located. The CSV file must contain the columns specified in the "Features and Target" section.
Directory Setup: The notebook will automatically create a models/ directory if it doesn't already exist.
Execute: Open the Test.ipynb file in a Jupyter environment (e.g., JupyterLab, Jupyter Notebook, VS Code with Jupyter extension) and run all cells sequentially.

Output
Upon successful execution, the notebook will:

Train the RandomForestClassifier model.
Save the trained model to models/random_forest_model.pkl.
Save the StandardScaler object to models/scaler.pkl.
Print the accuracy of the trained model on the test set to the console.

Example Output:
✅ Model trained and saved! Accuracy: 0.91

