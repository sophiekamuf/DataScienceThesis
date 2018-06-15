3.3.4 Ranking. We also performed ranking based on the downsampled
training set of article pairs, which was described in Section
3.3.2, using the aforementioned eight features:

(1) Cosine of TF-IDF
(2) Cosine of TF-IDF bigrams
(3) Cosine of TF-IDF trigrams
(4) Cosine of count vec
(5) Cosine of 50 LDA topics
(6) Cosine of 100 LDA topics
(7) Cosine of 200 LDA topics
(8) Common words

and applying the following four algorithms:

(1) Logistic Regression
(2) Random Forest
(3) Naive Bayes
(4) Support Vector Machines

Instead of predicting a binary variable as in Section 3.3.2, we
now predicted the probability of a link between two articles. We
then ranked the probabilities to determi
