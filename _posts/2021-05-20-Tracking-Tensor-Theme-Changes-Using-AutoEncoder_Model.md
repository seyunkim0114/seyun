---
title: Tracking Theme-change in Streaming Tensor Using AutoEncoder
layout: single
---
Tensors are multi-dimensional arrays that can carry a tremendous amount of information. Because of their size and complexity, many methods have been suggested to process them in different ways: decomposition, concept drift, change detection, and etc. Moreover, in real life, data are constantly created and stored as new block of tensors. In this setting, tensors need to be processed fast enough before the new tensor block is introduced.

My goal is to accurately decompose tensors and detect and track trend changes within them. For that end, I thought of autoencoders. The encoder part will compress the incoming tensor batch to latent vectors. The decoder part will be used to reconstruct the original tensor from several latent vectors (decomposition). I hypothesized that with careful tuning of the size, the latent vectors will contain

The objective of this experiment was to confirm if

Sample Video file

{% include video id="N-8QUdOdXls" provider="youtube" %}

Expected theme changes in the video

{% include figure image_path="/assets/images/TSNEdVectors.png" alt="Image not availalbe right now" caption="Latent vectors of AE projected to 2D space" %}
