# 🦋 Butterfly Species Classifier (Monarch, Painted Lady, Admiral) [AI assingment]

This project is an AI-based image classification model that was an assignment as part of my AI module in my Computer Science course.
This model distinguishes between three species of butterfly:
- Monarch
- Painted Lady
- Admiral
It was built using TensorFlow and Keras in Jupyter Notebook, it explores different modelling approaches such as baseline convolutional network, augmented training, and transfer learning.

## Technologies Used
- Python
- TensorFLow/ Keras
- Jupyter Notebook
- NumPy, Matplotlib
  
## Dataset
The dataset consists of labeled butterfly images (200 of each class). The data was processed using the following steps:
- Resized to **224x224**
- One-hot encode for categorical classification
- Shuffled before training for randomness

## Models used
### 1. **Baseline CovNet**
A simple convolutional network used as a benchmark. Establishes a performance baseline.

### 2. **CovNet + Data Augmentation & Dropout**
Improved version of the baseline with:
- RandomFlip
- RandomRotation
- RandomZoom
- RandomTranslation
- Dropout(0.5)
Helps to reduce overfitting and improce generalisation.

### 3. **Transfer Learning: ResNet 50**
Leveraged a pretrained ResNet50 model with a custom classifier head with:
- Conv2D
- MaxPooling
- Flatten
- Dense(3 softmax)
Some layers of the ResNet50 model were unfrozen to help fine-tune the model.

## Credits
Created by Peace Samuel. Part of my 4th year Computer Science course.
