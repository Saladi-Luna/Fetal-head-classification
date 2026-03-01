# Fetal Head Classification

A deep learning project for automated classification of fetal head standard planes in ultrasound images.

## Overview

This project applies convolutional neural networks (CNNs) to classify fetal head ultrasound images into standard anatomical planes. Accurate identification of these planes is essential for routine prenatal screening, enabling clinicians to take reliable biometric measurements such as head circumference (HC) and biparietal diameter (BPD).

The three standard fetal head planes targeted in this project are:
- **Transcerebellar (TC)** — used to visualize the cerebellum and cisterna magna
- **Transthalamic (TT)** — the standard plane for measuring biparietal diameter and head circumference
- **Transventricular (TV)** — used to assess the lateral ventricles

## Dataset

The model was trained and evaluated on fetal head ultrasound images. Each image is labeled with one of the three standard planes (TC, TT, TV) or marked as "other" if it does not correspond to a standard plane.

> **Note:** Due to patient privacy and data sharing regulations, the dataset is not included in this repository. Please refer to publicly available fetal ultrasound datasets such as the [HC18 Grand Challenge](https://hc18.grand-challenge.org/) if you wish to reproduce these experiments.

## Model Architecture

The classification pipeline is built on a CNN-based architecture with the following components:

- **Backbone:** Pre-trained convolutional network (e.g., VGG16 / ResNet50) used as a feature extractor
- **Transfer Learning:** ImageNet pre-trained weights fine-tuned on the fetal ultrasound dataset
- **Classifier head:** Fully connected layers with dropout regularization
- **Output:** Softmax activation over the class labels

## Requirements

- Python 3.8+
- TensorFlow / Keras or PyTorch
- NumPy
- OpenCV
- scikit-learn
- Matplotlib

Install dependencies with:

```bash
pip install -r requirements.txt
```

## Usage

### Training

```bash
python train.py --data_dir /path/to/dataset --epochs 50 --batch_size 32
```

### Evaluation

```bash
python evaluate.py --data_dir /path/to/dataset --model_path /path/to/model.h5
```

### Inference

```bash
python predict.py --image /path/to/image.png --model_path /path/to/model.h5
```

## Results

| Metric    | Score |
|-----------|-------|
| Accuracy  | —     |
| Precision | —     |
| Recall    | —     |
| F1 Score  | —     |

*Results will be updated after model training and evaluation.*

## Project Structure

```
Fetal-head-classification/
├── data/               # Dataset directory (not tracked)
├── models/             # Saved model weights
├── notebooks/          # Jupyter notebooks for exploration and analysis
├── src/
│   ├── train.py        # Training script
│   ├── evaluate.py     # Evaluation script
│   ├── predict.py      # Inference script
│   └── utils.py        # Helper functions
├── requirements.txt    # Python dependencies
├── LICENSE
└── README.md
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
