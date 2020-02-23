# Data Science Thesis

Topic: Semantic and Lexical Text representation for Linking Financial Regulations

Submitted in partial fulfillment for the degree Master of Science in Information Studies - Data Science

University of Amsterdam

2018-06-26

ABSTRACT

This research paper aims to use semantic and lexical text representation to find implicit references within the REGULATION (EU) No 575/2013, also known as "Capital Requirements Regulation" [9]. The models were tested by removing direct references from the regulation, which were then used as a labels for the correct identification of topical links between articles.

Several methods were explored: K-means clustering based on TF-IDF, LDA clustering, Logistic Regression, Random Forest, Naive Bayes, Support Vector Machines, Multi-layer Perceptron and Extreme Gradient Boosting. The features used were based on TF-IDF, LDA, count vec and common words. The mixture of imbalanced dataset, skewedness of links, and low lexical diversity has made this a very difficult research task. We have found that using the Multi-layer Perceptron and XGBoost on a downsampled dataset led to the highest recall results, while Random Forest on both a upsampled and skewed dataset led to the highest precision results. However, none of the models and features yielded a high combination of recall and precision.
