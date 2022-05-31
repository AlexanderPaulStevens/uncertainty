## README 
This repository contains the code for the paper "Learning Uncertainty with Artificial Neural Networks for Improved Predictive Monitoring". There are five notebooks.

"CNN" is the convolutional neural network we used in our experiments.

"LSTM" is the long short-term memory network we used in our experiments

Both "CNN" and "LSTM" rely on the class ConcreteDropout in the "Concrete" notebook.

The "Learning" notebook provides a simplified training mechanism to train the CNN and LSTM models, both for regression and classification.

The "Inference" notebook shows how to do inference with Monte Carlo simulations and to calculate aleatoric and epistemic uncertainty

The loss functions used in "Learning" can be found in "Loss_functions".

## Data
Data sources and required preprocessing steps can be found in the repository "https://github.com/hansweytjens/predictive-process-monitoring-benchmarks".

## PyTorch
Our neural networks are built with PyTorch. Information and installation instructions can be found on https://pytorch.org/.


## Paper abstract
The inability of artificial neural networks to assess the uncertainty of their predictions is an impediment to their widespread use. We distinguish two types of learnable uncertainty: model uncertainty due to a lack of training data and noise-induced observational uncertainty. Bayesian neural networks use solid mathematical
foundations to learn the model uncertainties of their predictions. The observational uncertainty can be calculated by adding one layer to these networks and augmenting
their loss functions. Our contribution is to apply these uncertainty concepts to predictive process monitoring tasks to train uncertainty-based models to predict the remaining time and outcomes. Our experiments show that uncertainty estimates allow more and less accurate predictions to be differentiated and confidence intervals to be
constructed in both regression and classification tasks. These conclusions remain true even in early stages of running processes. Moreover, the deployed techniques are fast and produce more accurate predictions. The learned uncertainty could increase users' confidence in their process prediction systems, promote better cooperation between humans and these systems, and enable earlier implementations with smaller datasets
