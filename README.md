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


# Options
--content_image:  Path to the content image.

--style_image:  Path to the style image.
--output_image: Path to save the stylized output image.
--content_weight: Weight for the content loss (default: 1e3).
--style_weight: Weight for the style loss (default: 1e-2).
--total_variation_weight: Weight for the total variation loss (default: 30).
--num_iterations: Number of optimization iterations (default: 1000).
--optimizer: Optimization algorithm (default: 'adam', options: 'lbfgs' or 'adam').

## Acknowledgments
> This project is based on the work by Gatys et al. in the paper "A Neural Algorithm of Artistic Style" (https://arxiv.org/abs/1508.06576)

## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.
