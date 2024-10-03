# Object Placement in Text-Conditioned Scenes


## Overview

Place an object's image in a text-conditioned scene using CompVis/stable-diffusion-v1-4 and generate an image through prompt them aligning other images over the generated scene/image.

## Features

- Text-Prompted Object Detection: Identify and segment objects based on natural language descriptions.
- Model Integration: Seamlessly combines CompVis/stable-diffusion-v1-4 for image generation.
- Output: Image masked from the white background and integrated with prompt-generated scene/image.
- GPU Support: Automatically utilizes GPU for faster inference if available.

## Setup

### Prerequisites

- Python 3.9 or higher
- CUDA (optional, for GPU acceleration)
- PyTorch compatible with your system and CUDA version

### Installation
 #### 1. Install Model dependencies:
```python
  pip install diffusers
```
#### 2. Install other required dependencies:
```python
  pip install numpy
  pip install torch 
  pip install cv2 
  pip install PIL 
  pip install argparse
```
## Usage
Here's how to use the script:

You can run the script directly using any Notebook IDE (Jupyterlabs/kaggle):

### Parameters:
```python
image_path = "Input image path"
text_prompt = "Your prompt"
output_path = "Output image path"
```
### Example
```python
image_path = "./example1.jpg"
text_prompt = "Product in a kitchen used in meal preparation"
output_path = "./generated.png"
```

## Output
### Example 1
![generated](https://github.com/user-attachments/assets/156cd0ef-801e-466f-a52d-f8c12c09ba0c)

### Example 2
![generated1](https://github.com/user-attachments/assets/070195b6-8cc6-4acf-bdbc-313732cc7b9f)


## Trouble Shooting
#### 1. CUDA Error: 
Ensure that CUDA is properly installed if you have a compatible GPU. If not, the script will automatically fall back to CPU.












