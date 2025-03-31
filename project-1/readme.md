





# Project 2: Diabetes Dataset Analysis
## Project Overview
For this project, I will be analyzing the patient's medical information to find the key characteristics associated with diabetes. The goal is to understand which characteristics are more prevalent in patients with diabetes.
## Dataset Information
- **Dataset Name**: Diabetes Dataset
- **Dataset Source**: Kaggle
- **Dataset URL**: [Diabetes Dataset](https://www.kaggle.com/datasets/akshaydattatraykhare/diabetes-dataset/data)
- **Dataset Description**: This dataset contains patient diagnostic measurements and if they have diabetes or not. All patients are female, at least 21 years old, and of Pima Indian heritage.
- **Author**: Akshay Dattatray Khare
- **Citations**: The author mentions that this dataset is originally from the National Institute of Diabetes and Digestive and Kidney Diseases and UCI Machine Learning.
- **Licensing and Usage**: According to the licensing section, this dataset is classified as CC0: Public Domain. The author has waived all of their rights to the work worldwide under copyright law. There are no restrictions on how I can use or share the data.
## Main Question
What key characteristics distinguish diabetic from non-diabetic patients?
## Dataset Structure
The dataset has the following columns:
- **Pregnancies**: The number of pregnancies the patient had.
- **Glucose**: The glucose level in the patient's blood.
- **BloodPressure**: The blood pressure measurement for each patient.
- **SkinThickness**: The thickness of the skin of the patient.
- **Insulin**: The insulin level in the patient's blood.
- **BMI**: The body mass index of the patient.
- **DiabetesPedigreeFunction**: The diabetes percentage of the patient.
- **Age**: The age of the patient.
- **Outcome**: Whether the patient has diabetes or not. 1 is Yes and 0 is No.
## Data Cleaning
The dataset was cleaned by performing the following:
- **Handling 0 values**: Replaced the 0 values with the median or used K-Nearest Neighbors.
- **Checked for missing values**: None were found.
- **Checked for duplicate rows**: None were found.
- **Examined data types**: The data types did not need to be adjusted.
- **Examined numerical data**: Reviewed distributions and outliers. Many outliers were kept. Without additional domain knowledge, there is not much justification to remove what are suspected to be outliers.
## Exploratory Data Analysis
I examined the potential relationships within the data through:
- **Correlation matrix and heatmap**: I found that 'Glucose', 'BMI', and 'Age' had the highest correlation to 'Outcome'.
- **Visualizations**: Through histograms, boxplots, and scatterplots I examined the relationships between different columns and the diabetes outcome.
## Findings
- **Glucose**: Higher glucose levels are associated with a patient having diabetes.
- **BMI**: A higher BMI is associated with a patient having diabetes.
- **Age**: Age is also a key indicator of a patient potentially having diabetes.
## Visualizations
I created a dashboard on Tableau Public with visualizations of the key findings.
[Tableau Dashboard](https://public.tableau.com/views/Project2DiabetesDatasetAnalysis/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
## Conclusion
- **Key Takeaways**: Higher glucose levels, BMI, and age are the strongest indicators of diabetes diagnosis.
- **Limitations**: The 'SkinThicknes' (227) and 'Insulin' (374) columns had many 0 values.
