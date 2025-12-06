Human Activity Recognition Using Smartphone Accelerometer Data

This project performs Human Activity Recognition (HAR) using accelerometer signals from the WISDM dataset. A complete pipeline is implemented—from data extraction to classical machine learning and a state-of-the-art deep learning model—optimized for speed, robustness, and realistic subject-based evaluation.

Smartphone accelerometers produce continuous motion data along three axes (X, Y, Z). These signals are segmented into sliding windows and used to classify activities such as walking, jogging, climbing stairs, sitting, standing, and other motions.

The system includes:

FAST feature extraction (24 time-domain features per axis)

FAST window extraction (60×3 windows with 50% overlap)

Subject-based train/test splitting to avoid identity leakage

Classical ML models: Linear SVM, Logistic Regression, Random Forest

DeepConvLSTM-SE model inspired by state-of-the-art HAR research

Evaluation metrics: Accuracy, Balanced Accuracy, Cohen’s Kappa, Macro-F1

The deep learning model uses convolutional layers, attention (SE blocks), and LSTMs to capture both short-term and long-term temporal patterns in motion signals. Classical models operate on flattened windows for fast benchmarking.

All models are compared on the same unseen-subject test split, ensuring realistic generalization performance.

Dataset:
WISDM Smartphone Accelerometer Dataset
🔗 https://drive.google.com/drive/folders/17QlLns0yeUwAtsNoGql2sfWLvA6_Hptl?usp=sharing
