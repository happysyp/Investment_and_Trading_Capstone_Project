# Capstone Project Overview
In this capstone project, what I’ve learned throughout the Nanodegree program was leveraged to solve a problem of my choice by applying machine learning algorithms and techniques. First, the problem was defined and potential solutions and performance metrics were investigated. Next, the problem was analyzed through visualizations and data exploration to have a better understanding of what algorithms and features are appropriate for solving it. The algorithms and metrics of choice, documenting the preprocessing, refinement, and postprocessing steps were implemented along the way. Afterwards, results were collected about the performance of the models used, visualize significant quantities, and validate/justify these values. Finally, conclusions were constructed about my results, and whether my implementation adequately solves the problem was discussed.

# Capstone Project Highlights
This project was designed to prepare me for delivering a polished, end-to-end solution report of a real-world problem in a field of interest. 

# Things learned by completing this project:

How to research and investigate a real-world problem of interest.
How to accurately apply specific machine learning algorithms and techniques.
How to properly analyze and visualize your data and results for validity.
How to document and write a report of your work.


# Project description
A stock price indicator has been built using machine learning as the capstone project of Udacity machine learning nanodegree program.
Investment firms, hedge funds and even individuals have been using financial models to better understand market behavior and make profitable investments and trades. A wealth of information is available in the form of historical stock prices and company performance data, suitable for machine learning algorithms to process.
For this project, I built a stock price predictor that takes daily trading data over a certain date range as input, and outputs projected estimates for given query dates. 

- data files: ten .cvs files were downloaded from Yahoo! Finance as the data analyzed in this project 
- proposal.pdf: detailed proposal for this project
- **project_report.pdf**: a detailed report (in PDF format) addressing the five major project development stages. 
- **project_implementation.ipynb**: all development Python code used for this project that is required to reproduce the implemented solution and result. Jupyter Notebook was used in this implementation
- environment: major packages used in the implementation of this project includes python 2.6.1, scikit-learn 0.19.0, pandas 0.20.3, matplotlib 2.0.2 and numpy 1.13.1

# Project details

Domain Background
In today's competitive markets, managers are hoping to discover new predictive patterns in data, through technologies like artificial intelligence, to gain an edge over rivals.  Machine learning is an application of artificial intelligence (AI) that allows computer systems to use algorithms to adapt to enable better outcomes, based on data rather than explicit programming.   It excels at finding patterns and making predictions, and used to be the preserve of technology firms. The financial industry has started to make use of it. One of the earliest investors in the industry even forecasted that machine learning poses a threat to equity hedge funds within the next decade as the technique becomes powerful enough to forecast market moves better than humans. 

Machine-learning has found its application in many different areas of finance. It has been applied to spot unusual patterns of transactions, which can indicate fraud. It has been applied in the document-heavy parts of finance, where AI-based systems can be used to recognize text. It is also good at automating financial decisions, like assessing creditworthiness or eligibility for an insurance policy. The newest frontier for machine-learning is in trading, where it is used both to analyze market data and to select and trade portfolios of securities.   This project will utilize machine-learning in this area to build a stock price indicator. 

# Problem Statement
The problem to be solved in this project is to accurately predict the future closing value of a given stock across a given period of time in the future. One potential solution is to utilize supervised machine learning algorithms to predict the future value. This model can be trained using the historical data of different stocks, and the predicted value can be compared with the actual value of these stocks. The percentage difference between the predicted value and the actual value can be used to calculate the accuracy of the model.
# Datasets and Inputs
This project will use open source historical stock price data from Yahoo! Finance. Yahoo finance provides a relatively simple process of obtaining basic financial information. Information available includes financial statements and price and volume data. CSV files can be obtained through its website about the data, and web API is available. 

Although data from Yahoo is free, the accuracy of its information is reliable.  Actually, a study by (Flanegin, et al 2009) suggested that Yahoo Finance data was acceptable for research purposes. The dataset will be imported and processed in the project. It will be split into training and testing set. The features in the dataset will be used to train the models and make prediction.
# Solution Statement
The solution to the problem is the predicted closing price across a given time in the future, based on the input data of a certain period of data for a certain stock. A good machine learning model should be able to make relatively accurate prediction for the future price of a given stock. The percentage difference between the predicted price and the actual price can be used as the metric of how well the model works.

# Benchmark Model
Stock market indexes are usually used as the benchmark for stock market prediction.  In this project, I used S&P 500 index as the benchmark. In this benchmark model, the price of a given stock will be calculated assuming the stock moves the same way as the S&P 500 index does. The predicted closing price across a period of time in the future is calculated as the product of the closing price of the last day of the input date and the percentage change of S&P 500 index across this period of time. This predicted price from the benchmark model will be compared with the predicted price from the machine learning model. 
Evaluation Metrics
The measures of performance for this project will be the percentage difference between predicted and actual closing values of the target stock. For more input of more than one stock, the mean percentage difference will be used as the metric.

# Project Design
The project was implemented with Python notebook and the corresponding python machine learning packages. It includes the following different stages.
1.	Setting Up Infrastructure
Python notebook and corresponding Python packages such as sklearn were imported
2.	Data preparation and exploration
Stock data was imported from csv, and the data was explored by calculating statistics and making plots. The data was also split into training model and testing model.
3.	Develop supervised learning model
Models such as linear regression and KNN were developed to fit the training data. The model parameters was adjusted to avoid overfitting and underfitting.
4.	Model evaluation
The model was tested against testing data. The result was measured against the evaluation metrics and be compared with the benchmark model.
5.	Discussion and conclusion
The result was discussed, and the conclusion was recorded into the project report.


