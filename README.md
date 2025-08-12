# Theoretical Statistics Project

This project explores the relationships between student lifestyle habits and academic performance.  
Using both **classical statistical methods** and **modern interpretation tools**, the analysis examines how factors like study time, sleep, exercise, mental health, and entertainment habits (for instance: Netflix and social media use) relate to exam scores.

The work combines **course tools** (Spearman correlation, linear regression, non-parametric tests) with additional methods such as SHAP value analysis for feature importance.


## Data
- **Dataset**: Simulated data
- **Features**:
  - `study_hours_per_day`
  - `sleep_hours`
  - `exercise_frequency`
  - `mental_health_rating`
  - `attendance_percentage`
  - `social_media_hours`
  - `netflix_hours`
  - `exam_score` (target)

---

## Methods
- **Exploratory Analysis**  
  - Spearman rank correlations between predictors and exam scores  
  - Visual correlation heatmaps

- **Regression Models**  
  - Ordinary Least Squares (OLS)  
  - Best subset selection  
  - SHAP-based feature importance

- **Hypothesis Testing**  
  - Mann–Whitney U-test for Netflix usage groups  
  - Sobel test for mediation (social media → sleep → exam score)  
  - Interaction analysis (moderation) for mental health × exercise

---

## Key Results
- **Strong positive** association between study hours and exam score.
- **Moderate positive** effect of mental health and exercise.
- **Negative** effect of heavy social media and Netflix usage.
- Netflix-heavy group scored **lower on average** (rank-biserial correlation: -0.15).

---

## Visualisations
- **Correlation heatmap** for all numeric variables
- **Boxplots** comparing Netflix groups
- **SHAP value plots** for feature importance
- **Predicted vs actual exam score scatter plot**
- **Regression diagnostics** (residual and Q–Q plots)

---

## How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/yaeliavni/Projects-DeepLearning-StatisticalModels.git
   ```
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn statsmodels scipy missingno networkx IPython graphviz scikit-learn shap
   ```
3. Run the script:
   ```bash
   python theoretical_statistics_project.py
   ```

---

## Notes
- The dataset is **simulated**.
