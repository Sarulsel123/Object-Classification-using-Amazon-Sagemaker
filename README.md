# Object-Classification-using-Amazon-Sagemaker

# What is Amazon Sagemaker? 
AWS SageMaker simplifies ML modeling into three steps: preparation, training and deployment.
Amazon SageMaker creates a fully managed ML instance in Amazon Elastic Compute Cloud (EC2). 
It supports the open source Jupyter Notebook web application that enables developers to share live code. 

# The Amazon SageMaker Object Detection - MXNet 
The algorithm detects and classifies objects in images using a single deep neural network. 
It is a supervised learning algorithm that takes images as input and identifies all instances of objects within the image scene. 
The object is categorized into one of the classes in a specified collection with a confidence score that it belongs to the class.

# Input/Output Interface for the Object Detection Algorithm

The SageMaker Object Detection algorithm supports both RecordIO (application/x-recordio) and image (image/png, image/jpeg, and application/x-image) 
content types for training in file mode and supports RecordIO (application/x-recordio) for training in pipe mode. 
However you can also train in pipe mode using the image files (image/png, image/jpeg, and application/x-image), 
without creating RecordIO files, by using the augmented manifest format. 

# Dataset
'http://www.robots.ox.ac.uk/~vgg/data/pets/data/images.tar.gz',
'http://www.robots.ox.ac.uk/~vgg/data/pets/data/annotations.tar.gz'

# Lets have a detailed step by step on how to perform object classification using Amazon Sagemaker 
Task 1: Create Notebook Instance
Introduction the Sagemaker
Creating a Notebook instance

Task 2: Annotations
Downloading and extracting the IIIT-Oxford Pets Dataset
Extracting the annotations
Creating a training and a validation set

Task 3: Visualize the Data
A quick look at some of the images and their corresponding bounding boxes

Task 4: Training Image for the Algorithm and Sagemaker Setup
Getting the Sagemaker execution role
Getting reference to the object detection training image

Task 5: Prepare Data for Sagemaker
Preparing data for object detector with the right folder structure and annotation files

Task 6: Uploading Data to S3
Creating an S3 bucket
Uploading the data to the bucket

Task 7: Sagemaker Estimator
Creating an Estimator

Task 8: Hyperparameters
Setting up the hyperparameters for the object detector

Task 9: Data Channels and Model Training
Creating the S3 Input data channels
Training the Model

Task 10: Deploy Model
Deploying the model

Task 11: Inference and Deleting the Endpoint
Using the deployed model for inference
Deleting the deployed endpoint
