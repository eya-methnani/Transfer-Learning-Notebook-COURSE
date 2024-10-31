# Transfer Learning with VGG16 and ResNet50 Models

This notebook is part of a deep learning course task assigned by Dr. Amal Tarifa. It demonstrates the use of transfer learning with the pre-trained VGG16 and ResNet50 models for image classification and feature extraction. The notebook includes detailed steps for loading, preprocessing, and predicting images with these models.

## Sections Overview

* ### Setup and Library Imports:
  * Imports necessary libraries such as `keras.applications` for model architectures, `keras.preprocessing` for image processing, and additional utility libraries for handling URLs and saving data.

* ### VGG16 Model for Image Classification:
  * **Image Loading and Preprocessing**:
    * Loads an image from a URL, resizes it to fit the VGG16 input requirements (224x224 pixels), and prepares it for model input.
  * **Model Loading and Prediction**:
    * Loads the VGG16 model pre-trained on ImageNet, predicts the class probabilities of the loaded image, and decodes the top prediction.
  * **Top Prediction Display**:
    * Prints the highest probability prediction (e.g., "Appenzeller (62.48%)") to indicate the classified object and confidence level.

* ### Displaying All Predicted Classes and Probabilities:
  * Lists and sorts the top predictions by probability, displaying the most likely classes for better interpretability.

* ### ResNet50 Model for Image Classification:
  * **Image Loading and ResNet50 Model Prediction**:
    * Loads the ResNet50 model and applies the same preprocessing steps as VGG16, performing classification and showing the top predicted classes and their probabilities.

* ### Feature Extraction using VGG16:
  * **Image Preprocessing and Model Modification**:
    * Loads the VGG16 model, removes its final classification layer, and uses it to extract high-level features.
  * **Feature Saving**:
    * Saves the extracted feature vector (4096-dimensional) to a file, which can be used for further machine learning tasks like clustering or similarity comparisons.

* ### Exporting and Reusing Features:
  * Stores the extracted features in `dog.pkl` for reuse, reducing the need for redundant computation when working with the same images in subsequent analyses.

## Summary
This notebook serves as an example of leveraging pre-trained models for both classification and feature extraction tasks. It can be expanded to explore fine-tuning, custom classification, and further analysis of extracted features.
