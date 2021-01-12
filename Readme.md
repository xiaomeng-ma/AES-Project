# Automated Essay Scoring (AES) using Word Frequency Distribution

## What is this project?

Automated Essay Scoring (AES) is an NLP application that assigns grades to essays. The two common approach for AES systems are feature-based and neural network. The feature based models try to evaluate essays from different dimensions including grammar, vocabulary, style, organization, cohesion and coherence. This project explores on a new feature, word-frequency distribution, and combining it with the neural network to improve the performance of the AES system. 

## Summary
### Data
TOEFL 11 Corpus

### Word-frequency distribution
For human languages, one of the most puzzling and also most robust facts is that a few words have very high frequency (e.g. 'a', 'the', 'of') and many words have very low frequency (e.g. 'ravioli', 'accordion'). This distribution roughly obeys a power law known as Zipf's law. In a Zifpian distribution, the frequency of a word (f) is inversely proprotional to its rank (r): f = \frac{C}{r^2}, where C is a constant and s is the power to which r is raised. The parameters (C,s) in Zipf's law can be used to measure linguistic complexity. In this project, the word frequencies in each essay were first fitted to a Zipfian distribution and a lognormal distribution to generate the best-fitting parameters. 

### Input
Zipfian parameters, lognormal parameters, the essays

### Output
A grade (which is compared to human rated grades)

### Model
Logistic regression (Zipfian parameters, lognormal parameters) + LSTM/Transformer


## Publication
In preparation
