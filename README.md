# Reddit OverWatch - Data collection using Reddit API and Data Cleaning
<img src="https://dynaimage.cdn.cnn.com/cnn/c_fill,g_auto,w_1200,h_675,ar_16:9/https%3A%2F%2Fcdn.cnn.com%2Fcnnnext%2Fdam%2Fassets%2F190626140144-reddit-app-stock.jpg">
# Problem Statement

Problem undertaken to solve is that intentional/unintentional miss categorisation of Reddit users posts with suicide tendencies going unnoticed under **Depression** subreddit category. Its a classification problem. A classification model is needed that predicts the proper category of the post a user written/writing  actually belongs to **Depression** subreddit or **SuicideWatch** subreddit. Accuracy to classify **SuicideWatch** category is important but misclassification of **Depression** is a real concern.

**Links**
[r/depression](https://www.reddit.com/r/depression/)
[r/SuicideWatch](https://www.reddit.com/r/SuicideWatch/)

# Evaluation

Models are evaluated by Classification Accuracy score

Classification Accuracy score=(True Positive + True Negative)/(True Positive + True Negative + False Positive + False Negative)

# Scope

- Using Reddit's API, collect posts from two subreddits of your choosing.
- Use NLP to train a classifier on which subreddit a given post came from.
- This is a binary classification problem.
---

## Requirements
- Gather and prepare your data using the requests library.
- Create and compare two models.
- One of these must be a Bayes classifier, however the other can be a classifier of your choosing: logistic regression, KNN, SVM, etc.
- A Jupyter Notebook with your analysis for a peer audience of data scientists.
- An executive summary of the results you found.
- A short presentation outlining your process and findings for a semi-technical audience.

## Project Deliverables

- A README.md
- Jupyter notebook analysis and models
- Data files
- Presentation slides
- Any other necessary files (images, etc.)
---

## Data Dictionary

|Dataframes:| comp1_df, comp2_df, final_df|
|---|---|

|Feature|Type|Description|
|---|---|---|
|name|object|post index|
|author|object|post author id|
|title|object|title of the post|
|selftext|object|actual body of the post|
|subreddit|int64|parent subedit post belongs to|
