# Facial Expression Recognition (Transfer Learning)

This project focuses on classifying human facial expressions into eight distinct emotions using a deep learning approach based on **transfer learning** with the **MobileNetV2** architecture.

---

## Emotions Detected

The model is trained to recognize the following 7 emotions:

- Anger
- Disgust
- Fear
- Happy
- Neutral
- Sad
- Surprised

---

## Dataset

The dataset consists of facial images grouped by emotion. Each emotion class contains images collected from various individuals. The original structure was reorganized into labeled folders corresponding to each emotion.

---

## Methodology

- **Preprocessing**: Images are resized to 224x224, normalized using ImageNet means and standard deviations.
- **Model**: MobileNetV2 pre-trained on ImageNet, with its classifier head modified to suit an 8-class classification task.
- **Freezing Strategy**: Feature extractor layers are frozen while the classifier head is trained.
- **Training Configuration**:
  - Optimizer: Adam
  - Loss Function: CrossEntropyLoss
  - Epochs: 10
  - Batch Size: 32

---

## Results

The model achieved high validation accuracy within 10 epochs. Training and validation curves for both accuracy and loss are plotted for performance analysis.

---

## How to Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/facial-expression-recognition.git
   cd facial-expression-recognition
   ```

2. **Install the required dependencies:**:
   ```bash
   pip install -r requirements.txt
   ```
   
3. **Clone the repository**:
   ```bash
   git clone https://github.com/shahmi0519/Facial-Expression-Recognition.git
   cd Facial-Expression-Recognition
   ```

4. **Prepare your dataset**:
   ```bash
   https://www.kaggle.com/datasets/apollo2506/facial-recognition-dataset
   ```

---

## Folder Structure
```bash
facial-expression-recognition/
├── notebooks/
│   └── facial_expression_recognition.ipynb
├── facial_expression_model.pth
├── requirements.txt
└── README.md
```
---

## Requirements

Install the following Python packages:

- torch
- torchvision
- matplotlib
- tqdm

---

## License

This project is licensed under the MIT License.
