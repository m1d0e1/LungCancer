# Lung Cancer Prediction Analysis

## Project Description
This Jupyter notebook analyzes a lung cancer survey dataset to explore patterns and correlations between features like smoking habits, symptoms, and demographics. The goal is to preprocess data for potential predictive modeling of lung cancer risk.

## Dataset
**Source**: [Kaggle](https://www.kaggle.com/datasets/nancyalaswad90/lung-cancer)  
**Features**:
- Demographics: `GENDER`, `AGE`
- Behavioral factors: `SMOKING`, `ALCOHOL CONSUMING`
- Symptoms: `COUGHING`, `FATIGUE`, `CHEST PAIN`, etc.
- Target variable: `LUNG_CANCER` (binary: YES/NO)

**Size**: 309 entries (276 after removing duplicates)

### Key Steps:
1. **Data Loading**:
   - Download dataset using `kagglehub`.
   - Load data with `pandas`.

2. **Data Exploration**:
   - Preview data with `df.head()`.
   - Statistical summary using `df.describe()`.

3. **Data Cleaning**:
   - Remove 33 duplicate rows.
   - Confirm no missing values with `df.isna().sum()`.

4. **Feature Engineering**:
   - Convert `SMOKING` (1→0, 2→1) and `GENDER`/`LUNG_CANCER` to numerical using `pd.get_dummies()`.

5. **Correlation Analysis**:
   - Generate a Spearman correlation heatmap to visualize relationships between variables.


## Results
- **Correlation Insights**: Variables like `SMOKING`, `AGE`, and `YELLOW_FINGERS` show notable correlations with `LUNG_CANCER`.

## Dependencies
- Python 3
- Libraries: `kagglehub`, `pandas`, `numpy`, `matplotlib`, `seaborn`
