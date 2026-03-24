# AG-news-text-classification
Recurrent Neural Network (RNN) and Long-Short Term Memory networks (LSTMs) trained to classify text data into 4 categories from the AG news dataset

## Abstract
This paper explores the performance of Recurrent Neural Networks (RNNs), Long-Short Term
Memory networks (LSTMs), and Convolutional Neural Networks (CNNs) at text classification
for news articles. Different model architectures are implemented to understand their effects on
model performance. This research uses the AG news dataset containing 120,000 and 7,600 news
articles across 4 categories for training and testing. TensorFlow and Keras are used to build the
models and NTLK is used to pre-process the text data. The best performing model of this
research uses 96 tokens for the top 1000 most frequent tokens in the corpus. It has an embedding
size of 256, bidirectional and dense layers with 128 nodes and 2 dropout layers (0.3, 0.5). It ran
for 5m and had a testing accuracy of 88% and loss of 0.33. The loss curves show an appropriate
fitting model and confusion matrix shows a great classification accuracy of articles to their
labeled classes.

## Methods
This research is conducted using the AG news dataset, which is split into 114,000 articles for
training, 6,000 for validation, and 7,600 for testing. The main libraries are Tensorflow (v 2.18.0),
Keras (v 3.8.0), NLTK, matplotlib, and scikit-learn libraries. The experiment is run on Google
CoLaboratory using T4 GPU.
In each experiment, one hyperparameter is tweaked to find a model with the best accuracy, loss
score, RMSE, and correct classification of the articles with the labelled class. All models are run
for 10 epochs in a batch size of 32. Rmsprop is used as the optimizer and Sparse Categorical
Cross Entropy is used for loss.

The articles in this dataset are tokenized using NLTK and stopwords are downloaded from
NLLK’s English stopwords. The accuracy and loss for training, validation, and testing, confusion
matrix are calculated and visualized with matplotlib.

13 models trained and compared
