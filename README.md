# Melanoma Skin Cancer Detection
In cancer, there are over 200 different forms. Out of 200, melanoma is the deadliest form of skin cancer. The diagnostic procedure for melanoma starts with clinical screening, followed by dermoscopic analysis and histopathological examination. Melanoma skin cancer is highly curable if it gets identified at the early stages. The first step of Melanoma skin cancer diagnosis is to conduct a visual examination of the skin's affected area. Dermatologists take the dermatoscopic images of the skin lesions by the high-speed camera, which have an accuracy of 65-80% in the melanoma diagnosis without any additional technical support. With further visual examination by cancer treatment specialists and dermatoscopic images, the overall prediction rate of melanoma diagnosis raised to 75-84% accuracy. The project aims to build an automated classification system based on image processing techniques to classify skin cancer using skin lesions images.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
 In the skin biopsy, the dermatologist takes some part of the skin lesion and examines it under the microscope. The current process takes almost a week or more, starting from getting a dermatologist appointment to getting a biopsy report.
 The aims to shorten the current gap to just a couple of days by providing the predictive model.
 The approach uses Convolutional Neural Network (CNN) to classify nine types of skin cancer from outlier lesions images. This reduction of a gap has the opportunity to impact millions of people positively.

 ### Business Problem
 The overarching goal is to support the efforts to reduce the death caused by skin cancer. The primary motivation that drives the project is to use the advanced image classification technology for the well-being of the people. Computer vision has made good progress in machine learning and deep learning that are scalable across domains.

 ### Dataset
The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images.

## Conclusions
1. When the model was trained with normal layers, it was quite overfitting, Training Accuracy was 90.24% while accuracy on validation was only 51.01 %. It was quite overfitting.
2. To overcome this issue, I have tried augmentation process where the image is randomly flipped, rotated, zoomed or shifted and also added dropout layer. After applying this fix, the overfiting is quite resolved. Training Accuracy became 46.58% and Validation Accuracy became 48%.
3. There was class imbalance in this model. The no of images available for each cancer type was not sufficied, Some were having more images and some were less images. To resolve this, we created randomly 500 images for each class using Augmentor
4. I have also applied BatchNormatization and noticed that model is now performing better than before. Final Training Accuracy is 67% and Validation Accuracy is 57%

## Technologies Used
pandas - 2.2.2
numpy - 1.26.4
matplotlib - 3.8.4
pathlib
os 
PIL
glob


## Acknowledgements
Give credit here.
- This project was inspired by...
- This project was based on [this tutorial](https://en.wikipedia.org/wiki/Melanoma).


## Contact
Created by [@manojshah2] - feel free to contact me!