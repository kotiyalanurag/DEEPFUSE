# :art: DEEPFUSE

Using neural networks to create artistic portraits given a pair of content and style image.

## Overview

We are using certain layers of a pre-trained VGG-19 for feature extraction from our style image. Using these features we try to recreate our content
image. Our end goal is to reduce the loss between generated image and our content image as much as possible.

Style Layers
```html
style_layer_names = [
    "block1_conv1",
    "block2_conv1",
    "block3_conv1",
    "block4_conv1",
    "block5_conv1",
]
```
Content Layers
```html
content_layer_name = "block5_conv2"
```
## Hyperparameters

```html
VAR_WGT = 1e-6
STYLE_WGT = 1e-6
CONTENT_WGT = 2.5e-8
STEPS = 2000
```
## Output


## How to get started?

Open the terminal on your mac and type 
```html
mkdir deep\ fuse
```
Then switch to the new directory using
```html
cd deep\ fuse
```
Now clone the repository on your local machine using
```html
git clone https://github.com/kotiyalanurag/DEEPFUSE.git
```
Now create a virtual environment using assuming you have python installed on your machine
```html
python -m venv env
```
Switch on your new environment using
```html
source env/bin/activate
```
Now install the requirements for this project using
```html
pip install -r requirements.txt
```
Have fun playing around with the notebook.
