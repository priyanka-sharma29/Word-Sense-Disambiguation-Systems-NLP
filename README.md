Word Sense Disambiguation (WSD) is a task to find the correct meaning of a word given context, which can be a building block for various high-level NLP tasks. Two different models are built here to implement WSD systems - Ontological Model & Supervised Model.

## Files Description
* 'Ontological WSD.ipynb' and 'Supervised WSD.ipynb' are the code files where the respective systems have been built.
* 'dictionary.xml' is the XML formatted dictionary that describes commonly used senses for each word.
* 'train.data', 'validate.data' and 'test.data' are the data files on which the classifiers are trained, validated and used for  predicting the sense of a new word, respectively.


## Ontological (dictionary-based) WSD
Dictionary-based approaches utilize definitions given in the dictionary. This WSD system disambiguates the sense by comparing
the definitions and examples of the target word to the relevant words in the context.

There are 2 methods in the dictionary-based approach:
1. Simple Lesk
2. Corpus Lesk

Scoring Model: Given a query word and its feature-represented context, we predict the highest-scored sense in the inventory on the test data.

## Supervised WSD
This WSD system uses a supervised machine learning approach to train classifiers that can tag words in a new unseen text. Naive Bayes classifier has been used to model the probable sense. 

Statistical Model:
Given a query word and its feature-represented context, we predict the most plausible sense in the inventory on the test data.

Smoothing has been implemented to achieve quality performance.
