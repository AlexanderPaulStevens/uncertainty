## README 
This repository contains the code for the paper "Learning Uncertainty with Artificial Neural Networks for Improved Predictive Monitoring". There are five notebooks.

"CNN" is the convolutional neural network we used in our experiments.

"LSTM" is the long short-term memory network we used in our experiments

Both "CNN" and "LSTM" rely on the class ConcreteDropout in the "Concrete" notebook.

The "Learning" notebook provides a simplified training mechanism to train the CNN and LSTM models, both for regression and classification.

The "Inference" notebook shows how to do inference with Monte Carlo simulations and to calculate aleatoric and epistemic uncertainty

The loss functions used in "Learning" can be found in "Loss_functions".


## PyTorch
Our neural networks are built with PyTorch. Information and installation instructions can be found on https://pytorch.org/.


## Paper abstract
Artificial neural networks’ inability to assess the uncertainty of their predictions poses a major roadblock towards more widespread adoption. We distinguish two strains of uncertainty, which can both be learned: model uncertainty -caused by a paucity of training data- and noise-induced observational uncertainty. Based on sound mathematical foundations, Bayesian neural networks can learn their predictions’ model uncertainty. Adding one layer to these networks and enriching their loss functions enables the learning of observational uncertainty as well. Our contribution is to introduce these uncertainty concepts to the field of predictive process monitoring. Our experiments show that the uncertainty estimates permit differentiating between more and less accurate predictions and building confidence intervals, both in regression and classification task settings. These conclusions hold from the early stages of running processes. Moreover, the deployed techniques are fast and yield more accurate predictions. Learning uncertainty could increase users’ confidence in their process prediction systems, foster a better cooperation with humans and enable an earlier implementation working with smaller datasets.
