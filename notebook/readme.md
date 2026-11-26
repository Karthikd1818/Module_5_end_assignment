# AI-Based Image Classification System Using Deep Learning

## Project Overview

This project develops an AI-based image classification system using deep learning techniques to classify images from the CIFAR-10 dataset into 10 different categories.

Two models were developed and compared:
1. Custom Convolutional Neural Network (CNN)
2. MobileNetV2 using Transfer Learning

## Dataset

**Dataset:** CIFAR-10

- Training images: 45,000
- Validation images: 5,000
- Testing images: 10,000
- Image dimensions: 32 × 32 × 3
- Number of classes: 10

### Classes

Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, Truck.

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Project Workflow

### 1. Data Preparation
- Loaded the CIFAR-10 dataset.
- Normalized image pixel values.
- Split the training data into training and validation sets.
- Saved the preprocessed dataset.

### 2. Custom CNN Development
- Built a CNN using convolutional and pooling layers.
- Added fully connected layers and dropout.
- Trained the model using CIFAR-10 images.

### 3. Transfer Learning
- Used pretrained MobileNetV2 with ImageNet weights.
- Resized images to 96 × 96.
- Applied MobileNetV2 preprocessing.
- Froze the pretrained base model.
- Added a custom classification head and trained it.

### 4. Model Evaluation
- Evaluated both models on the test dataset.
- Generated predictions.
- Compared classification performance.

## Model Performance

| Model | Test Accuracy | Test Loss |
|---|---:|---:|
| Custom CNN | 70.09% | 0.8914 |
| MobileNetV2 | 86.03% | 0.4070 |

MobileNetV2 achieved 15.94 percentage points higher test accuracy than the custom CNN.

## Conclusion

The project demonstrates the effectiveness of deep learning and transfer learning for image classification. MobileNetV2 achieved better performance than the custom CNN on the CIFAR-10 test dataset.

## How to Run

1. Clone or download this repository.
2. Install the required dependencies.
3. Open the Jupyter notebooks.
4. Run the notebooks in the following order:
   - `01_data_preparation.ipynb`
   - `02_cnn_model_development.ipynb`
   - `03_transfer_learning.ipynb`

## Installation

```bash
pip install tensorflow numpy pandas matplotlib scikit-learn jupyter
```

