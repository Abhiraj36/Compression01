This repository contains code for a simple convolutional autoencoder implemented in PyTorch to compress and reconstruct RGB images.

Overview
The autoencoder compresses a 64×64 RGB image into a small latent vector (size 16).

The model is trained to reconstruct the image from this compressed representation.

Quantization is applied to both the latent vector and model weights to reduce storage size.

The project demonstrates basic lossy image compression with deep learning.

Results
Original image size: ~1237 KB

Compressed latent vector size: ~0.57 KB

Quantized model size: ~275 KB

Total compressed size: ~275.5 KB

Note: The reconstructed images are blurry due to the small latent dimension and model capacity.

Requirements
Python 3.x

PyTorch

torchvision

numpy

matplotlib

PIL (Pillow)

Usage
Place your input image as image.jpg in the repository folder.

Run the training script to train the autoencoder on the image.

After training, the model and quantized latent vectors will be saved.

Visualize original and reconstructed images with the provided plotting code.

License
