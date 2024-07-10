# Web-Scraping-and-Deep-Learning
This project involves automating the classification of fashion products (shirts) based on their gender and sleeve type using web scraping and deep learning techniques. 

# Project Title: Automated Fashion Product Classification using Web Scraping and Deep Learning
##Project Overview:
This project involves automating the classification of fashion products (shirts) based on their gender and sleeve type using web scraping and deep learning techniques. Here’s a breakdown of the project:

## Web Scraping with Selenium:

**Objective**: Gather data from Myntra's website on full-sleeve and half-sleeve shirts for both men and women.

**Tools Used**: Selenium for web automation, Pandas for data manipulation, and Requests for image downloading.

**Details**:

Selenium is used to navigate through each URL, extract product images, metadata (brand, name, price), and classify them by gender and sleeve type.

Images are downloaded and saved locally, and metadata is stored in a CSV (myntra_data.csv).

## Image Classification:

**Objective**: Develop two classification models using TensorFlow/Keras for gender and sleeve type.

**Models Used**: Convolutional Neural Networks (CNNs).

**Details**:

Images from the CSV are loaded, resized to 128x128 pixels, and preprocessed.

Two separate CNN models are created and trained:

1. Gender Classification: Determines whether the product is for males or females.

2. Sleeve Type Classification: Identifies whether the shirt is full-sleeve or half-sleeve.

Models are compiled with categorical cross-entropy loss and trained using a train-test split of the dataset.

## Prediction on New Images:

**Objective**: Predict the gender and sleeve type of new shirt images using trained models.

**Details:**

New image paths are provided for prediction.
Images are loaded, preprocessed, and fed into the trained models.

Predictions are made and displayed alongside the corresponding images.

## Code Explanation:

**Web Scraping:** Uses Selenium to automate browsing, extract product details, and download images. Metadata and image paths are saved into a CSV.

**Image Loading and Preprocessing**: Loads images from paths stored in the CSV, resizes them to fit the model input, and prepares them for training.

**Model Creation and Training**: Defines CNN architectures for gender and sleeve type classification. Trains each model separately using the preprocessed image data.

**Prediction Function**: Loads new images, preprocesses them, and uses trained models to predict their gender and sleeve type.

This project combines web scraping for data collection and deep learning for image classification, demonstrating an end-to-end pipeline for automated fashion product classification.
--------------






