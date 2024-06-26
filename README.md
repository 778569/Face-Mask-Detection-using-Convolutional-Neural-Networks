# Face-Mask-Detection-using-Convolutional-Neural-Networks
 One example of a GitHub repository for face mask detection using Convolutional Neural Networks is "chandrikadeb7/Face-Mask-Detection." This repository provides a Python implementation using TensorFlow and Keras for detecting face masks in images.

## Project Overview

![image](https://github.com/778569/Face-Mask-Detection-using-Convolutional-Neural-Networks/assets/52319671/b5ee0376-9c8e-486b-bebe-ae1df97079d6)

* get the image with a face
* apply the cascade classifire
* give me the rigion on instrect of the face, it give face location and face height and width.
* take the face and pass it to a pre train CNN
* it will give output probability of with the mask or without mask.

## Dataset

The dataset consisted of 1376 images, 690 face images with masks and 686 without masks. The original dataset is prepared by Prajna Bhandary and available at Github<br><br> 
https://github.com/prajnasb/observations/tree/master/experiements/data


![image](https://github.com/778569/Face-Mask-Detection-using-Convolutional-Neural-Networks/assets/52319671/2f0ef47a-38cd-44a2-923e-6ac48a8e2b10)
this dataset use for CNN training.

### Data Preprocessing
![image](https://github.com/778569/Face-Mask-Detection-using-Convolutional-Neural-Networks/assets/52319671/160ae772-3473-4bcf-a506-f471f82a09d5)

* Convert image color in to gray scale
* Need comon size - so resize the images to 100 x 100 px

## Training the data using CNN

![image](https://github.com/778569/Face-Mask-Detection-using-Convolutional-Neural-Networks/assets/52319671/19ef69d4-e7c8-4197-9398-d98cfe5cc077) <br><br>

* this has two convolutional layers.
* input 100x100 image for this one.
* in here having 200 cornals 3x3 the first convolutional layer.
* 2nd layer 100 and 3x3 cornals.
* that convolutions I am going to Flatten
* next connect with dense layer with 50 neurons
* Final dense layer will be output layer. it has two neurons, with and without mask. 


## Detecting masks

* input image through a cascade classifire
* Detect the face
* crop the image
* Convert in to 100 x 100 image
* And passed my trained CNN
* wich predict weather with mask or without mask.













