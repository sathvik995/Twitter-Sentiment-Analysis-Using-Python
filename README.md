# Twitter-Sentiment-Analysis-Using-Python
Twitter Sentiment Analysis uses NLP and machine learning to classify tweets as positive, negative, or neutral. This project processes tweets individually or as part of a larger dataset to understand emotions and opinions.

## Dataset Details

The dataset used is the Sentiment140 Dataset, containing 1,600,000 tweets extracted via the Twitter API. The columns in this dataset are:

- **target**: The polarity of the tweet (positive or negative)
- **ids**: Unique ID of the tweet
- **date**: The date of the tweet
- **flag**: The query (if no query exists, it's "NO QUERY")
- **user**: The name of the user who tweeted
- **text**: The text of the tweet

## **You can dowload the dataset from here** 👉 : https://www.kaggle.com/datasets/kazanova/sentiment140

## Project Pipeline

The steps involved in the machine learning pipeline are:
1. Import necessary dependencies
2. Read and load the dataset
3. Perform exploratory data analysis (EDA)
4. Visualize target variables
5. Preprocess the data
6. Split data into train and test sets
7. Transform the dataset using TF-IDF Vectorizer
8. Create a function for model evaluation
9. Build the model
10. Evaluate the model


## Model Evaluation

### Accuracy
- **Logistic Regression** performs better than **SVM**, which in turn performs better than **Bernoulli Naive Bayes**.

### F1-score
- **Class 0**:
  - Bernoulli Naive Bayes: 0.90
  - SVM: 0.91
  - Logistic Regression: 0.92
- **Class 1**:
  - Bernoulli Naive Bayes: 0.66
  - SVM: 0.68
  - Logistic Regression: 0.69

### AUC Score
- All three models have the same ROC-AUC score.

## Conclusion
- **Logistic Regression** is the best model for this dataset.
- Following Occam’s Razor, Logistic Regression is the simplest and most effective model due to the lack of assumptions in the dataset.


- This project demonstrates how Twitter Sentiment Analysis can be used to understand public emotions in tweets. We preprocess the data and feed it into ML models to achieve the best accuracy.

### Key Takeaways

- **Twitter Sentiment Analysis** identifies and classifies sentiments in text.
- **Logistic Regression**, **SVM**, and **Naive Bayes** are effective algorithms for this task.
