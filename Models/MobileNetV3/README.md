Image Classification using MobileNetV2
  Overview:
    This notebook demonstrates how to build, train, and evaluate an image classification model using transfer learning     with MobileNetV2.
It covers the full pipeline starting from data preprocessing to model training and evaluation.

The goal is to achieve good performance while keeping the model lightweight and efficient.

Model Architecture

Base Model: MobileNetV2 (pretrained on ImageNet)

Custom classification head added on top

Global Average Pooling

Fully Connected (Dense) layers

Softmax activation for multi-class classification

Framework used:

TensorFlow

Keras

 Notebook Structure
Data Import & Preprocessing

Load image dataset

Resize images to required input size

Normalize pixel values

Apply data augmentation (if enabled)

Split data into training and validation sets

Base Model Setup

Load MobileNetV2 without the top layer

Freeze base model layers to prevent overfitting

Attach custom classification layers

Model Compilation

Optimizer: Adam

Loss function: Categorical Crossentropy

Metrics: Accuracy

Model Training

Train the model on the prepared dataset

Validate performance during training

Optional callbacks:

ModelCheckpoint

EarlyStopping

Evaluation & Results

Evaluate model accuracy on validation/test data

Analyze training and validation performance
