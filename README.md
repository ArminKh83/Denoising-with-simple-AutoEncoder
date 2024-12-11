# Denoising-with-simple-AutoEncoder

# Autoencoder for Denoising MNIST Images

This project implements a convolutional autoencoder in PyTorch to denoise images from the MNIST dataset. The model learns to remove Gaussian noise added to the images during training and then reconstructs the clean versions.

## Model Architecture
The autoencoder consists of:
- **Encoder**: A series of convolutional layers that downsample the input images.
- **Decoder**: A series of transposed convolutional layers that upsample the encoded features to reconstruct the image.

## Training
The model is trained using noisy MNIST images as input, with the original clean images as targets. The binary cross-entropy loss function is used to minimize the difference between the noisy input and the denoised output.

## Evaluation
After training, the model is evaluated on a set of test images. The original, noisy, and denoised images are visualized in a side-by-side plot for comparison.
