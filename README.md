# [Volatility model calibration with neural networks a comparison between direct and indirect methods](https://arxiv.org/abs/2007.03494)

In a recent paper "[Deep Learning Volatilities](https://arxiv.org/abs/1901.09647)" a fast 2-step deep calibration algorithm for rough volatility models was proposed: in the first step the time consuming mapping from the model parameter to the implied volatilities is learned by a  neural network and in the second step standard solver techniques are used to find the  best model parameter.

In our paper we compare these results with an alternative direct approach where the the mapping from market implied volatilities to model parameters is  approximated by the neural network, without the  need for an extra solver step. Using a whitening procedure and a projection of the target parameter to [0,1], in order to be able to use  a sigmoid type output function we found that the direct approach outperforms the two-step one  for the data sets and methods published in. 

For our implementation we use the open source tensorflow 2 library with python 3 and the packages given in *requirements.txt*. 

Authors: Dirk Roeder and Georgi Dimitroff

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/roederd/volatility_model_calibration_with_nn/master)
