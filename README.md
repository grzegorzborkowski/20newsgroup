# 20newsgroup

This repository contains processed The 20 newsgroups text dataset and MNIST dataset. The processing has been done 
for the purpose of propery visualization of the datasets.

The 20 newsgroup dataset was transformed by using the bag of word technique. The dataset after transformation consists of
two files: 20groups_bag_of_words.csv (containing mapping from number of documents to indices of words and occurences of those words
in particular document) and 20groups_word_mapping.csv (containing mapping from a word to a key used in 20groups_bag_of_words.csv)

The MNIST dataset was transformed as follows:
Firsty calculated nearest neighbours graph(k=20) - mnist_knn_*.csv, 
then calculated degrees of nodes in the graph (files mnist_knn_*_counts.csv)
then performed PCA, keeping 30 most relevant components and then applied TSNe keeping three components, saving the results
to mnist_*.csv files

