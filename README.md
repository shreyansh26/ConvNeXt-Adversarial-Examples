# Adversarial Example generation for ConvNeXt

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1c7EiO59cmVbxdCFZRDn82I-gBi6aTPDN?usp=sharing)

**This project is a Pytorch implementation of [@stanislavfort's project](https://twitter.com/stanislavfort/status/1481263565998805002?s=20).**

The notebook looks at generating adversarial images to "fool" the ConvNeXt model's image classification capabilities. [ConvNeXt](https://arxiv.org/abs/2201.03545) came out earlier this year from Meta AI.

The FGSM (Fast Gradient Sign Method) is a great algorithm to attack models in a *white-box* fashion with the goal of misclassification. Noise is added to the input image (not randomly) but in a manner such that the direction is the same as the gradient of the cost function with respect to the data.

Since this notebook is just the implementation - If you want to know more about FGSM, you may refer these - 

1. https://www.tensorflow.org/tutorials/generative/adversarial_fgsm
2. https://pytorch.org/tutorials/beginner/fgsm_tutorial.html
3. https://arxiv.org/abs/1412.6572

The following figure summarizes the goal of this notebook - 

<img src='https://i.imgur.com/C5YKxQ2.png'>

