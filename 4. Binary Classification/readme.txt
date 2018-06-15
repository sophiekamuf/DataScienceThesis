3.3.2 Binary Classification. 

We then decided to convert this problem to a binary classification problem 
creating article pairs and assigning the label 1 to article pairs 
with a link and label 0 to article pairs without a link. 
However, this resulted in a very unbalanced
dataset with 1190 linked pairs and 272.339 unlinked pairs. This
is effectively a ratio of 1:229. We therefore decided to use downsampling
and up-sampling for the training set before applying more
methods. Before doing so, we split the dataset into a training and
test set to ensure that the test set was representative of the 1:229
ratio of linked and unlinked article pairs. For down-sampling, we
took a random sample of the training set’s unlinked articles pairs
in order to create a 1:1 ratio between linked and unlinked pairs.

For up-sampling, we used scikit-learn’s resample method to create
more examples of the minority group of linked pairs.
We created a total of 8 features:

(1) Cosine of TF-IDF
(2) Cosine of TF-IDF bigrams
(3) Cosine of TF-IDF trigrams
(4) Cosine of count vec
(5) Cosine of 50 LDA topics
(6) Cosine of 100 LDA topics
(7) Cosine of 200 LDA topics
(8) Common words

In machine learning, no one algorithm works best for every
single problem, which is why we decided to apply a variety of
algorithms:

(1) Logistic Regression
(2) Random Forest
(3) Extreme Gradient Boosting
(4) Naive Bayes
(5) Support Vector Machines
(6) Multi-layer Perceptron
