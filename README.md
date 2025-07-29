# 🦴 Fracture Detection Using Deep Learning

This project focuses on detecting bone fractures in X-ray images using deep learning techniques. It employs multiple pretrained convolutional neural networks (CNNs) such as **DenseNet121**, **ResNet50**, **VGG16**, **MobileNet**, and **InceptionV3** for image classification.

The notebook includes training workflows, precision policies, model comparisons, and predictions—making it a complete pipeline for automated fracture detection.

## 🧠 Objective

- Automatically classify X-ray images as **fractured** or **normal**
- Compare performance of different CNN architectures
- Leverage transfer learning using pretrained models
- Utilize mixed-precision training for performance optimization

## 🗂️ Project Structure

fracture-detection/
├── fracture-detection.ipynb     # Main notebook
├── models/                      # Saved model weights (optional)
├── images/                      # X-ray samples and plots
├── results/                     # Accuracy plots, predictions
├── requirements.txt             # Auto-generated from notebook
└── README.md                    # You're here


## 🔍 Key Features

- ✅ Binary image classification
- ✅ Multiple pretrained CNNs (DenseNet, ResNet, VGG, MobileNet, etc.)
- ✅ Image preprocessing & data augmentation
- ✅ Training history plots
- ✅ Test-time predictions and visualization
- ✅ Mixed-precision policy support (`keras.mixed_precision`)


## 📦 Dataset Requirements

Your dataset should be structured as follows:

data/
├── train/
│   ├── fractured/
│   └── normal/
└── test/
├── fractured/
└── normal/


You can use publicly available datasets like:
- [MURA – Stanford ML Group](https://stanfordmlgroup.github.io/competitions/mura/)
- [RSNA Bone Fracture Detection – Kaggle](https://www.kaggle.com/competitions/rsna-bone-age)


## 🚀 Getting Started

### 1. Clone the Repository

git clone https://github.com/your-username/fracture-detection.git
cd fracture-detection

### 2. Install Dependencies

Install the required libraries using pip:

pip install -r requirements.txt

Or install manually (see libraries below).

### 3. Run the Notebook

jupyter notebook

Open `fracture-detection.ipynb` and execute all cells step-by-step.

## 🧪 Libraries Used

* `numpy`, `os`, `matplotlib`, `pandas`
* `keras`, `tensorflow`, `keras.applications`
* Pretrained models: `DenseNet121`, `ResNet50`, `InceptionV3`, `MobileNet`, `VGG16`, `Xception`
* `keras.mixed_precision` for policy setting
* `collections.Counter` (for dataset distribution)


## 📊 Evaluation

The notebook includes:

* Training & validation accuracy/loss plots
* Prediction on test set samples
* Model comparison via classification metrics
* Confusion matrix visualization


## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## Disclaimer

This tool is meant for **educational and research purposes** only. It is **not** certified for clinical use or diagnostics. Always consult a licensed radiologist for medical decisions.
