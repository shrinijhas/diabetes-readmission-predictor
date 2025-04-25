# Predicting Hospital Readmissions for Diabetic Patients

## Project Summary

In this project, I worked on predicting whether a diabetic patient is likely to be readmitted to the hospital within 30 days after discharge. This is important because hospitals want to reduce these short-term readmissions to improve care and lower costs.

I used the UCI Diabetes dataset, cleaned it, explored some trends, and then built a couple of machine learning models to make predictions.

---

## Step 1: Understanding the Data

The dataset includes 10 years’ worth of hospital records for diabetic patients. It has demographic info, admission details, and treatment history. My main goal was to use these details to predict short-term readmissions.

---

## Step 2: Cleaning the Data

Here’s what I did to get the data ready:

- Dropped columns that weren’t useful like IDs or info with too many missing values.
- Replaced “?” with proper missing values and removed rows with missing data.
- Turned the readmission column into a binary label:  
  `1` = readmitted within 30 days,  
  `0` = otherwise.
- Encoded all the categorical variables using one-hot encoding to prepare for modeling.

---

## Step 3: Exploratory Data Analysis

I looked at:

- How age, gender, race, and number of medications relate to readmissions.
- Found some interesting patterns — like older patients and those on more medications were more likely to be readmitted.
- Visualized these trends using Seaborn and Matplotlib.

---

## Step 4: Modeling

I tried two models:

### Logistic Regression
- Easy to understand and interpret.
- Worked okay as a baseline, but it didn’t catch many of the actual readmitted patients.

### Random Forest
- Performed better overall, especially in identifying those who were readmitted.
- It handled the categorical data well and gave better recall.

---

## Step 5: Feature Importance

Using the Random Forest model, I checked which features were most important. This gave good insights into what might be influencing readmissions — useful in real healthcare settings for early interventions.

---

## Step 6: Final Thoughts

- The project covers the full pipeline: cleaning, exploration, modeling, and evaluation.
- The Random Forest model gave better results for identifying readmitted patients.
- I learned a lot about handling real-world healthcare data and evaluating models with an imbalanced target.
- Definitely something I’d like to expand with more advanced models or even integrate into a Tableau dashboard next.

---

Thanks for checking out my project!
