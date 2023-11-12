# Neural Style Transfer with TensorFlow


# Overview
## This repository contains an implementation of Neural Style Transfer using TensorFlow. Neural Style Transfer is an artistic technique that allows the transfer of artistic styles from one image to another. This implementation utilizes a pre-trained VGG19 model to extract features from content and style images, and then optimizes a target image to minimize the content difference and style difference between the target image and the reference images.

# Requirements
Python 3.x
TensorFlow 2.x
NumPy
Matplotlib


# Getting Started
1. Clone the repository:
   git clone https://github.com/your-username/neural-style-transfer-tensorflow.git
cd neural-style-transfer-tensorflow
2. Install the required dependencies:
   pip install -r requirements.txt
3. Place your content and style images in the input folder.
4. Run the style transfer script:
   python style_transfer.py --content_image input/content.jpg --style_image input/style.jpg --output_image output/result.jpg


# Options
--content_image: Path to the content image.
--style_image: Path to the style image.
--output_image: Path to save the stylized output image.
--content_weight: Weight for the content loss (default: 1e3).
--style_weight: Weight for the style loss (default: 1e-2).
--total_variation_weight: Weight for the total variation loss (default: 30).
--num_iterations: Number of optimization iterations (default: 1000).
--optimizer: Optimization algorithm (default: 'adam', options: 'lbfgs' or 'adam').

# Acknowledgments
This implementation is based on the work by Gatys et al. in the paper "A Neural Algorithm of Artistic Style" (https://arxiv.org/abs/1508.06576).

# License
This project is licensed under the MIT License - see the LICENSE file for details.
