# Pix2Pix on Cityscapes Dataset

This project implements the **Pix2Pix** conditional Generative Adversarial Network (cGAN) for **image-to-image translation**, using the **Cityscapes** dataset.  
The model learns to translate **semantic segmentation maps** into realistic **urban street scenes**, demonstrating the effectiveness of supervised image generation.

---

## 📘 Overview

Pix2Pix, introduced by *Isola et al. (CVPR 2017)*, is a **conditional GAN** framework that learns a mapping from an input image to an output image using a paired dataset.  
In this implementation:
- The **generator** is a **U-Net** that transforms semantic label maps into realistic RGB images.  
- The **discriminator** is a **PatchGAN**, which judges image realism at the patch level.

---

## ⚙️ Setup

It is recommended to run this notebook on **Kaggle** or **Google Colab** with GPU enabled.

```bash
# Install dependencies
!pip install torch torchvision matplotlib numpy tqdm pillow
