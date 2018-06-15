Clustering using LDA and TF-IDF

3.3.1 Clustering. We used K-means clustering based on TF-IDF
and experimented with 10, 20, 50, 100, 150 clusters. K-means clustering
aims to separate the observations into a specified number
of clusters, in which each observation belongs to the cluster with
the closest mean. This results in the dataset being partitioned into
Voronoi cells. 
We have used the TF-IDF and k-means implementation of scikitlearn
to cluster the articles of the CRR regulation. The entire regulation
was used as the corpus whereas the separate articles were
used as documents of the corpus.

We also used LDA, short for latent Dirichlet allocation, which
is a generative statistical model that automatically discovers the
topics within a document based on the given number of topics. This
is very similar to LSA, short for latent semantic analysis, except
that LDA distributes topics based on Dirichlet prior, which assumes
that documents only have a small set of topics and these topics
only use a small numbers of words. This usually helps to more
precisely assign documents to topics.
The algorithm first assigns every word to a temporary topic, and
then loops through every single word in each document to determine
how prevalent the word is across topics and how prevalent
the topics are in the document. Based on this, it reassigns the topics,
cycling through the entire corpus several times. This iterative
updating leads to the final solution of topics.
We experimented with 10, 20, 50, 100 and 150 LDA topics. We
transformed the outcome into a matrix, which showed the probability
of each article belonging to a given topic. Then based on this
matrix, we clustered the articles to determine topical links between
them
