# CSET419 – Introduction to Generative AI
## Lab 1: Synthetic Data Generation

### Objective
To generate synthetic data using a pre-trained generative AI model.

### Experiment
Implementation of a simple generative algorithm using Stable Diffusion to generate synthetic image data.

### Domain
Image Data Generation

### Model Used
Stable Diffusion (runwayml/stable-diffusion-v1-5)

### Input Prompts
- A futuristic smart city at night
- A peaceful village in the mountains
- A robot studying in a classroom
- A robot studying in a classroom
- A cyberpunk street with neon lights
- An astronaut walking on Mars

### Output
- 5 synthetic images generated
- Images stored as dataset
- Sample outputs displayed in notebook

### Tools
- Python
- Google Colab
- Hugging Face Diffusers
- PyTorch



---

## Lab 2: GAN-Based Image Generation

### Objective
To implement and train a basic Generative Adversarial Network (GAN) to generate synthetic images and evaluate the quality of generated samples.

### Experiment
A basic GAN model consisting of a Generator and a Discriminator was implemented using PyTorch.  
The Generator learns to produce synthetic images from random noise, while the Discriminator learns to distinguish real images from generated ones.

### Dataset
MNIST / Fashion-MNIST (loaded using Torchvision dataset utilities)

### Model Architecture
- **Generator**: Converts random noise vectors into 28×28 grayscale images.
- **Discriminator**: Classifies images as real or fake.

### Training Details
- Alternating training of Generator and Discriminator
- Binary Cross-Entropy loss used
- Adam optimizer
- Training performed for multiple epochs with periodic saving of generated samples

### Outputs
- Epoch-wise training logs (Generator and Discriminator loss)
- Generated image samples saved periodically in `generated_samples/`
- 100 final synthetic images saved in `final_generated_images/`
- Label prediction of generated images using a pre-trained ResNet18 classifier

### Tools & Technologies
- Python
- PyTorch
- Torchvision
- Google Colab (GPU)
