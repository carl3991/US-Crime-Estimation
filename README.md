# U.S. Crime Analysis & Assault Rate Prediction
<br></br>

### Project Overview
This project analyzes U.S. crime trends from 1979 to 2023 using FBI Summary Reporting System (SRS) data. The primary goal is to predict the aggravated assault rate per 100,000 people across U.S. states by leveraging historical crime patterns, state-level differences, and temporal trends.
<br></br>

### Problem Statement
Crime remains a persistent social issue, and understanding how aggravated assault evolves over time can help agencies anticipate risk and allocate resources. The task is to build a model that predicts state-level assault rates, using:

* Previous year’s aggravated assault (lag feature)
* State Name
* Year
  
The challenge includes multicollinearity among crime variables and strong state-level variation


### Modeling Approach
The final model selected was XGBoost Regression, chosen for its ability to handle:

* Nonlinear relationships

* High-dimensional one-hot encoded features

* Temporal and categorical interactions

<blockquote> The model performed strongly on the test set with an **R² of 0.935** and a **RMSE of 36.56** assault incidents per 100k population.</blockquote>blockquote>
<br></br>

### Feature Importance Insights
* State identity was the most influential predictor, indicating that geographic differences dominate assault-rate patterns. 

* Lagged assault rate ranked 8th, showing moderate predictive value.

* Year ranked 22nd, suggesting weak national time trends compared to state-level variation

* <br></br>

# Conclusion
* Crime patterns vary far more by state than by year.

* Historical assault levels help, but not as strongly as geographic factors.

* XGBoost provides a robust framework for predicting state-level assault rates.

* This analysis can support agencies in identifying states at higher risk of rising aggravated assault
