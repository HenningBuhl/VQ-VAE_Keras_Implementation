# VQ-VAE Keras Implementation

## Keras implementaion of VQ-VAE (Vector Quantizer Variational AutoEncoder)

Sources:

* https://arxiv.org/abs/1711.00937
* https://github.com/deepmind/sonnet/blob/master/sonnet/python/modules/nets/vqvae.py
* https://github.com/deepmind/sonnet/blob/master/sonnet/examples/vqvae_example.ipynb

Example Notebook: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/HenningBuhl/VQ-VAE_Keras_Implementation/blob/master/VQ_VAE_Keras_MNIST_Example.ipynb)

## Original vs Reconstructed

![alt text](https://raw.githubusercontent.com/HenningBuhl/VQ-VAE_Keras_Implementation/master/recon_example.png)

## Notes on compatibility

* The notebook was created on a Google Colab machine (GPU accelerated) which ran TensorFlow version 1.x

* The notebook was tested with TensorFlow version 2.2.0 and Keras version 2.3.1 on a Google Colab machine (GPU accelerated) and worked when removing the parameter validate_indices from the call tf.nn.embedding_lookup (it is a deprecated argument).

* If you have issues with eager execution with TensorFlow version 2.x or higher, issue #2 might help you.
