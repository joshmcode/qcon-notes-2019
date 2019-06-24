# MACHINE-LEARNED INDEXES - RESEARCH FROM GOOGLE
Alex Beutel

## Introduction
One size does not fit all 

* Traditional data structures make no assumptions about your data. 

* Scales to O(n)

## B-Trees
B-trees are models

key -> Model -> ouput

This is equivalent to modeling the CDF

### Potential Advantages
* 300ns (B-Tree) compared to 80,000ns (model from TF)

Multiple problems arose: 
- Problem 1: Tensorflow is designed for large models
- Problem 2: B-Trees are great for overfitting
- Problem 3: B-Trees are cache efficient
- Search doesn't take advantage of a prediction

### Goals of talk
> How do we get the same degree of speed out of a model that we would get out of a B-Tree search. 

> How do we scale accuracy with size? 

> Thinking of traditional data structures as models

> Use hybrid ML models / traditional structures to get real meaningful benefits. 

## Hierarchicl Experts
Decouple model size and complexity. In this way we can swap out the Binary Tree. 

## Experimentation
Map data: Able to achieve 60% faster at 1/20th the space or 17% faster at 1/100th the space. 

In each case they were able to obtain a significant speedup. 

## Traditional Data Strcuture two: Hash Maps
Hash-Maps as Models 

Relates to conflicts (because conflicts are really expensive).

Refresh: the birthday paradox

## Bloom Filters as Models
Problem: False Negatives

- Use a bloom filter to take the false negatives for all misclassified records. Don't store the ones the model got right. 

### Future 
* Potential: Multidimensional Indexes
* TPUs/GPUs

