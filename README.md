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
following that, the number and percentage of existing and attrited customer from each categorical feature are illustrated.
<img src='https://github.com/AliAbbasiSh/Credit-Card-Customers/blob/main/Categorical%20Features.png'><br>
<img src='https://github.com/AliAbbasiSh/Credit-Card Customers/blob/main/Categorical%20Feature%20Percentages.png'><br>

</p>




