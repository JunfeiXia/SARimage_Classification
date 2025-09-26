# ViT-SAR-Classification

Code repository for the paper:

**Xia, J., Romeiser, R., Zhang, W., & Özgökmen, T. (2025). Use of Vision Transformer to Classify Sea Surface Phenomena in SAR Imagery. *IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing*.**
DOI: [10.1109/JSTARS.2025.3558673](https://doi.org/10.1109/JSTARS.2025.3558673)

---

## 📖 Overview

This repository contains the implementation of a **Vision Transformer (ViT)** framework for classifying sea surface phenomena in **Synthetic Aperture Radar (SAR)** imagery.

The code demonstrates:

* Preprocessing and training using the **TenGeoP-SARwv** dataset.
* Reproduction of selected figures and results shown in the manuscript.
* Example training configurations for ViT models (e.g., `vitl32_384`).

---

## 📂 Repository Structure

```
.
├── LICENSE
├── Manuscript Figure.ipynb        # Notebook to reproduce figures/results
├── README.md
├── requirements.txt               # Python dependencies
├── training_vitl32_384_balanced.ipynb    # Main training workflow (ViT-L/32, 384 input)
├── other tests/                   # Additional experiments / configs
```

---

## 📊 Dataset

The study uses the **TenGeoP-SARwv** dataset:

* DOI: [10.17882/56796](https://doi.org/10.17882/56796)
* Description: Global collection of Sentinel-1 SAR wave mode images annotated for ocean surface phenomena.
* Access: Download from SEANOE.

After downloading, adjust paths in the notebooks (`training_vitl32_384_balanced.ipynb`) to point to your local dataset folder.

---

## ⚙️ Requirements

* Python 3.9+
* Install dependencies:

  ```bash
  pip install -r requirements.txt
  ```

Key libraries include:

* PyTorch / torchvision
* numpy, pandas, matplotlib, scikit-learn...

---

## 🚀 Usage

### 1. Training

Open and run:

```bash
jupyter notebook training_vitl32_384_balanced.ipynb
```

This notebook:

* Loads TenGeoP-SARwv dataset.
* Trains a Vision Transformer (ViT-L/32, 384x384 input).
* Saves checkpoints and logs.

### 2. Reproducing Manuscript Figures

Run:

```bash
jupyter notebook "Manuscript Figure.ipynb"
```

This notebook:

* Visualizes classification results.
* Generates plots similar to those in the paper.
* Summarizes key metrics.

### 3. Other tests

The `other tests/` folder contains experimental variations (different model sizes, augmentations, and preprocessing schemes).

---

## 📈 Results

* Classification performance and selected visualizations are included in the notebooks.
* Figures in the manuscript (confusion matrices, attention maps, accuracy plots) can be regenerated from the provided code.

---

## 📌 Citation

If you use this code, please cite:

```
Xia, J., Romeiser, R., Zhang, W., & Özgökmen, T. (2025).
Use of Vision Transformer to Classify Sea Surface Phenomena in SAR Imagery.
IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing.
doi: 10.1109/JSTARS.2025.3558673
```

Dataset citation:

```
Wang et al. (2017). TenGeoP-SARwv. SEANOE. doi:10.17882/56796
```

---

## 📬 Contact

**Junfei Xia**
Email: [junfei.xia@outlook.com](mailto:junfei.xia@outlook.com) • Web: [www.junfeixia.com](http://www.junfeixia.com)

