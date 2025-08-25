# Eid-Al-Adha-2025-Sheep-Classification-Challenge

## Sheep Image Classification Project using Deep Learning
Project Overview:
The goal of this project is to build a model to classify sheep images into different breeds using deep learning techniques. The project uses the ResNet18 pretrained model, which is fine-tuned to suit our specific dataset.

## Project Components:
1- Data Loading: The dataset, consisting of sheep images, is loaded from a compressed file and extracted to the appropriate directory. A CSV file containing the breed labels associated with each image is also loaded.

2- Data Preprocessing: Several transformations are applied to the images to improve data diversity, including resizing, random cropping, and random rotation.

3- Data Splitting: The dataset is divided into training and validation sets using random split techniques while maintaining the distribution of the classes. Class weights are applied to handle class imbalance.

4- Model: The ResNet18 model from the Torchvision library is used and modified to fit the number of classes in our dataset. The model is trained using CrossEntropyLoss and the Adam optimizer.

5- Training: The model is trained over multiple epochs using the train_model function, with early stopping implemented to halt training when performance no longer improves.

6- Prediction: After training, the model is used to predict the breed of new images in the test set, and the predictions are displayed with confidence scores.

## Objective:
The objective of this project is to build a robust model for sheep image classification with high accuracy using deep learning techniques, which can be applied to various image classification tasks involving animals or similar images.
