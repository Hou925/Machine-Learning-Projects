# Machine-Learning-Projects

一套涵盖**分类、回归、聚类、序列标注与音频识别**的端到端机器学习项目合集，每个方向均提供多种模型实现，便于横向对比与学习。

> For English version, see [README.md](./README.md)

---

## 项目目录

### 1. 🖼️ FashionMNIST 图像分类
**路径：** `Classification_FashionMNIST/`

对 FashionMNIST 数据集的 10 类服装图像进行分类，并排对比三种建模思路：
- **随机森林**（`FashionMNIST_classification_Forest_Model.ipynb`）
- **神经网络**（`FashionMNIST_classification_NN_Model.ipynb`）
- **支持向量机**（`FashionMNIST_classification_SVM_Model.ipynb`）

---

### 2. 🔵 FashionMNIST 图像聚类
**路径：** `Clustering_FashionMNIST/`

在无监督场景下对 FashionMNIST 图像进行分组，探索三种差异化策略：
- **自编码器（Autoencoder）**——先学习低维潜在表示，再执行聚类（`FashionMNIST_clustering_Autoencoder_Model.ipynb`）
- **DBSCAN**——基于密度的聚类，无需预先指定簇数（`FashionMNIST_clustering_DBSCAN_Model.ipynb`）
- **K-Means**——经典质心聚类算法（`FashionMNIST_clustering_Kmeans_Model.ipynb`）

---

### 3. 🏠 加利福尼亚房价回归
**路径：** `Regression_California_Housing/`

对加州房价数据集进行价格预测，对比两类模型在可解释性与性能上的权衡：
- **随机森林**（`California_Housing_Regression_Forest_Model.ipynb`）
- **神经网络**（`California_Housing_Regression_NN_Model.ipynb`）

---

### 4. 🀄 CRF 中文分词
**路径：** `CRF_Chinese_Segmentation_Model/`

基于**条件随机场（CRF）**的中文分词序列标注模型：
- 使用《人民日报》语料库进行数据预处理（`corpus_process.ipynb`）
- 采用 BMES 标注体系实现字级别分词
- 包含完整的训练与评估流程（`crf_model.ipynb`）

---

### 5. 🎵 简易音频分类器
**路径：** `simple-audio-model based on google-teachable-machine/`

借助 **Google Teachable Machine** 在浏览器内零代码完成音频模型训练：
- 识别类别：背景噪音、拍手声、敲桌声、金属碰撞声
- 导出为可直接部署的 TensorFlow.js 模型（`model.json` + `weights.bin`）
- 全程无需编写训练代码，适合快速原型验证

---

## 技术栈

| 领域 | 工具 / 库 |
|------|----------|
| 深度学习 | TensorFlow / Keras |
| 传统机器学习 | scikit-learn |
| 序列标注 | sklearn-crfsuite |
| 数据处理 | NumPy、Pandas |
| 可视化 | Matplotlib |
| 音频（无代码） | Google Teachable Machine |

---

## 快速开始

各子项目均以独立的 Jupyter Notebook 形式呈现，克隆仓库后直接打开即可运行：

```bash
git clone https://github.com/Hou925/Machine-Learning-Projects.git
cd Machine-Learning-Projects
jupyter notebook
```

各项目依赖有所不同，请参考每个 Notebook 顶部的 `import` 单元格，按需安装（例如 `pip install scikit-learn tensorflow sklearn-crfsuite`）。
