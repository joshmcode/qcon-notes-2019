# Getting-Started-in-Deep-Learning-With-TensorFlow-2.0
Brad Miro

## Deep Learning
Creating models from unstructured data. 

Tensor definition

## Neural Network
- Input layer
- Hidden layers
    * This is what makes the learning "deep" 
    * Neurons responding to edges
    * Neurons responding to shapes
    * Neurons responding to objects
- Output layer

## When to use Deep Learning
* When we have lots of data (Matomo?). 
* When the problem is "complex" speech, vision, natural language (unstructured data)
* When we need the absolute "best" model (99.9% accuracy to 99.99%)

## When to "not" use Deep Learning
- You don't have a large dataset
- When traditional ML methods are working already me
- When data is structred and we posses proper domain knowledge (Matomo?)

## Tensor Flow
Open source deep learning libary from google. It provides utilities to write neural networks. It provides GPU / TPU (Tensor Processing Units) support. It makes the calculus/statistics easier to use. It has more than 2000 contributors. 

It's used all over the world. 41 million downloads and 55k commits. 

## How Google Uses Tensor Flow
- Apply to data center efficiency problems. 
- Google maps
- Augmented reality 
- Portrait mode in Google Pixel
- Music generation
- Medical research (e.g. which eye is healthy and which is not)
- Astronomy (exoplanet predictions)

## Tensor Flow 2.0
It should be easier, more powerful, and more scalable. 

#### Easier:
- Simplified APIs
- Keras
- eager execution (line-by-line)

#### Flexibility
- Servers (TensorFlow Extended)
- Edge (devices)

## Tensor Flow Use
Typical flow: train, export to saved model, and deploy.

## Other Branches
* TF Probability
* TF Text
* TF Ranking
* TF Federated

## TF 2.0 like NumPy
```python
import tensorflow as tf
# Then use
```

## What's Gone
* Session.run
* tf.control_dependencies
* tf.globabl_variables_initializer
* Other things were removed, so I might look at the slides for context

## What's New
* tf.function (wrapper for any Python code)
* Eager execution

## Keras
`keras.io` vs `tf.keras`

```python

# Beginner
model = tf.keras.models.Sequential([
    t.keras.layers.Flatten(),
    tf.keras.layers.Dense(512,activitation='relu')
])

# Expert: 
    # Use traditional Python models and import them
```

## Symbolic vs. Imperative APIs
I am not clear on the basic terminology here

## Distribution Strategies
`tf.distribution.Strategy`

## tensorflow_datasets
Because the datasets are so import, Google makes a bunch of these available to us. 

tensorflow.org/datasets

## Transfer Learning
Reusing models across other datasets because models can be "transferrable." 

See a list at TensorFlow Hub

## What I want to focus on in my career
* AI
* DevOps
* Software Architecture




