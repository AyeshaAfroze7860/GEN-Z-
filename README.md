## Title
### Gen Z Social Media Usage & Addiction Analysis

### Overview
This project analyzes social media usage patterns among Gen Z users and examines their relationship with addiction levels and mental health. Using data analysis, visualization and machine learning techniques, the project identifies key factors influencing social media addiction and predicts addiction levels based on user behavior.

### Objectives
Analyze Gen Z social media usage patterns.
Explore the relationship between social media usage and addiction levels.
Visualize trends and behavioral patterns.
Build a predictive model for addiction level classification.
Generate insights to better understand user behavior.

### Visualizations

The project includes:

Gender Distribution Analysis
Primary Platform Usage Analysis
Daily Usage Hours Distribution
Mental Health vs Usage Analysis
Addiction Level Distribution
Correlation Heatmap
Feature Importance Analysis

### Machine Learning Model
Algorithm: Random Forest Classifier
Data Split: 80% Training, 20% Testing
Evaluation Metrics:
Accuracy Score
Classification Report

### Key Insights
Higher social media usage is associated with increased addiction levels.
Platform preferences vary among users.
Usage behavior and screen time contribute significantly to addiction prediction.
Machine learning can effectively classify addiction levels based on user activity patterns.

## Pictures

<img width="851" height="633" alt="Screenshot 2026-06-16 153337" src="https://github.com/user-attachments/assets/d05650aa-86c8-4cc1-a93e-5e38813a525b" />

Observation:

The dataset contains 100,000 records and 12 features.
The first 5 rows display sample user information, social media usage patterns, mental health scores and addiction levels.
The dataset includes demographic details such as age, gender, and country, along with usage-related attributes like daily usage hours, primary platform and screen time before sleep.
The dataset shape and column list confirm that the data has been loaded successfully and is ready for further analysis.


<img width="636" height="773" alt="image" src="https://github.com/user-attachments/assets/c5ad6526-ea8b-4d49-adf1-2cc8a253ee15" />

Observation:

The dataset contains 100,000 records and 12 columns.
It includes 4 float columns, 3 integer columns and 5 categorical (object) columns.
The dataset occupies approximately 7.2 MB of memory.
Most columns contain complete data with very few missing values.
avg_session_minutes has 7 missing values.
mental_health_score has 7 missing values.
All other columns have no missing values.

Action Taken:

Missing values in numerical columns were handled by replacing them with the mean value of their respective columns.



<img width="825" height="765" alt="image" src="https://github.com/user-attachments/assets/e3cd71c1-efab-4fc0-9885-ab3d5d48a2c3" />

Observation:

The average age of users is approximately 20 years, with ages ranging from 13 to 27 years.
Users spend an average of 3.52 hours per day on social media.
On average, users engage with 3 social media platforms.
The average session duration is approximately 25 minutes.
The average mental health score is 7.16 out of 10.
The average screen time before sleep is approximately 40 minutes.
Most users have daily usage hours between 2.5 and 4.5 hours.

Purpose:

This summary provides key statistical measures such as mean, standard deviation, minimum, maximum and quartiles, helping to understand the overall distribution of the numerical features in the dataset.


<img width="962" height="606" alt="image" src="https://github.com/user-attachments/assets/d3e73b2e-37db-4fe1-bf1b-07e72e6590eb" />

Observation:

The number of Male and Female users is almost equal, with each category containing approximately 48,000 users.
The Other gender category has a significantly smaller number of users, around 4000.
Male and Female users together make up the majority of the dataset.

Purpose:

This visualization helps understand the gender composition of the dataset and ensures that the data is fairly balanced across the major gender categories.


<img width="1071" height="750" alt="image" src="https://github.com/user-attachments/assets/289cb40f-4e1d-41be-89b0-50e364b00f33" />
Observation:

Instagram is the most popular platform, with approximately 30,000 users.
YouTube and TikTok are the second most preferred platforms, each with around 25000 users.
Twitter and Snapchat have the lowest user counts, with approximately 10000 users each.
Most users prefer visual and video-based social media platforms.

Purpose:

This visualization helps identify the most frequently used social media platforms among Gen Z users and highlights platform popularity trends within the dataset.


<img width="1192" height="748" alt="image" src="https://github.com/user-attachments/assets/25ed2fa3-04fa-4d00-b2c2-5d48569a0e51" />
Observation:

Most users spend between 2 and 5 hours per day on social media.
The highest concentration of users is around 3.5 to 4 hours per day.
Very few users spend more than 7 hours daily on social media.
The distribution is slightly right-skewed, indicating that a small number of users have very high usage hours.

Purpose:

This histogram shows the distribution of daily social media usage among users and helps identify common usage patterns and extreme usage behavior.


<img width="1202" height="716" alt="image" src="https://github.com/user-attachments/assets/b4b60de8-71c9-411e-bd3a-559e4075ccf9" />
Observation:

The scatter plot shows a negative relationship between daily social media usage and mental health score.
Users with lower daily usage hours generally have higher mental health scores.
As daily usage hours increase, mental health scores tend to decrease.
Users spending 7–10 hours per day often have lower mental health scores compared to users with moderate usage.

Purpose:

This visualization helps examine the relationship between social media usage and mental health, showing how increased usage may be associated with lower mental well-being.


<img width="995" height="622" alt="image" src="https://github.com/user-attachments/assets/56ef5f46-0e0a-46e2-bab9-499f2fb9fb74" />

Observation:

The Medium addiction category has the highest number of users, with approximately 59,000 users.
The Low addiction category contains around 25000 users.
The High addiction category has the fewest users, with approximately 16000 users.
Most users fall into the Medium addiction level, indicating moderate social media dependence.

Purpose:

This visualization shows the distribution of users across different addiction levels and helps understand the prevalence of social media addiction within the dataset.


<img width="1352" height="575" alt="image" src="https://github.com/user-attachments/assets/d5d98e8f-1941-4920-a748-9bfd01114bcf" />
<img width="1362" height="462" alt="image" src="https://github.com/user-attachments/assets/a21c9f76-49f1-4003-82e3-d0f943c2b456" />

Observation:

The heatmap shows the correlation between numerical features in the dataset.
Daily usage hours and mental health score have a strong negative correlation (-0.76), indicating that higher social media usage is associated with lower mental health scores.
Most other feature pairs have correlation values close to 0, suggesting weak or no significant relationship.
The diagonal values are 1, representing perfect correlation of each feature with itself.

Purpose:

This visualization helps identify relationships between variables and highlights the features that may have the greatest influence on social media addiction and mental health outcomes.


<img width="757" height="377" alt="image" src="https://github.com/user-attachments/assets/50fc9700-76da-4861-a54d-e3fb35f4bf2b" />
Observation:

The Random Forest model achieved an accuracy of 1.0 (100%) on the test dataset.
Precision, Recall, and F1-score for all classes are 1.00, indicating perfect classification performance.
The model correctly classified all samples belonging to each addiction level category.
The test dataset contains 20,000 records, distributed across the three addiction classes.

Metrics Explanation:

Precision: Measures how many predicted values are actually correct.
Recall: Measures how many actual values were correctly identified.
F1-Score: Harmonic mean of precision and recall.
Support: Number of samples in each class.

Purpose:

This evaluation measures the performance of the Random Forest model and demonstrates its effectiveness in predicting social media addiction levels based on user behavior and usage patterns.


<img width="1463" height="766" alt="image" src="https://github.com/user-attachments/assets/fdb7875c-a630-4509-930d-53b1574b95b5" />

Observation:

Daily Usage Hours is the most important feature, contributing approximately 88% to the model's predictions.
Mental Health Score is the second most important feature, contributing around 12%.
Features such as Age, Gender, Country, Primary Platform, Purpose, Number of Platforms Used and Night Usage have very little impact on prediction.
The model relies mainly on users' social media usage patterns and mental health scores to determine addiction levels.

Purpose:

This visualization identifies the features that have the greatest influence on predicting social media addiction levels and helps understand which factors are most important in the machine learning model.


### Conclusion

This project demonstrates how data analytics and machine learning can be used to understand social media behavior among Gen Z users. The findings provide valuable insights into addiction patterns and highlight factors that may impact user well-being.
