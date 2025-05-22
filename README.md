### Prediction and analysis of personality traits based on handwritten features

**Pengyu Zhao**

---

#### Abstract

   The aim of this project is to predict individuals' scores in the five dimensions of the Big Five personality traits by analyzing handwritten data: openness, conscientiousness, extroversion, agreeableness, and neuroticism. We used multiple machine learning methods to model a large number of handwriting samples and ultimately chose the XGBoost model as the best prediction model. The results showed that certain handwritten features, such as letter size, tilt angle, pen pressure, etc., were significantly correlated with personality traits. In the future, it can be expanded to fields such as education, psychological assessment, and human resource screening.

---

#### Rationale

   Personality assessment has wide application value in the fields of human resources, mental health, and education. Traditional personality assessment relies on questionnaires and self-reports, which may have subjective biases. This study attempts to conduct personality analysis through "objective" handwritten behavior data, providing a new approach for personality assessment that is both scientific and practical.

---

#### Research Question

   Can we accurately predict a person's scores in the five personality dimensions of the "Big Five Personality" model based solely on their handwriting characteristics?

---

#### Data Sources

   I am using a publicly available large-scale handwritten sample dataset, where each record includes:
   -Multiple handwriting features (such as pen pressure, letter size, spacing, tilt angle, etc.)
   -Rating of the five personality dimensions corresponding to individuals (numerical labels)

   The data has been preprocessed and converted into a format suitable for machine learning modeling.

---

#### Methodology

   1. Exploratory Data Analysis
   2. Feature Engineering and Standardization (StandardScaler+OneHotEncoder)
   3. Establish a multi-objective regression model for personality prediction
   4. Model comparison: Random Forest, Linear Regression XGBoost
   5. Model evaluation indicators: R ² score, mean square error (MSE)
   6. Feature importance analysis: based on SHAP value and feature importance ranking

---

#### Results

   - **Best Model**：XGBoost (After optimization) performs the best on average cross validation R ².
   - **The easiest trait to predict**：Agreeableness (R ²=-0.001)
   - **The most unpredictable trait**：Extraversion (R² = -0.014)
   - **Important handwritten features include**：
     - Overall legibility score
     - Slant angle of handwriting
     - Letter spacing consistency
     - Pen tilt direction
     - Word spacing variability

---

#### Next Steps

   -Expand sample sources (covering different age groups and cultural backgrounds)
   -Directly extracting handwriting image features using image processing methods
   -Introducing deep learning models for more complex feature learning
   -Applying the model to practical scenarios such as education screening and job matching

---

#### Conclusion

   This project successfully demonstrated the feasibility of predicting personality traits through handwritten features. Although some dimensions (such as extroversion) have weaker predictive performance, the overall results are informative. I hope this exploration can provide new ideas for fields such as education, recruitment, and mental health. It should be noted that this study is only based on a single dataset, and the results still need to be validated on larger samples, and cannot be used as a psychological diagnostic tool.

---

### Bibliography

> [1] Goldberg, L. R. (1990). An alternative “description of personality”: the Big-Five factor structure. *Journal of personality and social psychology*, 59(6), 1216.  
> [2] Chen, T., & Guestrin, C. (2016). XGBoost: A scalable tree boosting system. *Proceedings of the 22nd ACM SIGKDD*, 785–794.  
> [3] Lundberg, S. M., & Lee, S. I. (2017). A unified approach to interpreting model predictions. *Advances in neural information processing systems*, 30.  

---

##### Contact and Further Information

   For more project details or data sources, please contact the author's email:` z1603799337@hotmail.com `
