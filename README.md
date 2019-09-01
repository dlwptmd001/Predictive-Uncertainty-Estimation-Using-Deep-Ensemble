# Predictive-Uncertainty-Estimation-Using-Deep-Ensemble
## Introduction
This repository is for implementation of the paper [Simple and Scalable Predictive Uncertainty Estimation using Deep Ensembles](https://arxiv.org/abs/1612.01474). This algorithm quantifies predictive predictive uncertainty in **non-Bayesian NN** with *Deep Ensemble Model*.  

Contribution of this paper  
- Describes simple and scalable method for estimating predictive uncertainty estimates from NN.
- Propose a series of tasks for evaluating the quality of the predictive uncertainty

This paper uses 3 things for training
- proper scoring rule
- adversarial training to compare other predictive distributions with others
- Deep Ensemble

This repository is implemented for verifying figure 6 without adversarial training.

I trained a network on MNIST and test in on a mix of test examples from MNIST(known classes) and NotMNIST(unknown classes), 9000 examples from each class.
![Deep Ensemble vs MC Dropout](https://user-images.githubusercontent.com/49624517/62756661-91d3cd00-bab3-11e9-9eae-2fa0f5f94668.png)

***As shown above, MC-dropout can produce overconfident wrong predictions as evidenced by low accuracy, whereas deep ensembles are significantly more robust.***


 Code is originally from @github/kyushik, but modified.
