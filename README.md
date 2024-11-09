# BNNs

Binarized Neural Network (BNN) comes from a paper by Courbariaux, Hubara, Soudry, El-Yaniv and Bengio from 2016. It introduced a new method to train neural networks, where weights and activations are binarized at train time, and then used to compute the gradients. 

This way, memory size is reduced, and bitwise operations improve the power efficiency. GPUs consume huge amounts of power, making it difficult for neural networks to be trained on low-power devices. BNNs can reduce power consumption by more than 32 times.

The paper showed that a binary matrix multiplication can be used to reduce the train time, which made it possible to train BNN on MNIST 7 times faster, achieving near state-of-the-art results.

I have used the **larq** library from Tensorflow as it provided the best results, with easy to read documentation and user-friendly implementation.

First I compared CNNs and BNNs on the MNIST dataset, and then worked further on BNNs.

Link to the original [paper](https://arxiv.org/pdf/1602.02830.pdf) .
