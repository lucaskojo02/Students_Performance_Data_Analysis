# Exploratory Data Analysis (EDA) and Modelling Report
![Medium Image](https://cdn-images-1.medium.com/max/800/0*uGSIJbw5FHlwzqBg.jpg)

## 1. Introduction

This report summarizes the findings from exploratory data analysis (EDA) and predictive modeling on student performance data. The objective is to understand the key factors influencing academic success and build predictive models to forecast performance based on various attributes.

# Column Descriptions

| Attribute                  | Description |
|----------------------------|-------------|
| **Hours_Studied**          | Number of hours spent studying per week. |
| **Attendance**             | Percentage of classes attended. |
| **Parental_Involvement**   | Level of parental involvement in the student's education (Low, Medium, High). |
| **Access_to_Resources**    | Availability of educational resources (Low, Medium, High). |
| **Extracurricular_Activities** | Participation in extracurricular activities (Yes, No). |
| **Sleep_Hours**            | Average number of hours of sleep per night. |
| **Previous_Scores**        | Scores from previous exams. |
| **Motivation_Level**       | Student's level of motivation (Low, Medium, High). |
| **Internet_Access**        | Availability of internet access (Yes, No). |
| **Tutoring_Sessions**      | Number of tutoring sessions attended per month. |
| **Family_Income**          | Family income level (Low, Medium, High). |
| **Teacher_Quality**        | Quality of the teachers (Low, Medium, High). |
| **School_Type**            | Type of school attended (Public, Private). |
| **Peer_Influence**         | Influence of peers on academic performance (Positive, Neutral, Negative). |
| **Physical_Activity**      | Average number of hours of physical activity per week. |
| **Learning_Disabilities**  | Presence of learning disabilities (Yes, No). |
| **Parental_Education_Level** | Highest education level of parents (High School, College, Postgraduate). |
| **Distance_from_Home**     | Distance from home to school (Near, Moderate, Far). |
| **Gender**                | Gender of the student (Male, Female). |
| **Exam_Score**            | Final exam score. |


## 2. Data Preprocessing and EDA

### 2.1 Data Cleaning

- Missing values were identified and handled appropriately.
- Outliers were detected and addressed where necessary.
- Data types were standardized for consistency.

### 2.2 Exploratory Data Analysis

#### Histogram Analysis

- **Hours Studied:** The distribution is approximately normal, peaking between 15-25 hours.
- **Attendance:** Mostly uniform, but a noticeable peak at 100% suggests many students maintain full attendance.
- **Sleep Hours:** A multimodal distribution with peaks around 5, 6, 7, and 8 hours.

#### Correlation Analysis

- **Strong positive correlation** between attendance(0.58) and exam score, and hours studied(0.45) and exam score.
- **Moderate positive correlation** between previous score(0.18) and exam score, and tutoring sessions(0.16) and exam score.
- **Weak correlation** between sleep hours and performance.

#### Box Plot Insights

- Variability in grades increases with higher study hours.
- Students with near-perfect attendance generally have better performance.

## 3. Predictive Modeling

### 3.1 Model Selection and Training

Several machine learning models were trained and evaluated, including:

- **Linear Regression**  
  - Simple yet effective for predicting student scores.  
  - R² score indicates moderate explanatory power.  

- **Random Forest Regression**  
  - Provides better generalization with ensemble learning.  
  - Achieved the highest accuracy among tested models.

- **XGBoost**  
  - Enhanced accuracy, leveragin sequential tree boosting to correct residual errors.
  - Achieved the highest predictive performance and was selected as the final model for interpretation and deployment.


### 3.2 Model Evaluation

- **Mean Squared Error (MSE):** Used to measure prediction accuracy.
- **R² Score:** Evaluated how well the model explains variance in student performance.
- **Random Forest** performed best in balancing bias and variance.
- **XGBoost** Achieved the highest predictive performance.

## 4. Conclusion and Recommendations

### Key Findings
- Study hours and attendance are the most influential factors in predicting student performance.

### Actionable Insights
- Encouraging students to maintain regular study schedules can boost performance.
- Improving attendance policies may positively impact overall student success.

### Future Work
- Integrating additional features such as mental well-being and extracurricular activities.
- Experimenting with deep learning models for improved prediction accuracy.

This analysis provides valuable insights into student learning patterns and can help educators develop data-driven strategies for academic improvement.
can help educators develop data-driven strategies for academic improvement.

## 5. References 
- [The Hidden Keys to Student Success: What Really Drives Performance?](https://medium.com/@crispinoigara/the-hidden-keys-to-student-success-what-really-drives-performance-b88b2aef37b3)
- [Hanushek, E. A., & Woessmann, L. (2011). "The Economics of International Differences in Educational Achievement."](https://www.nber.org/papers/w15949)  

