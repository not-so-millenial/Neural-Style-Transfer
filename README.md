# Neural Style Transfer with Pytorch

## Overview
This repository contains an implementation of Neural Style Transfer using TensorFlow. Neural Style Transfer is an artistic technique that allows the transfer of artistic styles from one image to another. This implementation utilizes a pre-trained VGG19 model to extract features from content and style images, and then optimizes a target image to minimize the content difference and style difference between the target image and the reference images.

## Requirements
Python 3.x 

Pytorch 

NumPy

Matplotlib


## Getting Started
1. Clone the repository:
   git clone https://github.com/your-username/neural-style-transfer-tensorflow.git
   cd neural-style-transfer-tensorflow
2. Install the required dependencies:
   pip install -r requirements.txt
3. Place your content and style images along with code in the folder.

## Model Architecture and Scope
- A **VGG19 model is used for NST** in the following respository, though **Resnet50** & a perpetual loss concept using an Image Transformer neural network which increases the speed of NST and it allows to train the **Image transformer** neural network per content and apply various styles without retraining.

- Two major loss functions defined in the architecture includes **content loss** and **style loss**; content loss will make content we want in the generated image captured efficiently. It has been observed that **CNN captures information about the content in the higher levels of the network**, whereas the lower levels are more focused on the individual pixel values.

- **Style Loss**; major content is **Gram Matrix** which is a representation of style in NST & captures correlations between features in layer, quantifying texture & patterns. As loss function for style has more work than content as multiple layers are involved in computing, Gram matrix helps in capturing essential information.


# Hyperparameter Options

-content_image:  Path to the content image (here used , IITR).

-style_image:  Path to the style image (here used, abstract).

-default size: Current size of 300x300 is used for faster training.

-content_weight: Weight for the content loss (default: 1).

-style_weight: Weight for the style loss (default: 1000000).

-num_iterations: Number of optimization iterations (default: 300).

-optimizer: Optimization algorithm (default: 'lbfgs', options: 'lbfgs' or 'adam').

-activation: Activation function (default: 'ReLU', options: 'Leaky ReLU' or 'ELUs' )

## Acknowledgments
> This project is based on the work by Gatys et al. in the paper "A Neural Algorithm of Artistic Style" (https://arxiv.org/abs/1508.06576)

## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.
