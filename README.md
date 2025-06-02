# Student Marks Classification and Visualization Project

This Python project analyzes student marks data, visualizes various relationships using graphs, and builds multiple machine learning models to classify student performance into categories (`L`, `M`, `H`). It also allows testing predictions on custom input data.

---

## Overview

- Loads and preprocesses student marks data from a CSV file.
- Provides interactive menu-driven visualization of different features vs. marks classification.
- Trains and evaluates several classifiers to predict student marks class.
- Allows user to test classification models with their own input data.

---

## Features

### 1. Data Visualization

The program displays 9 types of plots to analyze marks class distribution by:

1. Class count  
2. Semester-wise  
3. Gender-wise  
4. Nationality-wise  
5. Grade-wise  
6. Section-wise  
7. Topic-wise  
8. Stage-wise  
9. Student absence days-wise  

User selects which graph to display from the menu.

### 2. Data Preprocessing

- Drops irrelevant or redundant columns.  
- Converts categorical data to numerical using label encoding.  
- Shuffles the dataset.  
- Splits data into training (70%) and testing (30%) sets.

### 3. Machine Learning Models

Trains and tests the following classifiers on the data:

- **Decision Tree Classifier**  
- **Random Forest Classifier**  
- **Perceptron (Linear Model)**  
- **Logistic Regression (Linear Model)**  
- **MLP Neural Network Classifier**

The code outputs accuracy and classification reports for each model.

### 4. Custom Input Testing

After training, the user can input custom student data (such as gender, grade, semester, hands raised, etc.) to get predictions from all five models on the marks class.

---

## How to Run

1. Make sure required libraries are installed: `pandas`, `seaborn`, `matplotlib`, `numpy`, `scikit-learn`.  
2. Place the `AI-Data.csv` file in the correct path (default is `C:\Users\Dell\Downloads\AI-Data.csv` in the script).  
3. Run the script using:

   ```bash
   python Project.py
