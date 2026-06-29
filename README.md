# Medical-Image-Synthesis-GANs
A comprehensive deep learning framework for medical image synthesis using Conditional DCGAN, Progressive WGAN-GP, and StyleGAN2-ADA for medical image augmentation and class imbalance reduction.
# Medical Image Synthesis using GANs

A comprehensive deep learning framework for generating realistic synthetic medical images using multiple Generative Adversarial Network (GAN) architectures. This repository implements and compares Conditional DCGAN, Progressive WGAN-GP with Self-Attention, and StyleGAN2-ADA for medical image augmentation.

---

## Project Overview

Medical imaging datasets often suffer from class imbalance and limited data availability, reducing the performance of deep learning models. This project addresses these challenges by generating realistic synthetic medical images using advanced GAN architectures.

The repository contains multiple generative models designed for chest X-ray image synthesis and can be extended to other medical imaging modalities.

---

## Implemented Models

### 1. Conditional DCGAN

- Class-conditioned image generation
- Generator and discriminator with label embedding
- Domain-specific augmentation
- TBX11K dataset support

---

### 2. Progressive WGAN-GP

- Progressive Growing GAN
- Wasserstein Loss with Gradient Penalty
- Self-Attention Module
- Conditional image generation
- Stage-wise resolution training
- Warm-start using Stage-1 generator

Training Progression:

```
8×8
 ↓
16×16
 ↓
32×32
 ↓
64×64
 ↓
128×128
```

---

### 3. StyleGAN2-ADA

This repository also includes:

- StyleGAN2-ADA training
- Automatic resume training
- Google Drive checkpoint management
- FID evaluation
- High-resolution image generation
- Snapshot-based image synthesis

---

## Repository Structure

```
Medical-Image-Synthesis-GANs/

│
├── project.py                  # Conditional DCGAN + Progressive WGAN-GP
├── style_gan.py                # StyleGAN2-ADA implementation
│
├── outputs/
├── checkpoints/
├── generated_images/
├── evaluation/
├── datasets/
│
├── README.md
└── requirements.txt
```

---

## Datasets

### TBX11K

Chest X-ray dataset

Classes

- Healthy
- Tuberculosis
- Sick

---

### Messidor2

Fundus image dataset for diabetic retinopathy grading.

The framework is designed to support both datasets with minimal modifications.

---

## Features

- Conditional GAN Training
- Progressive GAN Training
- StyleGAN2-ADA Integration
- Self-Attention
- Gradient Penalty
- Domain Augmentation
- Automatic Checkpoint Saving
- Resume Training
- FID Evaluation
- High-Resolution Image Generation
- Google Colab Compatible

---

## Evaluation

Generated images are evaluated using

- Frechet Inception Distance (FID)
- Inception Score (optional)

---

## Technologies Used

- Python
- PyTorch
- TorchVision
- NumPy
- Pandas
- Matplotlib
- PIL
- KaggleHub
- StyleGAN2-ADA
- Google Colab

---

## Installation

Clone the repository

```bash
git clone https://github.com/yourusername/Medical-Image-Synthesis-GANs.git

cd Medical-Image-Synthesis-GANs
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## Training

### Stage 1

Train Conditional DCGAN

```bash
python project.py
```

### Stage 2

Train Progressive WGAN-GP

```bash
python project.py
```

### StyleGAN2-ADA

Train or Resume

```bash
python style_gan.py
```

---

## Applications

- Medical Image Augmentation
- Synthetic Chest X-ray Generation
- Tuberculosis Research
- Diabetic Retinopathy Research
- Dataset Balancing
- Medical AI Research

---

## Future Improvements

- StyleGAN3
- Diffusion Models
- Multi-modal Medical Image Generation
- Explainable AI Integration
- Federated Learning
- Synthetic Data Benchmarking

---

## License

MIT License

---

## Zamin Hamid

**Your Name**

Deep Learning • Medical Image Analysis • Computer Vision
