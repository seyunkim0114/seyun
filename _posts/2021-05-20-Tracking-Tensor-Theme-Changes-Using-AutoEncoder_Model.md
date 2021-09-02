---
title: Tracking Theme-change in Streaming Tensor Using AutoEncoder
layout: single
---
Tensor is a multi-dimensional array that can be useful for storing data with variety of features. However, as the size and dimension of a tensor grows, the harder it becomes to interpret and extract meaningful information from the noisy bulk of data. To address this issue, many researches are being done to track trend changes in tensors. This post will introduce a new attempt to captures trend changes in tensors using autoencoder.

Autoencoder is a type of neural network trained to copy its input to its output. In detail, the encoder network of autoencoder encodes the given input to a lower dimensional feature vector (although does not always have be a vector). During this process, encoder learns to compress the input so that the encoded vector only contains important information. The decoder network, then, takes the encoded vector as its input and tries to reconstruct the original input of autoencoder. Through this encoding and decoding process, the autoencoder network learns to extract the essence of the input data. The proposed method for theme tracking is based on this very ability of autoencoder.

![Image not available at the moment](autoencoder-architecture.png "AutoEncoder Network")
