AI & ML Internship – Task 4: Feature Encoding & Scaling

 Overview

This project focuses on **feature engineering** techniques applied to the **Adult Income Dataset** as part of *AI & ML Internship – Task 4*. The objective is to prepare raw data for machine learning models by performing encoding and scaling operations, ensuring better model performance and readiness.

Dataset

* **Name:** Adult Income Dataset (`adult.csv`)
* **Description:** Contains demographic and employment-related attributes used to predict whether an individual’s income exceeds $50K per year.
* **Target Variable:** Income (<=50K or >50K)

Tools & Libraries Used

* Python
* Pandas
* NumPy
* Scikit-learn (LabelEncoder, OneHotEncoder, StandardScaler)

 Tasks Performed
1. Identified Feature Types

* **Categorical Features:** workclass, education, marital-status, occupation, relationship, race, sex, native-country, income
* **Numerical Features:** age, fnlwgt, education-num, capital-gain, capital-loss, hours-per-week

2. Label Encoding

* Applied **Label Encoding** to the `education` column since it has an inherent order (ordinal feature).

 3. One-Hot Encoding

* Applied **One-Hot Encoding** to nominal categorical features where no order exists.
* Used `get_dummies()` with `drop_first=True` to avoid dummy variable trap.

 4. Feature Scaling

* Scaled all numerical features using **StandardScaler**.
* Ensured features have mean = 0 and standard deviation = 1.

5. Model Readiness Comparison

* **Before Scaling:** Numerical features had varying ranges, which could bias ML algorithms.
* **After Scaling:** All numerical features are standardized, improving learning stability and convergence speed.

 6. Impact of Scaling on ML Algorithms

* Essential for distance-based algorithms (KNN, SVM, K-Means).
* Improves performance of gradient-based models (Logistic Regression, Linear Regression).
* Tree-based models (Decision Tree, Random Forest) are generally not affected by scaling.

 7. Saving Processed Dataset

* Final preprocessed dataset saved as **`adult_processed.csv`**.

 Project Deliverables

* `adult.csv` – Original dataset
* `adult_processed.csv` – Encoded and scaled dataset
* Python preprocessing script / notebook
* README.md

Final Outcome

* Gained hands-on experience in **feature encoding and scaling**.
* Understood when and why to apply **Label Encoding vs One-Hot Encoding**.
* Learned the importance of **feature scaling** for machine learning algorithms.
 Interview Prep (From This Task)

* Difference between Label Encoding and One-Hot Encoding
* Why feature scaling is required
* Which ML algorithms need scaling
* What is feature engineering


This project ensures the dataset is **fully prepared for machine learning model training**.
