# 📖 About

This repository focuses on data analysis using **Generalized Linear Model (GLM)**, in particular the **Multivariate Logistic Regression** applied to a public dataset from a Portuguese banking institution's marketing campaign.
The aim is to provide an in-depth understanding of the differences in philosophy, methodology, and results between the Frequentist and Bayesian approaches, adhering to proper statistical assumptions to ensure the right interpretation of results.


## Pipeline of the Project:
1. **Data Preprocessing**: The dataset undergoes cleaning, feature selection, and transformation to ensure the quality and relevance of the input variables.
2. **Modeling Approaches**:
   - **Frequentist Approach**: The model is estimated using traditional maximum likelihood estimation methods.
   - **Bayesian Approach**: A probabilistic model is used, incorporating prior beliefs and updating them with observed data using Bayes' theorem.
3. **Model Evaluation**: Both models are evaluated using various performance metrics, including accuracy, precision, recall, F1-score, and AUC-ROC, to assess and compare their predictive performance.
4. **Interpretation**: Careful interpretation of the model's results is emphasized, ensuring that the conclusions drawn are statistically valid and meaningful.


## 📊 Dataset
[Moro S., Rita P., Cortez P. (2014). Bank Marketing UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing) has been used, in particular 'bank.csv' file insted of 'bank_full.csv' for computational reasons.

## 📈 Results

Using the *Covariance Matrix* to eliminate correleated varaibles and *Bayesian Feature Selection using Latent Variables* to to identify the most influential predictors, the model is fitted on a subset that consider: 

 - `housing | Yes`
 - `loan | Yes`
 - `campaign`
 - `previous`

| Covariance Matrix | Bayesian Feature Selection |
|---------|---------|
| ![Image 1](images/covariance.png) | ![Image 2](images/selection.png) |

The model is then fitted to the data using both approaches to obtain the estimates. However data suffers from an issue of unbalanced labels, thus from a predictive perspective, the model result in poor performance concerning the minority class, which is the information of primary interest. This problem could be solved with more advanced techniques.

# 💡 Conclusion
