Love it — let’s make your README look 🔥 GitHub-pro level.

You can copy-paste everything below directly into **README.md**.

---

# 🐱🐶 CNN Image Classification – Custom CNN vs Transfer Learning

![Python](https://img.shields.io/badge/Python-3.x-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Deep%20Learning-orange)
![Keras](https://img.shields.io/badge/Keras-CNN-red)
![Status](https://img.shields.io/badge/Assignment-Completed-success)

---

## 📌 Project Summary

This project implements and compares:

* 🧠 **Custom CNN** built from scratch
* 🚀 **Transfer Learning Model** using a pretrained backbone

on the **Cats vs Dogs** image classification dataset.

We analyze:

✔ Model accuracy
✔ Loss convergence
✔ Computational cost
✔ Impact of Global Average Pooling (GAP)

---

## 🗂 Dataset

| Feature    | Value                |
| ---------- | -------------------- |
| Dataset    | Cats vs Dogs         |
| Classes    | 2                    |
| Split      | 90% Train / 10% Test |
| Image Size | 224 × 224            |

---

## 🧠 Model Architectures

### 🔹 Custom CNN Architecture

![Image](https://www.researchgate.net/publication/336805909/figure/fig1/AS%3A11431281342674890%401743562251174/Schematic-diagram-of-a-basic-convolutional-neural-network-CNN-architecture-26.tif)

![Image](https://ik.imagekit.io/upgrad1/abroad-images/imageCompo/images/unnamed8PDPDZ_1_1ZBHFR.webp)

![Image](https://ars.els-cdn.com/content/image/1-s2.0-S0925231218310610-gr3.jpg)

![Image](https://www.researchgate.net/publication/339096868/figure/fig2/AS%3A11431281391083351%401745306731973/Difference-between-fully-connected-layer-and-global-average-pooling-layer.tif)

* 3 Convolution layers
* MaxPooling layers
* **Global Average Pooling (GAP)**
* Dropout regularization
* Softmax output

---

### 🚀 Transfer Learning (ResNet Backbone)

![Image](https://www.researchgate.net/publication/356162462/figure/fig3/AS%3A1089285335846971%401636717270496/The-architecture-of-the-ResNet-50-network.jpg)

![Image](https://analyticsstepsfiles.s3.ap-south-1.amazonaws.com/backend/media/thumbnail/1967565/9315476_1592890541_transfer.jpg)

![Image](https://www.researchgate.net/publication/362189708/figure/fig3/AS%3A1182053269811212%401658834869925/Feature-extraction-from-the-pre-trained-model-based-feature-extractors-and-classification.png)

![Image](https://www.researchgate.net/publication/374392722/figure/fig4/AS%3A11431281212146082%401702553554994/Pretrained-CNN-utilized-for-feature-extraction-from-the-aerial-image-dataset-The-weight.tif)

* Pretrained CNN feature extractor (frozen layers)
* Global Average Pooling
* Custom classification head

---

## ⚙️ Training Configuration

| Parameter  | Custom CNN                      | Transfer Learning |
| ---------- | ------------------------------- | ----------------- |
| Optimizer  | Adam                            | Adam              |
| Loss       | Sparse Categorical Crossentropy | Same              |
| Epochs     | 20–30                           | 5–10              |
| Batch Size | 32                              | 32                |

---

## 📊 Results

### 🧪 Custom CNN

| Metric    | Value     |
| --------- | --------- |
| Accuracy  | **0.917** |
| Precision | **0.917** |
| Recall    | **0.917** |
| F1 Score  | **0.917** |

**Loss Reduction:**
**76.7% decrease** from initial training loss.

Training Time: ~1260 sec
Parameters: 94,402

---

### 🚀 Transfer Learning

| Metric    | Value  |
| --------- | ------ |
| Accuracy  | ~0.713 |
| Precision | ~0.713 |
| Recall    | ~0.713 |
| F1 Score  | ~0.713 |

Training Time: ~680 sec
Parameters: 266,626

---

## 🔍 Key Insights

✔ Custom CNN outperformed transfer learning by **~20% accuracy**
✔ GAP reduced parameters and minimized overfitting
✔ Transfer learning trained faster but was less effective here
✔ Custom CNN learned domain-specific features better

---

## 📈 Evaluation Metrics

* Accuracy
* Precision (macro)
* Recall (macro)
* F1-score (macro)

---

## 🧩 Assignment Requirements Met

* Custom CNN with GAP
* Transfer learning with frozen backbone
* Loss convergence tracked
* All 4 metrics computed
* Comparative analysis provided
* JSON results output generated

---

## ▶️ How to Run

```bash
1. Open the notebook (.ipynb)
2. Restart & Run All
3. Ensure outputs and final JSON appear
```

---

## 🎯 Conclusion

A well-designed custom CNN can outperform transfer learning when sufficient task-specific data is available, while transfer learning remains computationally efficient.

---
