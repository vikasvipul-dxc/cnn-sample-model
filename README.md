🐱🐶 CNN Image Classification – Custom CNN vs Transfer Learning

Course: AIMLCZG511 – Deep Neural Networks
Program: BITS Pilani WILP
Task: Compare a custom CNN with a transfer learning model

📌 Project Summary

This project implements and evaluates two approaches for image classification on the Cats vs Dogs dataset:

Custom CNN built from scratch

Transfer Learning using a pretrained CNN backbone

The goal is to compare:

Model performance

Loss convergence

Computational cost

Impact of Global Average Pooling (GAP)

🗂 Dataset

Name: Cats vs Dogs

Classes: 2 (Cat, Dog)

Train/Test Split: 90/10

Image Size: 224 × 224

🧠 Models
🔹 Custom CNN

Conv2D layers: 3

MaxPooling layers

Global Average Pooling (GAP)

Dropout regularization

Softmax output

🔹 Transfer Learning Model

Pretrained CNN backbone (frozen layers)

Global Average Pooling

Custom classification head

Fine-tuned on dataset

⚙️ Training Configuration
Parameter	Custom CNN	Transfer Learning
Optimizer	Adam	Adam
Loss	Sparse Categorical Crossentropy	Same
Epochs	20–30	5–10
Batch Size	32	32
📊 Results
🧪 Custom CNN
Metric	Value
Accuracy	0.917
Precision	0.917
Recall	0.917
F1 Score	0.917

Loss Reduction:

(
0.6525
−
0.1522
)
/
0.6525
×
100
=
76.7
%
(0.6525−0.1522)/0.6525×100=76.7%

Training Time: ~1260 seconds
Parameters: 94,402

🚀 Transfer Learning
Metric	Value
Accuracy	~0.713
Precision	~0.713
Recall	~0.713
F1 Score	~0.713

Training Time: ~680 seconds
Parameters: 266,626

🔍 Key Insights

Custom CNN outperformed transfer learning by ~20% accuracy.

GAP reduced parameters and helped prevent overfitting.

Transfer learning trained faster but was less effective for this dataset.

Custom CNN learned dataset-specific features more effectively.

📈 Evaluation Metrics

Accuracy

Precision (macro)

Recall (macro)

F1-score (macro)

🧩 Assignment Requirements Met

✔ Custom CNN with GAP
✔ Transfer learning with frozen backbone
✔ Loss convergence tracked
✔ All 4 metrics computed
✔ Comparative analysis provided
✔ JSON results output generated

▶️ How to Run
1. Open notebook (.ipynb)
2. Restart & Run All
3. Ensure outputs and final JSON results appear

🎯 Conclusion

A well-designed custom CNN can outperform transfer learning when sufficient task-specific data is available, though transfer learning remains computationally efficient.
