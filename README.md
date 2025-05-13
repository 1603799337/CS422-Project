# CS422-Project

##  Project Background and Problem Statement

Each of us has our own unique handwriting, with some writing in large and loose strokes, while others are compact and meticulous. These seemingly simple handwritten features are actually closely related to our personality traits. The goal of this project is to explore:"**Can a person's handwriting reflect their personality traits?**"

To this end, we attempt to build a machine learning model that takes in a person's handwritten features (such as pen pressure, letter size, spacing, etc.) and predicts their scores in the five dimensions of the Big Five personality traits:

- **Openness**
- **Conscientiousness**
- **Extraversion**
- **Agreeableness**
- **Neuroticism**

---

##  Overview of Data and Methods

I used a large dataset containing thousands of handwritten samples, where each sample was labeled with its corresponding five personality scores. Multiple handwriting features were extracted from it, such as:

-The fluctuation of stroke pressure
-The spacing between letters
-Row spacing
-Letter height, width, etc

Then I used various machine learning methods (such as random forest, linear regression, gradient boosting, etc.) for training and comparison, and finally selected the optimal model to complete the prediction task.

---

##  Model performance

I ultimately chose the **Optimized XGBoost Model**, which performed the best in overall predictive ability. The model can accurately predict an individual's personality score

Some traits have relatively weak predictive performance due to unclear characteristic signals, but the overall trend still has explanatory power.

---

##  Key Findings

1. **Best Model**: *XGBoost (After optimization)* achieved the best performance based on average cross-validation R² scores across all personality traits.
2. **Easiest Trait to Predict**: *Agreeableness*, although the R² score was very low (-0.001), it was still the least difficult among the five traits.
3. **Most Unpredictable Trait**: *Extraversion*, with an R² of -0.014, was the hardest trait to predict accurately.
4. **Important Characteristics**:
   - **Feature_Overall legibility score**
   - **Feature_Slant angle of handwriting**
   - **Feature_Letter spacing consistency**
   - **Feature_Pen tilt direction**
   - **Feature_Word spacing variability**

---

 This project demonstrates how to establish a connection between everyday information (such as handwriting) and human psychological traits, expanding the boundaries of personality analysis and human-computer interaction. I hope this exploration can provide new ideas for fields such as education, recruitment, and mental health.
