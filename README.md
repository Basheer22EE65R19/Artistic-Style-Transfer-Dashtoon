# Artistic-Style-Transfer-Dashtoon

This repository contains code for neural style transfer using PyTorch.

## Overview

Neural style transfer is an optimization technique used to take two images — a content image and a style reference image — and blend them together in such a way that the output image looks like the content image, but "painted" in the style of the style reference image.

## Project Structure

The project is organized into three main parts:

1. **Training :**
   - The script takes command-line arguments for dataset path, style image, training parameters, and more.
   - It uses a custom implementation of the VGG16 model and the TransformerNet for style transfer.
   - Training involves optimizing the model's parameters using content and style losses.
   - Images are loaded from the specified dataset path, and style features are extracted from the style image.
   - The training loop saves checkpoints and sample images for evaluation at specified intervals.

2. **Style Image and Results Display :**
   - This Jupyter notebook displays the style image and the results of the style transfer.
   - It uses the matplotlib library to visualize the style image and the stylized output after training.

3. **Testing :**
   - This script performs style transfer on a user-specified image using a pre-trained model checkpoint.
   - The user can provide the path to the content image and the checkpoint model for stylization.
   - The stylized image is saved in the `images/outputs` directory.

## Install Dependencies:

- Ensure you have Python 3.x installed.
- Install the required Python packages:
  ```bash
  pip install -r requirements.txt

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/neural-style-transfer.git
   cd neural-style-transfer
   
2. Change the path with your dataset in Dashtoon.ipynb file and replace the style image datapath of your style.

### Libraries

- PyTorch
- torchvision
- Numpy
- Matplotlib

### Dataset: Art by AI - Neural Style Transfer

This dataset contains images created using neural style transfer techniques. [Explore the dataset](https://www.kaggle.com/datasets/vbookshelf/art-by-ai-neural-style-transfer) for more details.

### Training styled images
   ![Image 1](https://github.com/Basheer22EE65R19/Artistic-Style-Transfer-Dashtoon/blob/main/Images/Train_outputs/Cuphead/2000.jpg) | ![Image 2](https://github.com/Basheer22EE65R19/Artistic-Style-Transfer-Dashtoon/blob/main/Images/Train_outputs/Mosaic_outputs/2000.jpg) | ![Image 1](https://github.com/Basheer22EE65R19/Artistic-Style-Transfer-Dashtoon/blob/main/Images/Train_outputs/Starry_Night_outputs/2000.jpg)
   :-------------------------:|:-------------------------:|:-------------------------:
   Train Images for Cuphead style | Train Images for Mosaic style | Train images for Starry Night


### Three different styles

#### 1. Cuphead Style
   ![Alt Text](https://github.com/Basheer22EE65R19/Artistic-Style-Transfer-Dashtoon/blob/main/Images/Styles/cuphead.jpg)

#### 2. Mosaic Style
   ![Alt Text](https://github.com/Basheer22EE65R19/Artistic-Style-Transfer-Dashtoon/blob/main/Images/Styles/mosaic.jpg)

#### 3. Starry Night Style
   ![Alt Text](https://github.com/Basheer22EE65R19/Artistic-Style-Transfer-Dashtoon/blob/main/Images/Styles/starry_night.jpg)

### Test Input - Zurich

![Alt Text](https://github.com/Basheer22EE65R19/Artistic-Style-Transfer-Dashtoon/blob/main/Images/Test_image/zurich.jpeg)

### Test Outputs

#### 1. Cuphead Style - Zurich
   ![Alt Text](https://github.com/Basheer22EE65R19/Artistic-Style-Transfer-Dashtoon/blob/main/Images/Test_output/cuphead-zurich.jpeg)

#### 2. Mosaic Style - Zurich
   ![Alt Text](https://github.com/Basheer22EE65R19/Artistic-Style-Transfer-Dashtoon/blob/main/Images/Test_output/mosaic-zurich.jpeg)

#### 3. Stylized - Zurich
   ![Alt Text](https://github.com/Basheer22EE65R19/Artistic-Style-Transfer-Dashtoon/blob/main/Images/Test_output/stylized-zurich.jpeg)
