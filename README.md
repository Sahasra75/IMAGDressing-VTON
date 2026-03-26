# IMAGDressing: A Hybrid Diffusion Framework for Realistic Virtual Garment Try-On

IMAGDressing is an implementation-oriented virtual try-on framework built upon diffusion-based generative models. The system focuses on improving garment alignment, visual consistency, and identity preservation through structured multimodal conditioning within a pretrained latent diffusion pipeline.

This repository accompanies the research article:

**“Hybrid Diffusion Framework for Realistic Virtual Garment Try-On”**

---

## 🌟 Overview

Image-based virtual try-on (VTON) aims to generate realistic images of a person wearing a target garment. While recent diffusion-based approaches have shown promising results, challenges remain in maintaining structural alignment, texture fidelity, and identity consistency.

IMAGDressing explores these challenges through a structured implementation that integrates garment features, pose guidance, and identity-aware conditioning into a unified diffusion pipeline.

---

## 🌟 Contributions

- Implementation of a diffusion-based virtual try-on pipeline integrating garment, pose, and identity-aware conditioning  
- Exploration of hybrid conditioning strategies for improving synthesis consistency  
- Evaluation on standard benchmarks (VITON, VITON-HD)  
- Public release of code and experimental setup for reproducibility  

## 🧠 Method Overview

The framework operates within a pretrained latent diffusion model and integrates multiple conditioning inputs.

### Inputs:

* Person image (Ip)
* Garment image (Ig)
* Pose representation (P)
* Optional text conditioning

### Pipeline Components:

* Garment feature extraction
* Pose estimation and human parsing
* Identity-aware conditioning
* Diffusion-based image synthesis

These components are fused through attention mechanisms to generate realistic try-on outputs while maintaining structural and visual consistency.

---

## 📁 Repository Structure

```text
├── src/                  # Core diffusion pipeline
├── preprocess/           # Pose estimation & human parsing
├── gradio_demo/          # Interactive demo interface
├── ckpt/                 # Pretrained weights
├── configs/              # Configuration files
├── inference.py          # Inference script
├── train.py              # Training (if applicable)
├── results/              # Sample outputs
└── README.md
```

---

## 🛠️ Installation

**Requirements:**

* Python 3.10+
* PyTorch 2.0+
* CUDA 11.8+

```bash
git clone https://github.com/Sahasra75/IMAGDressing-VTON
cd IMAGDressing-VTON

conda env create -f environment.yaml
conda activate imagdressing
```

---

## 🚀 Usage

### Run Demo

```bash
python gradio_demo/app.py
```

### Inference

```bash
python inference.py \
    --person_image path/to/person.jpg \
    --garment_image path/to/garment.jpg \
    --output_dir results/
```

---

## 📊 Datasets

The framework is evaluated on:

* **VITON Dataset**
  http://www.yumingjiang.com/research/virtual_tryon/

* **VITON-HD Dataset**
  https://psh01087.github.io/VITON-HD/

---

## 📈 Results

The model generates visually consistent try-on outputs with improved garment alignment and reduced artifacts.

Quantitative evaluation results are reported in the paper. Representative qualitative outputs are provided in the repository.

---

## 🔗 Reproducibility

* **GitHub Repository:**
  https://github.com/Sahasra75/IMAGDressing-VTON

* **Zenodo DOI:**
  https://doi.org/10.5281/zenodo.19232693

This ensures long-term accessibility and reproducibility of the work.

---

## ⚠️ Limitations

* Performance may vary under extreme poses or occlusions
* Fine-grained texture preservation can be challenging
* Identity consistency may degrade in complex scenarios

---

## 📄 Citation

```bibtex
@article{imagdressing2026,
  title={Hybrid Diffusion Framework for Realistic Virtual Garment Try-On},
  author={Reddy, Veerababu and others},
  journal={The Visual Computer},
  year={2026}
}
```

---

## 📬 Contact

(Your email here)
