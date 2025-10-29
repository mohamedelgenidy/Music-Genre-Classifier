# Music Genre Recommendation System

This repository contains the code for a simple machine learning model that predicts a user's preferred music genre based on their age and gender. This project serves as a great introduction to machine learning concepts, data preparation, and model training using Scikit-learn.

## 🚀 Project Overview

The goal is to train a **Decision Tree Classifier** on a small dataset to learn the patterns between a user's age/gender and their musical taste. Once trained, the model can predict the likely genre for new users.

## 📊 Dataset

* **Source:** The model is trained on `music.csv`.
* **Features (Input):**
    * `age`: The user's age (e.g., 20, 25, 30).
    * `gender`: The user's gender (1 for Male, 0 for Female).
* **Target (Output):**
    * `genre`: The user's preferred music genre (e.g., `HipHop`, `Jazz`, `Classical`).

## ⚙️ Project Workflow

The project notebook (`Project2.ipynb`) follows these key steps:

1.  **Load Data:** The `music.csv` file is loaded into a Pandas DataFrame.
2.  **Separate Features & Target:** The data is split into:
    * `X`: The input features (`age`, `gender`).
    * `y`: The output target (`genre`).
3.  **Train-Test Split:** The dataset is split into a training set (70%) and a testing set (30%) to evaluate the model's performance on unseen data.
4.  **Model Training:**
    * A `DecisionTreeClassifier` from Scikit-learn is initialized.
    * The model is trained on the `X_train` and `y_train` data using `model.fit()`.
5.  **Inference (Prediction):**
    * The trained model is used to make predictions on new, example data. For instance, predicting the genre for a 22-year-old female and a 26-year-old male.

## 🛠️ Technologies Used

* Python 3
* Pandas
* Scikit-learn (`DecisionTreeClassifier`, `train_test_split`)
* Jupyter Notebook
