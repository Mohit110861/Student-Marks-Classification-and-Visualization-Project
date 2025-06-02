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

### Data Visualization Output and Graph Explanation

When you run the script, it displays the following menu options to select different graphs related to the student marks classification data:


---

#### Explanation of Each Graph:

1. **Marks Class Count Graph:**  
   A simple bar chart showing the total count of students in each marks class (`L`, `M`, `H`). This helps understand the distribution of students across different performance levels.

2. **Marks Class Semester-wise Graph:**  
   A grouped bar chart showing the number of students in each marks class broken down by semester (e.g., First or Second semester). This reveals if semester influences performance distribution.

3. **Marks Class Gender-wise Graph:**  
   A grouped bar chart that shows marks class distribution for male and female students. Useful to check if gender correlates with performance classes.

4. **Marks Class Nationality-wise Graph:**  
   Displays the counts of each marks class for different nationalities, showing how performance varies across student nationalities.

5. **Marks Class Grade-wise Graph:**  
   Shows marks class counts broken down by grade level (e.g., G-02 to G-12). This can highlight trends in performance as students progress through grades.

6. **Marks Class Section-wise Graph:**  
   A grouped bar chart showing marks classes distributed by section IDs, indicating how performance differs across sections or groups.

7. **Marks Class Topic-wise Graph:**  
   Displays the count of students in each marks class for different topics (subjects). Helps analyze which subjects might influence student marks class.

8. **Marks Class Stage-wise Graph:**  
   Shows performance class counts across different stages (StageID), which might correspond to learning or evaluation phases.

9. **Marks Class Absent Days-wise Graph:**  
   A grouped bar chart showing marks class counts broken down by student absence days (`Under-7` or `Above-7` days). This helps to analyze how absenteeism impacts performance.

10. **No Graph (Exit):**  
    Exits the visualization menu.

---

#### Sample Graph Interpretation:

For example, the **Marks Class Gender-wise Graph** might show that female students have a higher count in the `H` (high marks) class compared to male students, suggesting a possible gender performance gap. Similarly, the **Absent Days-wise Graph** might reveal that students with fewer absences tend to fall more in the `H` class, indicating attendance affects academic performance.

Each graph uses color hues to differentiate the marks classes (`L`, `M`, `H`) and provides a clear visual representation of how different factors relate to student marks classification.

---

### Output Example in Console

Upon running, the menu appears:



---

## How to Run

1. Make sure required libraries are installed: `pandas`, `seaborn`, `matplotlib`, `numpy`, `scikit-learn`.  
2. Place the `AI-Data.csv` file in the correct path (default is `C:\Users\Dell\Downloads\AI-Data.csv` in the script).  
3. Run the script using:

   ```bash
   python Project.py
