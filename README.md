# Student Depression Analysis

## Project Overview

This project aims to analyze and predict student depression using machine learning models. The analysis focuses on identifying key factors that contribute to student mental health issues, such as academic pressure, financial stress, sleep duration, and lifestyle habits.

### Goals:
- To predict the likelihood of a student suffering from depression based on multiple variables.
- To explore and identify the most significant factors affecting student mental health.
- To provide insights that can guide interventions for improving student well-being.

## Data
The dataset used in this project contains several features related to student mental health, including:
- **Depression**: Target variable (0 for no depression, 1 for depression).
- **Academic Pressure**: Measure of the academic stress students face.
- **Work Pressure**: Pressure caused by work or job.
- **Study Satisfaction**: Level of satisfaction with studies.
- **Sleep Duration**: Average hours of sleep per night.
- **Dietary Habits**: Healthiness of dietary habits.
- **Financial Stress**: Pressure caused by financial difficulties.
- **Family History of Mental Illness**: Presence of family history regarding mental health.

## Process Summary

### 1. **Data Cleaning and Preparation**
   - Handle missing values and duplicates in the dataset.
   - Exploratory data analysis to understand the relationships between variables and the target.
   - Feature engineering where applicable to improve model performance.

### 2. **Modeling Approach**
   - Used tree-based machine learning algorithms: **XGBoost** and **LightGBM**.
   - Split the dataset into training and testing sets for model training and evaluation.
   - Applied **early stopping** to prevent overfitting in the model.
   - **Feature importance analysis** was performed to identify the most influential predictors of depression.

### 3. **Balancing the Dataset**
   - Performed **undersampling** and **oversampling** techniques to handle imbalanced classes.
     - **Undersampling**: Reducing the majority class (students with no depression) to balance the target variable.
     - **Oversampling**: Increasing the minority class (students with depression) to match the majority.
   - The final balanced dataset was used for training machine learning models.

### 4. **Model Evaluation**
   - Evaluated model performance using metrics such as **accuracy** and **AUC (Area Under the ROC Curve)**.
   - Compared the results of XGBoost and LightGBM models.
   - Determined which features had the greatest impact on the likelihood of student depression.

### 5. **Key Insights**
   - Financial stress, academic pressure, and sleep duration were found to be the most significant contributors to student depression.
   - Study satisfaction and healthy lifestyle habits (good sleep and diet) play a role in reducing depression risk.
   - The field of study (degree choice) was not as impactful as overall academic pressure.

## Summary of Results

### 1. **What factors in a student’s academic environment increase the likelihood of them experiencing depression?**
   - Our analysis revealed that financial stress, academic pressure, and sleep duration are the most significant factors affecting the likelihood of depression among students. Students facing financial difficulties and high academic stress, combined with insufficient sleep, are at a higher risk of experiencing mental health issues.

### 2. **Does the pressure from pursuing certain degree programs affect students’ mental health?**
   - While the specific degree chosen by a student was not a significant factor in predicting depression, the level of academic pressure was. This finding suggests that the overall workload and expectations from academic programs are more likely to contribute to depression than the particular field of study.

### 3. **How do students’ lifestyle choices and overall health influence their satisfaction and ability to manage academic pressure?**
   - Our analysis revealed that financial stress, academic pressure, and sleep duration are the most significant factors affecting the likelihood of depression among students. Students facing financial difficulties and high academic stress, combined with insufficient sleep, are at a higher risk of experiencing mental health issues.

## Blogpost

- The findings of the notebook are showcased in the following blogpost: https://medium.com/@cyberspartan228/analyzing-student-depression-a-data-science-perspective-0330c9c1b7e1

## Acknowledgements

The used in this notebook was retrieved from the open-source datasest provide by Kaggle: https://www.kaggle.com/datasets/ikynahidwin/depression-student-dataset

## Installation

To run the notebook and reproduce the analysis, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/TiisetsoM228/Udacity-Project-1.git
   cd Udacity-Project-1-Tiisetso-Masalesa
   ```

2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter notebook:
   ```bash
   jupyter notebook
   ```

4. Open the notebook `DS_Project_1.ipynb` to explore the data, model training, and results.

## Dependencies

- **Python 3.x**
- **Jupyter Notebook**
- **XGBoost**
- **LightGBM**
- **Pandas**
- **Numpy**
- **Scikit-learn**
- **Matplotlib** and **Seaborn** for visualizations

## File Structure

```
.
├── DS_Project_1.ipynb        # Main notebook containing data analysis and modeling
├── README.md                 # This README file
├── requirements.txt          # Python package dependencies
└── data/                     # Data files (if applicable)
```
