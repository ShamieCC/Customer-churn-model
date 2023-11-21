# Customer-churn-model
### This project is about identifying customers that are likely to churn or stop using a service using a logistic regression model.

I used a kaggle dataset for this project https://www.kaggle.com/datasets/blastchar/telco-customer-churn 
The model's prediction belongs to the classes {0,1}, 0 the negative value or no churning, and 1 the positive value or churning. The historical data from each customer is used to assign a probability score of the likelihood of churning. Based on the output, the company would send an email with discounts or other promotions to avoid churning. 

I started with data preparation, that is looking at the data to understand it, checking if columns read correctly, and checking if names and values are uniform. I preprocessed the data by handling missing values, encoding categorical features and spliting the data into training, validation and testing set. I chose logistic regression for the problem and evaluated the model's performance using the validation/testing data and calculated evaluation metrics (accuracy, precision, recall, etc.) then optimized the model's hyperparameters for better performance. I deployed the model for making predictions on new unseen data by turning the jupyter notebook into a python script, saved the model to a pickle file and served the model with flask. I plan on using Docker to manage the environments and deploy to the cloud using Amazon elastic beanstalk. 
