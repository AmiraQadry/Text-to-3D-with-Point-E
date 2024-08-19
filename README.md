# 3D Image Generation using Point-E (ViT + GPT-2) 

This project showcases the use of OpenAI's Point-E model to generate 3D images from text prompts. By leveraging a combination of Vision Transformers (ViT) and GPT-2, 
Point-E can synthesize view-based images from text and convert them into detailed 3D point clouds. 
This project demonstrates the entire process, from setting up the environment to generating various 3D objects based on text descriptions.

## Table of Contents
- [Introduction](#introduction)
- [How Point-E Works](#how-point-e-works)
- [Project Setup](#project-setup)
- [Examples](#examples)
- [References](#references)
- [Contributing](#contributing)

## Introduction
This notebook demonstrates the use of OpenAI's Point-E model to generate 3D images from text prompts. The Point-E model combines a text-to-image model with an image-to-3D model, 
leveraging large datasets of (text, image) and (image, 3D) pairs, respectively.

### Key Highlights:
- Introduction to the Point-E model.
- Inference examples showcasing text-to-3D object generation.
- The libraries used include Point-E and PyTorch.

## How Point-E Works
The Point-E model generates 3D objects from text prompts by following these steps:

1. **Synthetic View Generation**: Creates an image based on the text caption.
2. **Coarse Point Cloud Production**: Generates a low-resolution (1,024 points) point cloud based on the synthetic view.
3. **Fine Point Cloud Production**: Refines the point cloud to a higher resolution (4,096 points) using the initial point cloud and the synthetic view.

The model assumes that the synthetic view sufficiently represents the information from the text caption.

## Project Setup
### Prerequisites
- Python 
- Git
- PyTorch
- Point-E

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/openai/point-e
   cd point-e
   ```
2. Install the dependencies:
   ```bash
   pip install -e .
   ```

### Running the Notebook
To run the notebook, follow these steps:
1. Import necessary libraries.
2. Set up the model and configure the sampler.
3. Use provided examples to generate 3D point clouds from text prompts.

## Examples
Here are some examples of 3D objects generated from text prompts:

1. **A Red Motorcycle**
2. **A Red Santa Hat**
3. **Purple Headphones**
4. **A Realistic 3D Rendering of a Corgi**
5. **A Blue Mug**
6. **A Robot**
7. **An Elaborate Fountain**
8. **An Orange and White Traffic Cone**
9. **A 3D Printable Gear**

Each example includes a text prompt and a corresponding 3D point cloud visualization.

## References
- [OpenAI's Point-E Paper](https://arxiv.org/abs/2212.08751)
- [Point-E GitHub Repository](https://github.com/openai/point-e)
- [YouTube Video on Point-E](https://www.youtube.com/watch?v=Q7kF7TUXgoA)
- [Text to Point Cloud Example](https://huggingface.co/Point-E)

## Contributing
If you have any suggestions or feedback, feel free to open an issue or submit a pull request. Contributions are welcome!

---

Thank you for checking out this project! 😊
