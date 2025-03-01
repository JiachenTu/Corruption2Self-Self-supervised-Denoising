# Corruption2Self: Score-based Self-supervised MRI Denoising

<div align="center">
  <a href="https://jiachentu.github.io/Corruption2Self-Self-Supervised-Denoising/">
    <img src="https://img.shields.io/badge/🌐_Project_Website-Visit_Now-blue?style=for-the-badge" alt="Project Website" height="35">
  </a>
</div>

<div align="center">
  <a href="https://openreview.net/forum?id=uNd289HjLi">
    <img src="https://img.shields.io/badge/ICLR-2025-b31b1b?style=flat-square" alt="Conference">
  </a>
  <a href="https://github.com/JiachenTu/Corruption2Self-Self-Supervised-Denoising/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square" alt="License: MIT">
  </a>
</div>

<br>

This repository contains the official PyTorch implementation of our paper:

> **Score-based Self-supervised MRI Denoising**  
> Jiachen Tu, Yaokun Shi, Fan Lam  
> *ICLR 2025*  
> [Paper](https://openreview.net/forum?id=uNd289HjLi) | [Website](https://jiachentu.github.io/Corruption2Self-Self-Supervised-Denoising/)

## Abstract

Magnetic resonance imaging (MRI) is a powerful noninvasive diagnostic imaging tool that provides unparalleled soft tissue contrast and anatomical detail. Noise contamination, especially in accelerated and/or low-field acquisitions, can significantly degrade image quality and diagnostic accuracy. Supervised learning-based denoising approaches have achieved impressive performance but require high signal-to-noise ratio (SNR) labels, which are often unavailable. Self-supervised learning holds promise to address the label scarcity issue, but existing self-supervised denoising methods tend to oversmooth fine spatial features and often yield inferior performance than supervised methods.

We introduce Corruption2Self (C2S), a novel score-based self-supervised framework for MRI denoising. At the core of C2S is a generalized denoising score matching (GDSM) loss, which extends denoising score matching to work directly with noisy observations by modeling the conditional expectation of higher-SNR images given further corrupted observations. This allows the model to effectively learn denoising across multiple noise levels directly from noisy data. Additionally, we incorporate a reparameterization of noise levels to stabilize training and enhance convergence, and introduce a detail refinement extension to balance noise reduction with the preservation of fine spatial features. Moreover, C2S can be extended to multi-contrast denoising by leveraging complementary information across different MRI contrasts.

We demonstrate that our method achieves state-of-the-art performance among self-supervised methods and competitive results compared to supervised counterparts across varying noise conditions and MRI contrasts on the M4Raw and fastMRI datasets.

## Code Release

⏳ **The code will be released soon. Please stay tuned!**

Upon release, this repository will include:
- 🔧 Implementation of the Corruption2Self (C2S) framework
- 📊 Training and evaluation scripts
- 📚 Pre-trained models for various MRI contrasts
- 📝 Documentation and usage examples

## Citation

If you find our work useful for your research, please consider citing:

```bibtex
@inproceedings{
tu2025scorebased,
title={Score-based Self-supervised {MRI} Denoising},
author={Jiachen Tu and Yaokun Shi and Fan Lam},
booktitle={The Thirteenth International Conference on Learning Representations},
year={2025},
url={https://openreview.net/forum?id=uNd289HjLi}
}
