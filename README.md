# Handwritten Digit Generation using GAN

This project builds a Generative Adversarial Network to generate handwritten digits similar to the MNIST dataset.

The model learns by training two neural networks against each other. One creates fake images, while the other tries to detect them. Over time, the generator improves and starts producing more realistic digits.

## Project Overview

The goal of this project is to understand how GANs work in practice by training a model to generate images from random noise.

The dataset used is MNIST, which contains grayscale images of handwritten digits from 0 to 9.

## How it Works

The model has two parts:

Generator

* Takes random noise as input
* Produces fake digit images
* Learns to make images that look real

Discriminator

* Takes an image as input
* Predicts whether the image is real or fake
* Helps the generator improve by giving feedback

Both models are trained together. The generator tries to fool the discriminator, while the discriminator tries to get better at spotting fake images.

## Results

At the beginning, the generated images look like random noise.

After training for several epochs:

* Shapes of digits start to appear
* Images become clearer
* Some digits are easy to recognize

The final outputs show that the model can generate digit-like images, although some are still imperfect.

## Challenges

Training a GAN is not straightforward. Some issues faced during this project:
* Training can be unstable
* Loss values do not always decrease smoothly
* The generator and discriminator must stay balanced
* Results improve slowly and need multiple epochs

## Requirements
* Python
* TensorFlow or PyTorch
* NumPy
* Matplotlib

## How to Run
* Clone the repository
* Open the notebook file
* Run all cells step by step
* Observe training and generated outputs

## File Structure
* Handwritten-Digit-Generation-Using-GAN.ipynb – Main notebook with model and training
* Report: Handwritten Digit Generation Using GAN - Project Report
* README.md – Project description

## Conclusion

This project shows how a simple GAN can learn to generate handwritten digits from noise. While the results are not perfect, the model is able to capture the basic structure of digits.

It also highlights that GANs are powerful but require careful training and tuning.
