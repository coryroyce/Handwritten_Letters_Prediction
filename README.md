# Handwritten Letter Prediction 

Use EMNIST letter dataset to create a Convolution Neural Network (CNN) machine learning model to predict handwritten letters, then build an interactive demo using live prediction from the custom model.


[Overview Slides]()

[Colab Demo]()

# Project Overview
1. EMNIST Letter Dataset
1. ML Model
1. User Application

# EMNIST Letter Dataset
The EMNIST dataset has a pre-made Python library called [emnist](https://pypi.org/project/emnist/) which made loading the various datasets straight forward and simple. After a few custom functions, it was straight forward to generate quick visualizations of the letters along with their labels.

![Letter Data Visualization with Label](https://github.com/coryroyce/Handwritten_Letters_Prediction/blob/main/reference/labeled_image_A.png)

# ML Model
After creating a few different versions of a Tensorflow Deep Neural Net we ultimately used an architecture that did well in a [Kaggle competition](https://www.kaggle.com/cdeotte/25-million-images-0-99757-mnist) with the 0-9 MNIST digit data set.

![Model Architecture - Image from cdeotte/25-million-images-0-99757-mnist](https://github.com/coryroyce/Handwritten_Letters_Prediction/blob/main/reference/model_architecture_diagram.png)

# User Application
To create an interactive experience for users to draw handwritten digits and provide model prediction in real time, we used [Streamlit](https://streamlit.io/) to create our [front end application](https://github.com/coryroyce/Handwritten_Letters_Prediction/tree/main/streamlit_application). This demo can easily be run in out [Streamlit_App.ipynb](https://github.com/coryroyce/Handwritten_Letters_Prediction/blob/main/streamlit_application/Streamlit_App.ipynb) Colab notebook.

![App Example](https://github.com/coryroyce/Handwritten_Letters_Prediction/blob/main/reference/app_demo_image.png)

# Reference

## Data Set References

[Original EMNIST Paper](https://arxiv.org/pdf/1702.05373.pdf)

EMNIST dataset: https://www.nist.gov/itl/iad/image-group/emnist-dataset

Direct download: http://www.itl.nist.gov/iaui/vip/cs_links/EMNIST/gzip.zip

Cohen, G., Afshar, S., Tapson, J., & van Schaik, A. (2017). EMNIST: an extension of MNIST to handwritten letters. Retrieved from http://arxiv.org/abs/1702.05373

Importing and formatting Image data inspired by [ArangurenAndres/EMNSIT-Image-classification](https://github.com/ArangurenAndres/EMNSIT-Image-classification/blob/master/cognition_project.ipynb)

Mapping and original file reference [Website](https://www.kaggle.com/crawford/emnist/version/1?select=emnist-balanced-mapping.txt)

## Classification Reference

Image Classification in 10 Minutes with MNIST Dataset [Article](https://towardsdatascience.com/image-classification-in-10-minutes-with-mnist-dataset-54c35b77a38d)

How to Develop a CNN for MNIST [Article](https://machinelearningmastery.com/how-to-develop-a-convolutional-neural-network-from-scratch-for-mnist-handwritten-digit-classification/)

Kaggle Competition with MNIST 0-9 digits [Article](https://www.kaggle.com/cdeotte/25-million-images-0-99757-mnist)

Image dimensionality reduction and prediction project [github repo](https://github.com/coryroyce/emnist_letter_exploration_and_prediction)
