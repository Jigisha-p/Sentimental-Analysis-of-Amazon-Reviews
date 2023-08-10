# Sentiment Analysis of Amazon Reviews


### Problem Statement:

Over 34,000 consumer reviews for Amazon brand products like Kindle, Fire TV Stick and more are provided.
The dataset has attributes like brand, categories, primary categories, reviews.title, reviews.text, and the sentiment. Sentiment is a categorical variable with three levels "Positive", "Negative“, and "Neutral". For a given unseen data, the sentiment needs to be predicted. The project is designed to predict Sentiment or Satisfaction of a purchase based on multiple features and review text.<br>

### Steps:

<b>Class Imbalance Problem:</b>

1. Perform an EDA on the dataset.

- See what a positive, negative, and neutral review looks like

- Check the class count for each class. It’s a class imbalance problem.

2. Convert the reviews in Tf-Idf score.

3. Run multinomial Naive Bayes classifier. Everything will be classified as positive because of the class imbalance.

<b>Tackling Class Imbalance Problem:</b>

4. Oversampling or undersampling can be used to tackle the class imbalance problem.

5. In case of class imbalance criteria, use the following metrices for evaluating model performance: precision, recall, F1-score, AUC-ROC curve. Use F1-Score as the evaluation criteria for this project.

6. Use Tree-based classifiers like Random Forest and XGBoost.

Note: Tree-based classifiers work on two ideologies namely, Bagging or Boosting and have fine-tuning parameter which takes care of the imbalanced class.

<b>Model Selection:</b>

7. Apply multi-class SVM’s and neural nets.

8. Use possible ensemble techniques like: XGboost + oversampled_multinomial_NB.

9. Assign a score to the sentence sentiment (engineer a feature called sentiment score). Use this engineered feature in the model and check for improvements. Draw insights on the same.

<b>Applying LSTM:</b>

10. Use LSTM for the previous problem (use parameters of LSTM like top-word, embedding-length, Dropout, epochs, number of layers, etc.)

Hint: Another variation of LSTM, GRU (Gated Recurrent Units) can be tried as well.

11. Compare the accuracy of neural nets with traditional ML based algorithms.

12. Find the best setting of LSTM (Neural Net) and GRU that can best classify the reviews as positive, negative, and neutral.

Hint: Use techniques like Grid Search, Cross-Validation and Random Search

<b> Topic Modeling:</b>

13. Cluster similar reviews.

Note: Some reviews may talk about the device as a gift-option. Other reviews may be about product looks and some may highlight about its battery and performance. Try naming the clusters.

14. Perform Topic Modeling

Hint: Use scikit-learn provided Latent Dirchlette Allocation (LDA) and Non-Negative Matrix Factorization (NMF).<br>

### Setup and Installation:
```bash
pip install --upgrade pip
pip install -r requirements.txt
pip list
```
