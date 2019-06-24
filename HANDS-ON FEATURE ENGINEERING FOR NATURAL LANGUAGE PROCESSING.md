# HANDS-ON FEATURE ENGINEERING FOR NATURAL LANGUAGE PROCESSING
Susan Li
Sr. Data Scientist at Kognitiv (also on Medium)

## NLP is so difficult
Context and meaning can be difficult to ascertain by machines. 

## Meta and Text Features
* Number of words in the text
* N-Grams

> At the end of the day, some ML projects succeed and some fail. The difference is oftentimes the features chosen. 

Feature engineering is the most importatn part of developing NLP applications

## Feature Engineering for NLP
### Problem 1: Predict label of a Stack Overflow question

https://storage.googleapis.com/tensorflow-workshop-examples/stack-overflow-data.csv

Our problem is best formulated as multi-class single label text classification which predicts a given Stack Overflow question classification. 

A TF-IDF computation of the wrod "python"

```math
documents_total/docs_with_python mentioned = Tf*idf
```

Word2vec: 
- CBOW: neighbors 
- Skip-gram: self

Fastext: An extension of Word2vec

### Problem 2: Topic Modeling (unsupervised)

Filter out undesirable words and/or sentences. 


### Problem 3: Auto detect duplicate Stack Overflow questions
Problem formulation: binary classification problem which we identify and classify. 

FuzzyWuzzy: a Fuzzy feature library on github. 
- https://github.com/seatgeek/fuzzywuzzy

Word mover's distance:
> How far apart two documents are
- markroxor.github.io/gensim/static/notebooks/wmd_tutorial.html

## The Future of Feature Engineering
More and more automation to select features. 

But how do we explain Auto ML models? Use of LIME and SHAP can help us understand our models. 

Resources for Feature Engineering
* Glove
Word2vec

## Other thoughts
DevOps
AI
Software Architecture



