## Diabetic-Retinopathy-Classification WebbAppBot using Deep Learning: CNN and NLP 

## Objective:

The objective of this project is to make information and diagnosis of Diabetic Retinopathy accessible to diabetes patients and also to assist ophthalmologist in diagnosing the disease. The project will reduce the window, between the testing and start of treatment, significantly

## Table of Contents
1. [Obtaining the Datasets](#data)
2. [Loading and Preprocessing](#preprocessing)
    * [Loading Images](#download-all-images)
    * [Resize Images](#crop-and-resize-all-images)
    * [Class Imbalance](#Class-Imbalance)
3. [Model Architecture](#neural-network-architecture)
5. [Web Deployment](#web-deployment)
8. [Authors](#Authors)

## Obtaining the Datasets

* Classification Images: The scanned images originates from [Kaggle competition](https://www.kaggle.com/c/aptos2019-blindness-detection).
* Corpus Dataset: Created the corpus by web-scraping [MedicineNet](https://www.medicinenet.com).

### Installation

Install:

* [Anaconda](https://www.continuum.io/downloads)
* [Python (Minimum 3)](https://www.continuum.io/blog/developer-blog/python-3-support-anaconda)
* [Keras for Model deployment](https://pypi.org/project/Keras/)
* [Seaborn for visualization](https://seaborn.pydata.org/)
* [OpenCV for cleaning the images](https://pypi.org/project/opencv-python/)
* [anvil for web deployment](https://anvil.works)

## Loading and Preprocessing

### The NLP Model was processed on the Google Colab while the Image classification was processed on my personal machine.


### Resize All Images
The images were of different sizes. I created Height and width columns for each images and resized the images to the average of height and width using openCV before feeding the to the model 

### Class Imbalance
Applied data augmentation to the dataset using image data generator with keras, I 

## Training the Model:
After trying different method to train the classification model, ResNet50 was used for feature extraction applied on the augmented data to train the image classification model. For the natural language processing, i used fasttext to handle any out of vocabulary text using fasttext representation algoritm


## Web Deployment
The webapp is hosted on anvil.works [### retinopathyBOT](https://retinopathyBOT.anvil.app)


## Authors

* **[Omolewa Davids](https://www.omolewadavids.com)**

