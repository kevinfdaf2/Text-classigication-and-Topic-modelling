# Text-classigication-and-Topic-modelling


## Data description


The content has been gathered from the popular academic website arXiv.org for articles tagged as computer science content (though some of these are in mathematics or physics categories). Training is 1990-2014 and testing is 2015 plus a bit of 2016. The fields are:


  - ID: a unique alphanumeric ID.
  - URL: a working URL if you prepend "http://".
  - Date: the date in format YYYY-MM-DD.
  - Title: the full title, though with non-ASCII characters modified and any "," deleted.
  - InfoTheory: a "1" if it is classified as an Information Theorey article, otherwise "0".
  - CompVis: a "1" if it is classified as a Computer Vision article, otherwise "0".
  - Math: a "1" if it is classified as a Mathematics article as well, otherwise "0".
  - Abstract: the full abstract, though with non-ASCII characters modified.


## Model


The variations we would like to consider are:
  1. Task: 3 Boolean tasks
  2. Algorithm: use 2 different algorithms from tutorials, use the RNN and then choose one of the statistical classifiers (SVN, logistic regressions, etc.); you may use another classifier but it should be readily available in Python, and it is not expected
  3. Text preprocessing: do 2 different versions of your choosing (for instance one version might be snowball stemming, no stopwords, delete numbers, convert all letters to lowercase, etc.)
  4. Data size: train on the first 1000 cases in the training set only, then train on all in the
training set.


So this makes 3 by 2 by 2 by 2 different configurations. For each configuration test the algorithm on the test set provided and report the following:
  - F1, precision, recall
  - precision-recall curve



## Topic Modelling

Two variations might be:


  - different pre-processing of text or vocabulary
  - use of bi-grams or not
  - different numbers of topics (e.g., K=10, K=40)


Now run these two on the first 1000 and the first 20,000 articles in the training data set. This means there are 2 by 2 different configurations for the LDA runs. Then make visualisations of some kind in the notebook. These should allow you to analyse and interpret the output of the topic models. The actual discussion (analysis and interpretation) about the results should not appear in the notebook but be in the separate PDF discussion report. This is a 2 page discussion giving your analysis and findings that were presented in the notebook output. 

Find out more in the report.pdf file.
