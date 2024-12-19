# df_physical-activity-problematic-internet-use
### [DF Project] Child Mind Institute — Problematic Internet Use Relating Physical Activity to Problematic Internet Use


This project analyzes the relationship between physical activity and problematic internet use in children and adolescents. Using machine learning techniques, the goal is to predict levels of problematic internet usage based on physical activity and fitness data from the Kaggle competition: [Child Mind Institute — Problematic Internet Use](https://www.kaggle.com/competitions/child-mind-institute-problematic-internet-use).  

---

## Project Highlights  
- **Dataset**: The dataset includes features such as physical activity metrics, demographics, and health indicators.  
- **Target Variable**: The target variable (`sii`) reflects the severity of problematic internet usage on a scale of 0 to 3.  
- **Imputation**: Missing values were handled using methods such as KNN and Random Forest imputation.  
- **Feature Engineering**: Derived new features like BMI-to-age ratio and internet hours adjusted by age.  
- **Modeling**: Trained regression models to predict `PCIAT-PCIAT_Total` scores and classified them into `sii` levels.  

---

## Workflow  

### 1. Data Exploration  
- Checked for missing values and feature correlations.  
- Visualized relationships between physical activity and internet usage.  
- Used heatmaps and scatterplots to explore feature significance.  

### 2. Preprocessing  
- Dropped irrelevant features (e.g., season and redundant demographic data).  
- Handled missing values using a combination of mean, KNN, and Random Forest imputation.  
- Standardized and encoded categorical variables for modeling.  

### 3. Feature Engineering  
- Created new interaction terms (e.g., BMI scaled by age).  
- Calculated feature correlations to select impactful predictors.  

### 4. Model Development  
- Trained various regression models including **LightGBM**, **Random Forest**, and **Linear Regression**.  
- Fine-tuned hyperparameters for better performance.  
- Predicted `PCIAT-PCIAT_Total` and mapped results to `sii` levels using custom thresholds.  

### 5. Evaluation  
- Evaluated models using **accuracy**, **F1-score**, and **Cohen's Kappa**.  
- Conducted validation and refined the models iteratively.  

---

## Results  
- The model achieved [include key metrics here, such as accuracy or Kappa score].  
- Physical activity during evenings had a strong correlation with problematic internet usage.  
- Feature engineering improved prediction accuracy significantly.  

---

## Tools and Libraries  
- **Python**  
- Libraries:  
  - **NumPy**, **Pandas**: Data manipulation and analysis.  
  - **Matplotlib**, **Seaborn**: Data visualization.  
  - **Scikit-learn**, **LightGBM**: Machine learning models.  

---

## How to Run  

1. Clone the repository:  
   ```bash  
   git clone [repository URL]  
   cd [repository folder]  
   ```  

2. Install dependencies:  
   ```bash  
   pip install -r requirements.txt  
   ```  

3. Run the notebook:  
   ```bash  
   jupyter notebook df-physical-activity-problematic-internet-use.ipynb
   ```  

---
