# 📖 About

This repository focuses on data analysis using different statistical methodologies applied to a public dataset from a Portuguese banking institution's marketing campaign. **Generalized Linear Model (GLM)** have been implemented, in particular the ** Multivariate Logistic Regression**.

The main objective is to provide an in-depth understanding of the differences in philosophy, methodology, and results between the Frequentist and Bayesian approaches, adhering to proper statistical assumptions to ensure the right interpretation of results.


## Pipeline of the Project:
1. **Data Preprocessing**: The dataset undergoes cleaning, feature selection, and transformation to ensure the quality and relevance of the input variables.
2. **Modeling Approaches**:
   - **Frequentist Approach**: The model is estimated using traditional maximum likelihood estimation methods.
   - **Bayesian Approach**: A probabilistic model is used, incorporating prior beliefs and updating them with observed data using Bayes' theorem.
3. **Model Evaluation**: Both models are evaluated using various performance metrics, including accuracy, precision, recall, F1-score, and AUC-ROC, to assess and compare their predictive performance.
4. **Interpretation**: Careful interpretation of the model's results is emphasized, ensuring that the conclusions drawn are statistically valid and meaningful.


## 📊 Dataset
[Moro S., Rita P., Cortez P. (2014). Bank Marketing UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing) has been used, in particular 'bank.csv' file insted of 'bank_full.csv' for computational reasons.

# 📈 Results

The two models are fitted with a subset of variables obtained from a *Bayesian Feature Selection using Latent Variables*. 

From the predictive perspective the model suffer of unbalanced label issue, leading to poor performance w.r.t. our minority class witch is the information of interest. Several techniques could be implemented but are not the focus of this analysis.

# 💡 Conclusion
