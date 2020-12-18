# Bird Bible: Bird Call Classification
### Authors: Ben Spilsbury

## Overview

The data science team investigates how to create a model to correctly identify bird species by audio recordings of their respective calls. For MVP analysis, only three bird species are considered in the data set. Three models are produced; these are a simple decision tree, an ensemble of a decision tree and a random forest, and finally a sequential neural network. The ensemble model performs the best with an accuracy of ~47%, but there exists much room for improvement. The key focus for next steps and model betterment is integrity of the training data set.


## Business Problem

Build a web app that allows users to record actual bird calls in real time and, with this recording, identifies the encountered species. This app will lower the barrier to entry for birding as a hobby.

## Data

Online repository xeno-canto is used to extract over 1,000 bird call recordings of cardinals, blue jays, and gold finches. These recordings are in .wav format.

## Method


### Feature Engineering

Six frequency and volume output features are engineered to serve as the basis for the resulting models

### Models

Three models are produced (decision tree, ensemble of decision tree and random forest, and sequential neural network).

### Evaluation

Ensemble model performs best at 0.47 accuracy. This is poor when compared to percent share of majority class. Lack of performance likely due to integrity of user-submitted recordings.

## Conclusions

Poor performance of the model is, again, likely due to high degree of white noise in sample recordings. Recommendation would be to cull a smaller, more representative data set of 'paragon' bird calls and re-execute models.