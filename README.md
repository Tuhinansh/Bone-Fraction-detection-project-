# Bone Fracture Detection using DenseNet121

This project implements an automated **Bone Fracture Detection System** using **Deep Learning** and **DenseNet121**. The system classifies X-ray images into two categories:

* **Normal**
* **Fractured**

The project includes data preprocessing, model training, evaluation, and deployment-ready architecture.

---

## 📂 Project Structure

```
├── Dataset/
│   ├── train/
│   │   ├── normal/
│   │   └── fractured/
│   └── val/
│       ├── normal/
│       └── fractured/
├── model/
│   └── best_model.h5
├── src/
│   ├── preprocess.py
│   ├── train.py
│   ├── evaluate.py
│   └── utils.py
├── README.md
└── requirements.txt
```

---

## 📘 Description

This project uses the **DenseNet121 CNN architecture** for classifying bone X-ray images. DenseNet’s dense connectivity helps detect subtle fracture lines and micro-cracks.

The model was trained using:

* **Binary Cross Entropy loss**
* **Adam optimizer**
* **Learning rate = 1e-4**
* **Batch size = 8**
* **Image size = 384×384**

The dataset includes real-world X-ray images from Kaggle.

---

## 🛠 Features

* Fully automated fracture classification
* Preprocessing pipeline with augmentation
* DenseNet121 transfer learning
* High accuracy and generalization performance
* Modular code (easy to extend)
* Ready for deployment (Flask/Streamlit/TFLite compatible)

---

## 📊 Model Performance

* **Accuracy:** ~90–94%
* **Precision / Recall:** Balanced detection
* **AUC:** High (>0.90)

Plots included during training:

* Accuracy vs Epochs
* Loss vs Epochs
* ROC Curve
* Confusion Matrix

---

## ⚙ Installation

### 1. Clone the repository

```
git clone https://github.com/username/bone-fracture-detection.git
cd bone-fracture-detection
```

### 2. Install dependencies

```
pip install -r requirements.txt
```

---

## ▶ Training the Model

```
python src/train.py
```

The script will:

* Load and preprocess images
* Train DenseNet121
* Save best model as `best_model.h5`

---

## 🧪 Evaluating the Model

```
python src/evaluate.py
```

Generates:

* Accuracy metrics
* Confusion matrix
* Predictions on validation set

---

## 🚀 Deployment

You can deploy the model using:

* **Streamlit** (web app)
* **Flask** API
* **TensorFlow Lite** for mobile

Example Streamlit command:

```
streamlit run app.py
```

---

## 📎 Dataset

Dataset used: **Bone X-Ray Images (Normal vs Fractured)** from Kaggle.
Organized into train and validation folders.

---

## 🤝 Contributions

Contributions, issues, and improvements are welcome.

---

## 📜 License

This project is licensed under MIT License.

---

## 🙌 Acknowledgements

* Kaggle for providing dataset
* DenseNet authors for architecture
* TensorFlow/Keras community
