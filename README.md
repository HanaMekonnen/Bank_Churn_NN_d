# Bank_Churn_NN_d

Project Overview / Objective

In the competitive banking industry, customer churn—the likelihood of clients leaving for other service providers—has a significant impact on revenue and long-term business viability. Banks must identify the behavioral and demographic factors that lead to churn and intervene early with targeted actions.

As a data scientist at the bank, developing a neural network-based classification model to predict whether a customer is likely to leave the bank within the next six months. The goal was not only to maximize predictive accuracy but also to derive actionable insights to support strategic retention efforts by the bank’s leadership.

Approach & Implementation

I followed a systematic, experiment-driven approach to ensure model effectiveness and business value:

🔹 1. Setup and Data Exploration

Imported necessary libraries and loaded the dataset.


Conducted a data overview, understanding key attributes like CreditScore, Geography, Age, Tenure, Account Balance, Number of Products, and whether the customer was active or had a credit card.


🔹 2. Exploratory Data Analysis (EDA)

Performed univariate analysis to understand individual feature distributions and bivariate analysis to assess relationships with churn (Exited variable).


Identified trends such as higher churn among inactive users and certain age groups.


🔹 3. Data Preprocessing

Created dummy variables for categorical features such as Geography and Gender.


Applied data normalization to scale numerical features.


Split the data into training, validation, and testing sets for robust model evaluation.


🔹 4. Model Building and Iterative Improvement

Built a baseline neural network model using SGD optimizer, and evaluated performance using accuracy and loss curves.


Switched to Adam optimizer for faster convergence and better results.


Added dropout layers to reduce overfitting and improve generalization.


Addressed class imbalance by applying SMOTE (Synthetic Minority Oversampling Technique) to the training data.


Built multiple model variations:


Neural network with SMOTE + SGD


SMOTE + Adam + Dropout


Four-layer neural network with Adam + Dropout


Final model: Four-layer neural network with Adam, Dropout, and BatchNormalization for enhanced stability and performance


🔹 5. Model Selection and Evaluation

Compared all models on validation/test accuracy and precision-recall metrics.


Selected the final model based on superior generalization and consistency on unseen data.



RESULT

 ✅ Successfully developed a high-performing neural network model capable of predicting customer churn with high accuracy.

 ✅ Integrated advanced techniques like Adam optimizer, SMOTE, dropout, and batch normalization, resulting in a model that handles data imbalance and overfitting effectively.
 
 ✅ Derived actionable insights, identifying age, account activity, and tenure as key churn indicators.
 
 ✅ Recommendations enabled the bank to prioritize outreach strategies for high-risk customers, ultimately supporting customer retention efforts and improving service alignment with client behavior.
