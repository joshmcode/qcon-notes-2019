# MLFLOW: AN OPEN PLATFORM TO SIMPLIFY THE MACHINE LEARNING LIFECYCLE
Corey Zumar

> Note

## Overview of ML Development Challenges
* It's complex

Cycle: 
START Raw Data (Azure, Delta, Kafka, MonoDB, Hadoo) -> 
Data Prep (Spark, Python, Pandas) -> 
Training (Pytorch, TensorFlow) -> 
Deploy (Spark, Docker)

We need a lineage around the models that are deployed. 

There are some products tackling these projects. The ones that exist are not open source and internally these products are not easily useable. 

> Can we provide a similar benefit in an open manner? 

## How MLFlow Tackles these challenges
* Works with any ML library & language
* Runs the same way anywhere (cloud)
* Designed to be useful locally or at scale (1 or 1000 people)

## MLFlow components
- Tracking
- Projects
- Models

#### Tracking
Parameters, metics, source (code), version, artifacts, tags and notes

## Demo 

## How to get started
1. Entity (metadata) store
    * FileStore
    * SQLStore
    * REST Store

2. Artifact Store
    * S3, Azure, etc. for storing

## Motivations
MLResults are difficult to reproduce. 

Can execute inside of a Docker container for reproducibility. 

```yaml
my_project/
    - MLproject

    - conda.yaml
    - main.py
    - model.py
```

Run example:

```shell
mlflow run git://<my_project>
```

## MLFlow Models Motivations
Simplify the n * n mappings between products. 

MLFlow is a directory structure. 

> Can run on prem

## Some other thoughts
A simple goal: help my team solve their data problems. Make this one of my goals starting even this year. 

Another goal: ML for factory opimizations. Quote tools. 

What if I spoke to Gene Baker and got access to their data? 

Talk to Tameka about obtaining proprietary access to Intellectual Property I create. 