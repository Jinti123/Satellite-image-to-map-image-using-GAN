#  Satellite-to-Map using GAN

This repository contains the implementation of a deep learning model that translates **satellite images** into **map images** using a **Conditional Generative Adversarial Network (cGAN)**.  
We use a **U-Net** based generator and a **PatchGAN** discriminator, inspired by the **pix2pix** framework.

---

##  Overview

Generating map-like representations from satellite imagery is useful in various applications such as:

- Urban planning
- Navigation
- Disaster response

In this work, we train a **conditional GAN** that learns a mapping from satellite images to corresponding map images using paired datasets.

---

## 🧠 Model Architecture

###  Generator - U-Net
- Encoder-decoder structure with skip connections.
- Preserves spatial details and context from input satellite images.

###  Discriminator - PatchGAN
- Operates on **70×70** image patches.
- Outputs a matrix indicating real/fake per patch.
- Encourages high-frequency detail in the generated maps.

---

## 📂 Dataset

We use the **Maps dataset** provided by the authors of the pix2pix paper, which contains paired satellite and map images.

📥 **Download Links:**
- **Maps Dataset:** [maps.tar.gz](http://efrosgans.eecs.berkeley.edu/pix2pix/datasets/maps.tar.gz)
- **More Datasets:** [pix2pix datasets](http://efrosgans.eecs.berkeley.edu/pix2pix/datasets/)

## Research Paper Implemented in this project : 
**Original pix2pix paper: https://arxiv.org/pdf/1611.07004.pdf**

**Github for the original paper:** https://phillipi.github.io/pix2pix/


