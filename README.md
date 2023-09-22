# Plastic Detection in Rivers

## Overview

This project aims to address the critical issue of plastic pollution in rivers by developing a model for the automatic detection of plastic waste in river environments. The project utilizes a dataset from the Reva University Plastic Free Rivers Hackathon, which has been annotated to create ground truths for training a machine learning model. The model has been trained using Roboflow and is accessible through the Roboflow API for plastic detection predictions.

## Dataset

The dataset used in this project is sourced from the Reva University Plastic Free Rivers Hackathon. It contains a collection of images depicting river environments, some of which contain plastic waste. To facilitate the development of a machine learning model, the dataset has been annotated to define ground truths, i.e., marking the locations of plastic waste within the images.

### Dataset Structure

The annotated dataset has been organized into the "PlasticDetectionRivers" directory within this repository. This directory contains both the images and the labels (annotations) for training the model.

## Model Training

The model for plastic detection in rivers has been trained using Roboflow, a powerful platform for computer vision tasks. To replicate the training process or make predictions using the pre-trained model, you'll need to use the Roboflow API.

### Steps to Train the Model 

1. **Clone the yolov5 repository** link to clone - https://github.com/ultralytics/yolov5.git. Here we are making a custom model where num_classes = 1 i.e plastic and fine tuning the yolov5 model which is trained on 80 different classes.  

1. **Sign Up on Roboflow:** If you don't already have an account, sign up on the Roboflow platform at [Roboflow](https://roboflow.com/).

2. **Upload the Dataset:** Create a new dataset on Roboflow and upload the annotated dataset from the "PlasticDetectionRivers" directory.

3. **Training:** Train the model on Roboflow using the uploaded dataset. The platform provides tools to configure and fine-tune your model for optimal performance.

4. **API Key:** Obtain your Roboflow API key. You can find this key in your Roboflow account settings.

5. **Run the Code:** In this repository, you will find code that uses the Roboflow API to load the pre-trained model. Make sure to input your API key in the code, and you can then run it to make predictions.
6. I have also written the code if you want to train your model on local machine and not on roboflow. 

## Screenshots

Below are some screenshots captured during the model training process:

- [dataset details]

<img width="722" alt="image" src="https://github.com/shivam-gupta12/Plastic-Detection-In-Rivers/assets/109721120/901c9101-4e1a-4f60-9c29-6b51f83b977c">

- [model training]

<img width="1097" alt="image" src="https://github.com/shivam-gupta12/Plastic-Detection-In-Rivers/assets/109721120/257b7a76-8d4c-46df-9501-716dbbd4e202">

- [results after training]

<img width="1097" alt="image" src="https://github.com/shivam-gupta12/Plastic-Detection-In-Rivers/assets/109721120/cdecd3fe-f478-4d79-b482-795d5461ce24">

- [predictions]

<img width="1097" alt="image" src="https://github.com/shivam-gupta12/Plastic-Detection-In-Rivers/assets/109721120/bfe2cbe4-fc32-4f42-ad0b-c6715a0d7551">

- [training graphs]

<img width="722" alt="image" src="https://github.com/shivam-gupta12/Plastic-Detection-In-Rivers/assets/109721120/67afc012-712f-4e56-9336-c9d52a3853ae">

<img width="1097" alt="image" src="https://github.com/shivam-gupta12/Plastic-Detection-In-Rivers/assets/109721120/3422faf6-6315-4299-b185-bf6aee9c7163">

- [Annotations - defining ground truths]

<img width="1280" alt="image" src="https://github.com/shivam-gupta12/Plastic-Detection-In-Rivers/assets/109721120/6d844f6b-9f5e-4e31-942c-0948c7a509e8">


## Making Predictions

After training the model, you can use it to make predictions on new images or video frames. The code in this repository demonstrates how to load the pre-trained model using the Roboflow API and apply it to detect plastic waste in river images.
one of the predictions that i did on vscode is there in repository as prediction.jpg. Also , the screenshots include testing of the model.

## Conclusion

Plastic pollution in rivers is a pressing environmental concern, and the development of automated detection models can aid in mitigating this issue. This project showcases the process of annotating a dataset, training a plastic detection model using Roboflow, and making predictions using the pre-trained model. By following the provided steps, you can contribute to the effort to keep rivers plastic-free. Screenshots show the results of Mean Average Precision , Precision and Recall
