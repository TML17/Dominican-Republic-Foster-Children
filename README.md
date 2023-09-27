# Dominican-Republic-Foster-Children

**Authors:** Brady Vest, Maya Gardner, & Tommy Liu  
**Date:** May 19, 2023

## Project Overview
This project aims to analyze and model data related to child fosterage in the Dominican Republic, exploring a range of socio-economic, demographic, and behavioral variables to predict fosterage status.

## Repository Contents

### Code Files
- **Fosterage_Data_Cleaning.rmd:** Cleans and reshapes the raw data, transforming it into a usable dataset.
- **Fosterage_Model_Selection.rmd:** Contains procedures for forward stepwise selection, backward stepwise selection, and lasso regression.
- **Fosterage_Visualization.rmd:** Houses various visualizations to provide insights into the modeling results.
- **Fosterage_Model_Accuracy.rmd:** Evaluates the accuracy of the models, guiding the choice of the final model.

### Data Files
- **Clean_Data_Training.csv:** Training dataset containing 80% of the cleaned data.
- **Clean_Data_Testing.csv:** Testing dataset containing 20% of the cleaned data.

### Visualizations
![Fixed Effects Visualization](/Code/fixed_effects_vis.png)  
*Fixed effects of each variable with 95% confidence intervals.*

![Odds Ratios Visualization](/Code/odds_vis.png)  
*Odds ratios of each variable with 95% confidence intervals.*

## Methodology
- **Data Cleaning and Transformation:** Leveraged `dplyr` and `tidyr` to reshape raw data, making unique children the primary observations.
- **Model Selection:** Employed forward stepwise selection, backward stepwise selection, and lasso regression to identify the most explanatory variables.
- **Visualization:** Utilized `ggplot2` to generate insightful visualizations, aiding in the interpretation of model results.
- **Accuracy Evaluation:** Assessed model accuracy on training data and generalized results using AUC values.

## Key Metrics and Definitions
- **AUC (Area Under the Curve):** Measures the true positive rate against the false positive rate. A value closer to 1 indicates higher accuracy.
- **AIC (Akaike Information Criterion):** Assesses model quality, considering the number of variables and the model's likelihood. A lower AIC indicates a better model.
- **Percent Accuracy:** Indicates how often the model correctly predicts fosterage status.
- **Odds Ratios:** Used to compare the odds of fosterage between different groups based on predictor variables.

## Insights and Interpretations
- Increasing child age increases the odds of fosterage.
- An increase in mother's age reduces the odds of fosterage.
- Wealthier families and higher education levels of mothers reduce the odds of fosterage.
