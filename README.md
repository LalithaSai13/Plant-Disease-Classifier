# 🌿 Plant Disease Classifier

A deep learning model built using **PyTorch** to classify plant diseases from leaf images with high accuracy. The model uses a **Convolutional Neural Network (CNN)** architecture and achieves **92.4% test accuracy** on the dataset.

---

## 📌 Features

- CNN architecture with `Conv2d`, `ReLU`, `MaxPool2d`, and `Dropout` layers
- High-accuracy plant disease detection (**92.4%**)
- Built using `PyTorch` and `Torchvision` for seamless image processing
- Supports RGB image inputs resized to **150x150**
- Uses `CrossEntropyLoss` and the `Adam` optimizer
- Easy dataset integration with `ImageFolder` and `DataLoader`
- Structured and modular code for flexibility and experimentation

---

## 🧠 Model Architecture

```
Input Image (3x150x150)
↓
Conv2d (3 → 32) + ReLU + MaxPool2d
↓
Conv2d (32 → 64) + ReLU + MaxPool2d
↓
Flatten
↓
Linear → ReLU → Dropout
↓
Linear → Output (Number of classes)
```

---

## 🗂 Dataset

This project uses a dataset of plant leaves categorized into disease classes. Images are organized in the following format:

```
dataset/
├── class1/
│   ├── image1.jpg
│   └── ...
├── class2/
│   └── ...
```

Update the `root` path in the code to point to your dataset location.

---

## ⚙️ Setup & Usage

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/plant-disease-classifier.git
cd plant-disease-classifier
```

### 2. Install dependencies

```bash
pip install torch torchvision
```

### 3. Run the training script

Make sure your dataset is placed correctly. Then, run:

```bash
python train.py
```

### 4. Evaluate the model

The test accuracy will be printed after training completes.

---

## 📊 Results

- **Accuracy:** 92.4%
- **Loss Function:** CrossEntropyLoss
- **Optimizer:** Adam
- **Input Size:** 3 x 150 x 150

---

## 🧪 Future Work

- Add support for real-time inference
- Deploy the model using Flask or FastAPI
- Integrate Grad-CAM for visual explanation

---

## 📎 License

This project is open-source and available under the [MIT License](LICENSE).

---
