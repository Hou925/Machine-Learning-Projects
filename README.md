# Machine-Learning-Projects

A collection of end-to-end machine learning projects covering classification, regression, clustering, sequence labeling, and audio recognition — each implemented with multiple models for direct comparison.

> 中文版说明请见 [README_CN.md](./README_CN.md)

---

## Projects

### 1. 🖼️ FashionMNIST Classification
**Directory:** `Classification_FashionMNIST/`

Classifies the 10 clothing categories in FashionMNIST using three different approaches, enabling a clear apples-to-apples model comparison:
- **Random Forest** (`FashionMNIST_classification_Forest_Model.ipynb`)
- **Neural Network** (`FashionMNIST_classification_NN_Model.ipynb`)
- **Support Vector Machine** (`FashionMNIST_classification_SVM_Model.ipynb`)

---

### 2. 🔵 FashionMNIST Clustering
**Directory:** `Clustering_FashionMNIST/`

Explores unsupervised grouping of FashionMNIST images with three distinct strategies:
- **Autoencoder** – learns a compressed latent representation before clustering (`FashionMNIST_clustering_Autoencoder_Model.ipynb`)
- **DBSCAN** – density-based clustering, no need to specify cluster count (`FashionMNIST_clustering_DBSCAN_Model.ipynb`)
- **K-Means** – classic centroid-based clustering (`FashionMNIST_clustering_Kmeans_Model.ipynb`)

---

### 3. 🏠 California Housing Regression
**Directory:** `Regression_California_Housing/`

Predicts California housing prices using two model families, highlighting trade-offs between interpretability and raw performance:
- **Random Forest** (`California_Housing_Regression_Forest_Model.ipynb`)
- **Neural Network** (`California_Housing_Regression_NN_Model.ipynb`)

---

### 4. 🀄 CRF Chinese Word Segmentation
**Directory:** `CRF_Chinese_Segmentation_Model/`

Builds a **Conditional Random Field (CRF)** sequence labeling model for Chinese word segmentation:
- Corpus pre-processing pipeline using the **People's Daily** dataset (`corpus_process.ipynb`)
- BMES tagging scheme for character-level segmentation
- Full training and evaluation workflow (`crf_model.ipynb`)

---

### 5. 🎵 Simple Audio Classifier
**Directory:** `simple-audio-model based on google-teachable-machine/`

A lightweight audio recognition model trained entirely in-browser via **Google Teachable Machine**:
- Classes: background noise, clapping, table-knocking, metal collision
- Exported as a ready-to-use TensorFlow.js model (`model.json` + `weights.bin`)
- Zero-code training pipeline — great for rapid prototyping

---

## Tech Stack

| Area | Tools / Libraries |
|------|------------------|
| Deep Learning | TensorFlow / Keras |
| Classical ML | scikit-learn |
| Sequence Labeling | sklearn-crfsuite |
| Data Processing | NumPy, Pandas |
| Visualization | Matplotlib |
| Audio (no-code) | Google Teachable Machine |

---

## Getting Started

Each sub-project is self-contained as a Jupyter Notebook. Clone the repo and open any notebook to get started:

```bash
git clone https://github.com/Hou925/Machine-Learning-Projects.git
cd Machine-Learning-Projects
jupyter notebook
```

Dependencies vary by project — check the import cells at the top of each notebook and install as needed (e.g., `pip install scikit-learn tensorflow sklearn-crfsuite`).
