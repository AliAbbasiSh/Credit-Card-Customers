<h2> Credit Card Customer Classification</h2>
<h4> Project Description </h4>
<p> 
This project tries to classify credit customer of a bank based on whether they are going to churn. The dataset is obtained from <a href='https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers'>Kaggle.</a> and it contains different customer features alongside whether or not they are an existing customer.<br>
</p>
<h4> Step-by-Step Solution </h4>
<p>
The following steps are used to identify and classify the customers:<br>
<ol>
<li> <strong> Explanatory Data Analysis: </strong> In order to better understand different features, the relationship with each other, and their impact on the output, explanatory data analysis is conducted </li>
<li> <strong> Feature Selection: </strong> Another approach to identify the impact of each feature on the output (customer churning) is feature selection using metrics such as p-value </li>
<li> <strong> Data Preprocessing: </strong> To process the data with machine learning classification models the categorical data has to be transformed into numerical data and scaled to better balance the impact of different features </li>
<li> <strong> Model Selection and Training: </strong> The best model is selected based on f1 score is selected and trained on the data for the classification </li>
</ol>
</p>
<h4> Explanatory Data Analysis</h4>
<p>
First of all, the distribution of the customer churn is investigated as it can be seen in the following image.<br>
<br>
<img src='https://github.com/AliAbbasiSh/Credit-Card-Customers/blob/main/download.png' ><br>
<br>
following that, the number and percentage of existing and attrited customer from each categorical feature are illustrated.<br>
<br>
<img src='https://github.com/AliAbbasiSh/Credit-Card-Customers/blob/main/Categorical%20Features.png'><br>
<br>
<img src='https://github.com/AliAbbasiSh/Credit-Card-Customers/blob/main/Categorical%20Feature%20Percentages.png'><br>
<br>
The effect of some of the features are obvious in this graphs (for example female customers are more likely to leave the bank).
</p>
<h4> Feature Selection</h4>
<p>
In order to further determine the effect of each feature on the result, feature selection using hypothesis testing is done on categorical features and as it can be seen from the two screen-shots of some of the results we can conclude that gender ahd customer churning are related whereas card_category and customer churning are unrelated.<br>
<br>
<br>
<img src='https://github.com/AliAbbasiSh/Credit-Card-Customers/blob/main/Screenshot%202022-08-05%20135835.png'><br>
<br>
<img src='https://github.com/AliAbbasiSh/Credit-Card-Customers/blob/main/Screenshot%202022-08-05%20135929.png'><br>
<br>
</p>
<h4> Data Preprocessing</h4>
<p>
The next step is to transform categorical data into numerical ones. For the Attrition_Flag which is the main result column, simple label encoding is conducted. For other features (gender,marital_status,card_category) we used one-hot encoding and for categorical features which represented values(higher income category means higher spending power) ordinal encoding was utilized. Some of these features can be seen before and after transformation. <br>
<br>
<br>
<img src='https://github.com/AliAbbasiSh/Credit-Card-Customers/blob/main/Screenshot%202022-08-05%20141941.png'><br>
<br>
<img src='https://github.com/AliAbbasiSh/Credit-Card-Customers/blob/main/Screenshot%202022-08-05%20142036.png'><br>
<br>
<img src='https://github.com/AliAbbasiSh/Credit-Card-Customers/blob/main/Screenshot%202022-08-05%20142055.png'><br>
<br>
</p>
<h4> Model Selection and Training</h4>
<p>
For the model selection we trained the data on some of the mostly used classification methods (K-neighbor,decision tree, xg boost, SVM, and random forest) and compared the f1 scores<br>
<br>
<br>
<img src='https://github.com/AliAbbasiSh/Credit-Card-Customers/blob/main/Screenshot%202022-08-05%20143053.png'><br>
<br>
As it can be seen XGBoost has the best score and as a result a randomized gridsearch is conducted to find the optimum hyperparameters for the best score.
<img src='https://github.com/AliAbbasiSh/Credit-Card-Customers/blob/main/Screenshot%202022-08-05%20143355.png'><br>
<br>
In conclusion, we were able to achieve an f1 score of 0.98 using XGBoost for our classification
</p>

