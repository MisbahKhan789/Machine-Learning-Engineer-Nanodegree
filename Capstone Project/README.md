# Daily News for Stock Market Prediction

Medium Article Post: 

https://carsonzhang.medium.com/build-a-ml-web-app-for-stock-market-prediction-from-daily-news-with-streamlit-and-python-7c4cf918d9b4

# Dataset Overview:

- Time Range of the Dataset: 2008-08-08 to 2016-07-01.
- News data contains crawled historical news headlines from Reddit WorldNews Channel (/r/worldnews). They are ranked by reddit users' votes, and only the top 25 headlines are considered for a single date.
- Stock data: Dow Jones Industrial Average (DJIA) is used to "prove the concept".
- For task evaluation, please use data from 2008-08-08 to 2014-12-31 as Training Set, and Test Set is then the following two years data (from 2015-01-02 to 2016-07-01). This is roughly a 80%/20% split.

# Project Summary:

I am very proud to complete this project because it challenged my skills not only in Machine Learning Engineering but also in domains such as Data Engineering and Software Engineering. I managed to learn how to use the Streamlit library in Python to build my whole ML Web app. On the web interface, you can simply start from choosing your ML model type, then adjusting hyperparameters of the model and finally selecting your evaluation metrics.

Random Forest Model & Logistic Regression Model are tested as benchmark models first and only Random Forest Model is used for further refinement steps.
Before refinement, RF model is evaluated by the classification report method and achieves an accuracy of 81%. However, after using refinement method including GridSearch CV, the RF model successfully improves its accuracy by an increment of 3% to 84%.

# Benchmark Model:

- Random forest
- Logistic Regression 

# Evaluation Metrics:

- classification report
- confusion matrix
- accuracy score 

Final model results will go through model tuning steps for the highest accuracy. Tuning methods including: GridSearchCV. 

# Project Outline:

- Data Preprocessing (filling NaN values; combining headlines columns)
- NLP Preprocessing (removing punctuations; changing texts to lowercases; tokenization)
- ML Pipeline (applying countvectorizer to all the headlines; applying ML models)
- Model Tuning (utilizing GridSearchCV to achieve higher accuracy)
- Model Comparing (comparing final results between tuned and benchmark models)
- Converting the whole process into a ML pipeline 
- Presenting as a user-friendly ML web app (By using Streamlit Python Library)





