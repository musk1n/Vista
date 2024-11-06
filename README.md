# Predicting Course Completion for Vidya Vigyan

**Team:** THE MAESTRO  
**Members:** Subhashree Kedia, Shivansh Gupta, Muskan  
**Project:** Vista 2024 - Data Beyond Boundaries

## Overview
This project aims to predict course completion rates for Vidya Vigyan, leveraging data-driven insights into student engagement patterns and performance metrics. Our goal is to identify factors driving course success and provide actionable recommendations to enhance user engagement.

## Key Findings
1. **Engagement Hours and Content Consumption**: Students with 35-45 engagement hours and 7-10 units of content consumed are more likely to succeed.
2. **Assessment and Performance**: More than four assessments taken with a performance metric above 75 correlate with higher completion rates.
3. **Access Mode & Pathway Types**: These factors did not significantly impact course success, which was counterintuitive to our expectations.

## Analysis Techniques
- **Exploratory Data Analysis (EDA)**: Provided insights into student behaviors and feature distributions.
- **Survival Analysis**: Helped assess completion likelihood based on engagement hours.
- **ANOVA**: Revealed feature significance in distinguishing between students who complete and those who don’t.
- **Partial Dependence Plots (PDP)**: Identified thresholds for key features impacting success rates.

## Feature Engineering
- **Custom Metrics**: Developed metrics like `InvolvementMetric` and `StudyDedicationIndex` to capture engagement levels in the context of India's competitive education system.
- **Transformation**: Converted features into binary based on PDP thresholds for smoother model training.
- **Feature Validation**: Used correlation matrices and eta squared values to validate newly engineered features.

## Model Selection
- **Algorithms Applied**: Initially experimented with Logistic Regression, Random Forest, Decision Tree, XGBoost, SVM, Neural Network, and Gaussian Naive Bayes.
- **Challenges**: Gaussian Naive Bayes and Logistic Regression performed poorly due to non-normal data distribution.
- **Binary Feature Training**: After transforming features to binary, we achieved higher accuracy with Bernoulli Naive Bayes.
- **Ensemble Methods**: Final model was a Stacking Classifier (Logistic Regression meta-model), achieving 96% accuracy, capturing student behavior effectively.

## Recommendations
1. **Gamification**: Introduce incentives for reaching key milestones and implement performance-based leaderboards.
2. **UI/UX Improvements**: Enhance interactivity on web and mobile platforms to boost user engagement.
3. **Community Building**: Add community features like chat to foster loyalty and motivation.
4. **Targeted Interventions**: Use predictive insights to provide personalized support to students likely to struggle.

## Tools and Libraries
- **Python Libraries**: NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn, XGBoost.
- **Statistical Methods**: ANOVA, Survival Analysis, Eta Square.
- **Ensemble Models**: Voting Classifier, Stacking, and Bagging with XGBoost.

## Appendix
- **Abbreviations**: EDA (Exploratory Data Analysis), ANOVA, SVM (Support Vector Machine), η² (Eta Squared).
- **Model Descriptions**: Overview of Bernoulli Naive Bayes, Logistic Regression, Decision Tree, and other models used.
