authorshipattribution-naivebayes
================================

A program to determine the author of a document by using a Naive Bayes Classifier.

    class NaiveBayesClassifier
     |  A program to determine the author of a document by using a Naive Bayes Classifier.
     |   Usage:
     |  >>> aac = NaiveBayesClassifier(labels = ['acd', 'shakespeare'], location = 'documents/')
     |   >>> aac.classify('documents/shakespeare-comedy-merchant.txt')
     |   comedy
     |  
     |  Methods defined here:
     |  
     |   __init__(self, labels, location)
     |      Constructor method to load training data, and train classifier.
     |  
     |   calculateLikelihood(self, word, label)
     |       Method to calculate Likelihood.
     |  
     |  calculatePrior(self)
     |      Method to calculate Prior.
     |  
     |  classify(self, document)
     |       Method to load test data and classify using training data.
     |  
     |  createUnigram(self)
     |      Method to create Unigram for each class/label.
     |   
     |  getDocuments(self, location)
     |      Method to retrieve test data.
     |  
     |  loadDocuments(self, loc, files)
     |      Method to load labeled data from the training set.
     |  
     |  train(self)
     |      Method to train classifier by calculating Prior and Likelihood.
     |  
     |  unigramProbability(self, word, label)
     |      Method to calculate Unigram Maximum Likelihood Probability with Laplace Add-1 Smoothing.