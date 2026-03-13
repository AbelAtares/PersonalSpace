# Delaney Solubility Prediction with Molecular Descriptors

This project explores the Delaney solubility dataset using molecular descriptors to predict solubility (logS). We implemented a **Linear Regression model** as our main approach and compared it with a **Random Forest model** in the appendix.

---

## Linear Regression Model

### 1. Loading and Preparing Data
- The dataset was loaded from a public repository.  
- We created the variable `X` to store the features used for predicting the target variable.  
- The target variable `Y` contains the solubility values (`logS`).  
- Data was split into training and test sets, with **80% for training** and **20% for testing**.

### 2. Model
- A **Linear Regression model** was created using **Scikit-learn**.  
- The model was trained on the training data and then used to predict values for the test set.

### 3. Model Evaluation
- Predictions were evaluated using different regression metrics, such as **R²**, **MSE** and **RMSE**, to assess the performance of the model.  
- These metrics help quantify how well the model captures the variability of the target variable.

### 4. Data Visualization
- We used **Matplotlib** to plot the predicted vs. actual logS values.  
- Scatter plots provide a visual understanding of how well the model performs and help identify trends and potential deviations.

---

## Appendix: Random Forest

- As an additional experiment, we implemented a **Random Forest model** using **Scikit-learn**.  
- The same train-test split and evaluation metrics were applied to compare its performance with the Linear Regression model.  
- According to the metrics, both models performed similarly.  
- Since Linear Regression is **simpler and more interpretable**, it was concluded to be the most suitable model for this problem.

---

**Conclusion:**  
For the Delaney solubility dataset, a simple Linear Regression model is sufficient to capture the underlying trends in the data. Random Forest did not provide a significant improvement in performance, making the linear model the preferred choice for its simplicity and interpretability.
