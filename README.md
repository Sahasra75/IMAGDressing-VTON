# IMAGDressing: Hybrid Diffusion-Based Virtual Try-On Framework

## Overview

IMAGDressing is a hybrid diffusion-based virtual try-on (VTON) framework designed to generate realistic garment transfer results while preserving human pose, garment structure, and facial identity. The proposed approach integrates structural conditioning with diffusion-based synthesis to improve visual consistency, garment alignment, and perceptual fidelity.

This repository provides the official implementation, experimental setup, and evaluation pipeline associated with our manuscript submitted to *The Visual Computer*.

---

## 🔗 Resources

* **GitHub Repository:** https://github.com/Sahasra75/IMAGDressing-VTON
* **DOI:** *(To be added after Zenodo release)*

---

## ✨ Key Features

* Hybrid diffusion-based virtual try-on framework
* Pose-guided and garment-conditioned image generation
* Enhanced garment alignment and texture preservation
* Improved identity consistency across synthesized outputs
* Modular and extensible architecture for research use

---

## 📂 Dataset

This project utilizes publicly available benchmark datasets for virtual try-on:

### 1. VITON Dataset

* Official Project Page: http://www.yumingjiang.com/research/virtual_tryon/
* Paper: *Toward Characteristic-Preserving Image-based Virtual Try-On Network*
* Description:

  * Paired images of models and in-shop garments
  * Includes pose annotations and segmentation maps
  * Widely used benchmark dataset for virtual try-on research

---

### 2. VITON-HD Dataset

* Official Project Page: https://psh01087.github.io/VITON-HD/
* Paper: *VITON-HD: High-Resolution Virtual Try-On via Misalignment-Aware Normalization*
* Description:

  * High-resolution extension of VITON (1024×768)
  * Provides fine-grained garment details and textures
  * Suitable for evaluating advanced generative models

---

> ⚠️ Note: Access to datasets may require agreement to usage terms or permission from the respective authors. Please follow the instructions provided on the official project pages.

---

## ⚙️ Installation

```bash
git clone https://github.com/Sahasra75/IMAGDressing-VTON.git
cd IMAGDressing-VTON
pip install -r requirements.txt
```

---

## 🚀 Usage

### Run Inference

```bash
python test.py
```

### Train Model

```bash
python train.py
```

---

## 📊 Evaluation

The model is evaluated using standard image synthesis metrics:

* Structural Similarity Index (SSIM)
* Peak Signal-to-Noise Ratio (PSNR)
* Fréchet Inception Distance (FID)
* Learned Perceptual Image Patch Similarity (LPIPS)

These metrics assess structural fidelity, perceptual realism, and reconstruction quality.

---

## 📈 Results

IMAGDressing demonstrates improvements in:

* Garment alignment accuracy
* Texture preservation
* Identity consistency

compared to existing virtual try-on approaches.

---

## 📌 Citation

If you find this work useful, please cite:

```
@article{IMAGDressing2026,
  title={IMAGDressing: Hybrid Diffusion-Based Virtual Try-On Framework},
  author={Veerababu Reddy},
  journal={The Visual Computer},
  year={2026},
  doi={To be added}
}
```

---

## 📄 License

This project is intended for academic and research purposes only.

---

## 🙌 Acknowledgements

This work builds upon prior research in virtual try-on systems, diffusion models, and garment modeling techniques.

---

 

> 🔔 This repository is directly associated with a manuscript submitted to *The Visual Computer*. If you use this code, please cite the corresponding paper.
