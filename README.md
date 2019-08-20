# DCGAN-CIFAR10-pytorch
A DCGAN built on the CIFAR10 dataset using pytorch

DCGAN is one of the popular and successful network designs for GAN. It mainly composes
of convolution layers without max pooling or fully connected layers. It uses convolutional
stride and transposed convolution for the downsampling and the upsampling. Architecture
guidelines for stable Deep Convolutional GANs as mentioned by Soumith Chintala

These are the guidelines for constructing a DCGAN as mentioned by Soumith Chintala (https://arxiv.org/abs/1511.06434)

Replace any pooling layers with strided convolutions(discriminator) and fractional-
strided convolutions (generator).

Use batchnorm in both the generator and the discriminator.

Remove fully connected hidden layers for deeper architectures.

Use ReLU activation in generator for all layers except for the output, which uses Tanh.

Use LeakyReLU activation in the discriminator for all layers.

The simplicity of DCGAN contributes to its success. We reach certain bottleneck that
increasing the complexity of the generator does not necessarily improve the image quality.
Until we identify the bottleneck and know how to train GANs more effective, DCGAN
remains a good start point for a new project.
I created a DCGAN model for mimicking the data distribution of CIFAR-10 dataset
