# Image Classification with FastAI 🖼️🤖

This project demonstrates **image classification** using the **FastAI** library on the **ImageNette** dataset (a subset of ImageNet). The goal is to classify images into 10 categories using a pre-trained **ResNet50** model. 🎯📊

---

## Table of Contents 📑
1. [Overview](#overview-)
2. [Installation](#installation-)
3. [Usage](#usage-)
4. [Code Structure](#code-structure-)
5. [Results](#results-)
6. [License](#license-)

---

## Overview 🚀

This project:
- Uses **FastAI** to build and train an image classification model. 🤖📸
- Leverages **transfer learning** with a pre-trained ResNet50 model. 🧠🔍
- Implements data augmentation, normalization, and fine-tuning for improved performance. 📊📉

---

## Installation 🛠️

To run this project, you need to install the required libraries. Run the following commands:

```bash
!pip install fastai
!pip install torch torchvision
```

---

## Usage 🖥️

1. **Load Dataset**: The script loads the ImageNette dataset using FastAI's data block API.
2. **Preprocess Data**: Applies data augmentation, resizing, and normalization.
3. **Build Model**: Uses a pre-trained ResNet50 model for transfer learning.
4. **Train Model**: Fine-tunes the model using the `fit_one_cycle` method.
5. **Evaluate Results**: Evaluates model performance using accuracy and TTA (Test Time Augmentation).

---

## Code Structure 🗂️

- **Data Preparation**:
  - Loads the ImageNette dataset and prepares it for training.
  - Defines data loaders, transformations, and normalization.

- **Model Definition**:
  - Uses a pre-trained ResNet50 model for transfer learning.
  - Implements label smoothing for improved generalization.

- **Training**:
  - Fine-tunes the model using the `fit_one_cycle` method.
  - Tracks training metrics and evaluates model performance.

- **Evaluation**:
  - Uses TTA (Test Time Augmentation) to improve prediction accuracy.
  - Visualizes training progress and model predictions.

---

## Results 📊

- **Training Accuracy**: The model achieves high accuracy on the ImageNette dataset.
- **Fine-Tuning**: Fine-tuning improves model performance significantly.
- **TTA**: Test Time Augmentation further boosts prediction accuracy.

---

## License 📜

This project is licensed under the **MIT License**. Feel free to use, modify, and distribute it as needed.

---

## Example Output 🖼️

Here’s an example of the model's training progress:

```plaintext
Epoch 1: train_loss=0.123, val_loss=0.045, accuracy=0.987
Epoch 2: train_loss=0.045, val_loss=0.032, accuracy=0.991
```

---

## Dependencies 📦

- `fastai`
- `torch`
- `torchvision`

---

## Author 👨‍💻

This project was created by **[Navid Falah](https://github.com/navidfalah)**. Feel free to reach out for questions or collaborations at **navid.falah7@gmail.com**! 🤝
