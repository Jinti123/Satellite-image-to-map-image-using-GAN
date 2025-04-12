# Satellite-to-map-using-GAN
This repository contains the implementation of a deep learning model that translates **satellite images** into **map images** using a **Conditional Generative Adversarial Network (cGAN)**. We use a **U-Net** based generator and a **PatchGAN discriminator**, inspired by the **pix2pix** framework.
# Overview
Generating map-like representations from satellite imagery is useful in various applications such as urban planning, navigation, and disaster response. In this work, we train a conditional GAN that learns a mapping from satellite images to corresponding map images using paired datasets.
# Model Architecture
**Generator - U-Net**
1. Encoder-decoder structure with skip connections.

Preserves spatial info from input satellite images.

**Discriminator - PatchGAN**
Operates on 70×70 image patches.

Outputs a matrix indicating real/fake per patch — better for textures and fine details.
#Dataset
We use the **Maps dataset** provided by the authors of pix2pix, which contains paired satellite and map images.

**Download: ** 
**Maps Dataset:** http://efrosgans.eecs.berkeley.edu/pix2pix/datasets/maps.tar.gz
More datasets can be found here:  
**pix2pix datasets:** http://efrosgans.eecs.berkeley.edu/pix2pix/datasets/

#Research Paper Implemented in this Project : 
**Original pix2pix paper:** https://arxiv.org/pdf/1611.07004.pdf
**Github for the original paper:** https://phillipi.github.io/pix2pix/



