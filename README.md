## Project name: Pneumonia detection with ML and DL methods

## Table of contents

* [Problem description](#Problem)

* [Data](#Data)

* [Approaches](#Approaches)

* [Pipeline](#Pipeline)

* [Metrics](#Metrics)

* [Results](#Results)

* [Contribution](#Contribution)


## Problem

The main goal of our project is prediction of pneumonia and defining the stage of the disease depending on chest X-rays.

Pneumonia is a lung infection that can sometimes lead to severe or life-threatening illness and even death. It's usually caused by a bacterial infection or a virus.
This disease is a great threat to people, especially children and adults over the age of 65. Pneumonia is the leading cause of death for children under 5: pneumonia killed 740 180 children under the age of 5 in 2019, accounting for 14% of all deaths of children.

To understand the general situation here is an infographic provided. We can see that although the number of pneumonia cases slightly decreases, it still causes a lot of deaths.

![stat](https://user-images.githubusercontent.com/60686300/149668779-846ae977-e5e8-4300-be42-c229db650f05.jpg)

And of course, the coronavirus disease had a major impact on the world. About 15% of COVID-19 cases are severe and cause pneumonia. And about 5% of people have critical infections and need a ventilator.

It is very important to make a diagnosis in time and start treatment immediately. Computed tomography (CT), magnetic resonance imaging (MRI), or radiography (X-rays) is frequently used for diagnosis. X-ray imaging is considered a non-invasive and relatively inexpensive examination of the lungs. But the problem is that the contrast in chest X-ray images is rather low, and it sometimes makes manual evaluation inefficient. Besides, X-ray images have similar region information for different diseases, such as lung cancer.

And that is where computers and AI can help. Computer-aided diagnosis can enhance efficiency and lead to timely treatment.


## Data

Our dataset:
* [Pneumonia X-Ray Images](https://www.kaggle.com/pcbreviglieri/pneumonia-xray-images/discussion)

It is well splitted - it consists of 3 directories: train, test and validation, each of which contains other 2 directories: the first one with X-Rays of pneumonia and the second one with normal lungs. Besides, it suits well for the use of machine and deep learning.

Example of X-Rays with normal lungs:

![normal](https://user-images.githubusercontent.com/60686300/149668833-99e0f8f9-6077-438a-97b7-4c59bea543d0.jpg)

Example of X-Rays with pneumonia:

![pneumonia](https://user-images.githubusercontent.com/60686300/149668838-90931d93-bacd-4f69-9084-04defae85071.jpg)

Distibution of data in each dataset (train, test and validation):

![stat2](https://user-images.githubusercontent.com/60686300/149668850-74cc7d72-e894-4ac9-babd-b1583e4b2a4a.jpg)

## Approaches

Pneumonia detection is a classification problem for which various algorithms of machine learning and deep learning mostly are used.
To make it more interesting, we decided to use and analyze both of the approaches.

We have implemented two models of machine learning:
* SVM (support vector machine model)
* XGBoost (Extreme Gradient Boosting model)

Regarding deep learning, we implemented three models:
* CNN
* Resnet
* MobileNet


## Pipeline


1. Data processing
      - Getting train, validation and test datasets.
 
2. Images processing
      - Improvement  of images, getting away unwanted distortions

3. Investigation of Machine Learning models: SVM, Random Forest, Xgboost, K-nearest neighbor.
      - Validation of  model hyperparameters
      - Training and testing data
      - Results evaluation
 
4. Investigation of Deep learning models: CNN, ResNet50, MobileNet:
      - Validation of  model hyperparameters
      - Training and testing data
      - Results evaluation

5. Choosing the best model

## Metrics

In our project we used confusion matrix to evaluate results of ML and NN models.

![matrix](https://user-images.githubusercontent.com/60686300/149668240-aa408d55-029d-4bb8-b8bd-007f545dc7b0.png)


**SVM**

![svm](https://user-images.githubusercontent.com/60686300/149668510-1ceefb7f-fb42-41c7-9567-3feada9ba2d6.png)

**XGBoost**

![boost](https://user-images.githubusercontent.com/60686300/149668694-2f0f49fd-1bbe-4375-8a54-94e3f178dc2e.png)

**CNN**

![cnn](https://user-images.githubusercontent.com/60686300/149668703-2b6fd665-a172-4f83-b75f-0072c54bc493.png)

**ResNet**

![resnet](https://user-images.githubusercontent.com/60686300/149668715-23b0b203-515e-44d6-b1f8-be8b5754593b.png)

**MobileNet**

![mobilenet](https://user-images.githubusercontent.com/60686300/149668721-2df185d9-62ff-4e91-944b-652ac530502c.png)


From thise pictires cam be seen that the best model is MobileNet and we decided to use it.

## Results

We analysed different ML and NN approaches, chose ones that suited our problem. Mostly we worked on finding better ML or NN among chosen ones to get bigger accuracy number.

![pneumonia](https://user-images.githubusercontent.com/60686300/149668737-a23215b4-7391-4b9b-a149-ef50e6a3171d.png)

![normal](https://user-images.githubusercontent.com/60686300/149668743-92d673da-a589-47ff-a4e1-ada46d59ef68.png)

From there can be seen with what probability were found images with pneumonia and normal lungs on trained MobileNet NN.

## Contribution

* Kokolius Khrystyna
* Kyba Sofia


