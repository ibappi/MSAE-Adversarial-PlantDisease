# Multi-Scale Convolutional Reconstruction Defense Against Adversarial and Real-World Corruptions in Plant Disease Recognition

This repository contains the implementation of a robust plant disease recognition framework that combines a Multi-Scale Autoencoder (MSAE) defense mechanism with a ConvNeXt V2 classifier to improve robustness against adversarial attacks and real-world image corruptions.

---

## Paper Information

**Title:** Multi-Scale Convolutional Reconstruction Defense Against Adversarial and Real-World Corruptions in Plant Disease Recognition

**Authors:** MD Ilias Bappi, Urusha Shakhakarmi, Jisoo Shin, Kyungbaek Kim

**Conference:** 2026 International Conference on Artificial Intelligence in Information and Communication (ICAIIC)

**Publisher:** IEEE

**Pages:** 1402–1407

**Publication Date:** 2026-02-24

---

## Overview

Deep learning models for plant disease recognition are highly vulnerable to adversarial perturbations and environmental image corruptions such as blur, noise, haze, compression artifacts, and lighting variations.

To address these limitations, this work introduces a robust defense framework that integrates:

- Multi-Scale Autoencoder (MSAE)
- ConvNeXt V2 classifier
- Adversarial defense mechanisms
- Real-world corruption robustness

The proposed MSAE reconstructs lesion structures at multiple spatial resolutions, helping preserve disease-related features under corrupted or adversarial conditions.

---

## Key Contributions

- Multi-scale reconstruction-based adversarial defense
- Robust plant disease recognition under image corruptions
- Integration of MSAE with ConvNeXt V2
- Improved resilience against FGSM, PGD, and natural corruptions
- Reconstruction-aware feature preservation

---

## Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/MSAE-Adversarial-PlantDisease.git
cd MSAE-Plant-Disease-Defense
```

Create virtual environment:

```bash
python -m venv venv
```

### Windows

```bash
venv\Scripts\activate
```
---

## Dataset Structure

```text
data/
└── PlantVillage/
    ├── Potato___Early_blight/
    ├── Potato___Late_blight/
    ├── Tomato___Leaf_Mold/
    ├── Tomato___Healthy/
    └── ...
```
---

## Adversarial Attacks

Supported attacks include:

- FGSM
- PGD
- AutoAttack

Attack implementations are available in:

```text
src/attacks.py
```

---

## Real-World Corruptions

Supported corruption scenarios include:

- Gaussian Noise
- Blur
- Haze
- JPEG Compression
- Brightness Variation
- Contrast Distortion

Corruption generation scripts are available in:

```text
src/corruptions.py
```

---

## Results

The proposed framework significantly improves robustness against both adversarial attacks and natural corruptions while preserving plant lesion structures.

| Method | Robust Accuracy |
|---|---|
| ConvNeXt V2 Baseline | Lower under attacks |
| MSAE + ConvNeXt V2 | Improved robustness |

---

## Methodology

The proposed framework consists of:

1. Multi-Scale Autoencoder reconstruction module
2. ConvNeXt V2 disease classifier
3. Adversarial perturbation defense pipeline
4. Corruption-aware feature reconstruction

The MSAE reconstructs lesion-specific structures at multiple resolutions, helping the classifier maintain reliable predictions under challenging environmental conditions.

---

## Citation

If you use this work, please cite:

```bibtex
@inproceedings{bappi2026msae,
  title={Multi-Scale Convolutional Reconstruction Defense Against Adversarial and Real-World Corruptions in Plant Disease Recognition},
  author={Bappi, MD Ilias and Shakhakarmi, Urusha and Shin, Jisoo and Kim, Kyungbaek},
  booktitle={2026 International Conference on Artificial Intelligence in Information and Communication (ICAIIC)},
  pages={1402--1407},
  year={2026},
  publisher={IEEE}
}
```

---

## Authors

- MD Ilias Bappi
- Urusha Shakhakarmi
- Jisoo Shin
- Kyungbaek Kim

---

## License

This repository is intended for academic and research purposes.
