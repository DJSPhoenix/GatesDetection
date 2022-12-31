# GatesDetection
## Introduction
- This project aims to train YOLO v3 for gate detection on google colab  which can identify any gate from the given robust data set of multiple number of gates
- The software stacks implemented in this project are google colab,Python and google drive used as an external storage device. 
- We also made use of OpenCV  and CNN for the gate detection part.
- The Goal of this project is to give information to the microprocessor by identifying the gates (a specific area through which drone has to pass) in front of it by us ing the camera feed as its input source.

## Installations
### Pre-Requisites :
- Python equipped with matplotlib libraries.
- A  google drive which acts as an external storage ,which contains all the test and training models 
- A labeled data set of gates
- _https://pjreddie.com/media/files/darkn..._  From here  we downloaded pre-trained weights for the convolutional layers 

## Preparing the data set and uploading it in the drive
So, first, download the images from Google and label them with https://github.com/developer0hye/Yolo Label this labelling tool. After labelling and renaming all of the photos in the data set, compress it in a zip file and upload it to your drive. The data set should include jpg files, which are photos of the gates, as well as.txt files containing the coordinates of the given label and a class file that identifies the label. Rename the class.txt file and include the Python files that train text and label the data set.
### Google colab
Mount your drive on Google Colab. Execute your Python files in it, grant darknet executable permissions, and use the GPU feature of Google Colab to train the given data set using the knowledge of a pretrained data set and a convoluted neural network. After that, the drive will now have trained weights, indicating the end of Yolo's training.
### Code explained in detail
- **Creating_files-data-and-name.py** : - The purpose of this code is to compile the name and data of the labels of the data set into a single text file called labelled data.
- **Creating_train-and-text-files.py**:-The goal of this code is to create full paths by scanning a list of paths and extracting 15% of them to save in the folders train.txt and test.txt. This code will generate two files, train.txt and test.txt, containing full paths to images.
- **Test.py**:- This code is the project's heart. It then tests and simulates the bot using an open cv source using the data from the pretrained weights that were applied during training. As a result of the code, the machine will be able to easily label the unlabeled image using a webcam.
## Purpose of this project
Our ultimate goal is to build an autonomous racing drone, and in order for that to happen, the drone must automatically detect and pass through the gates in order to stay on the correct trajectory. This is the first step of the project, identifying the gates. The simulations and tests went well, and video recordings will be attached to this document.



https://user-images.githubusercontent.com/93365067/210038002-582968df-21e2-4dee-a818-321d7233216d.mp4

Dataset and trained weights model.
https://bit.ly/Gate_Detection
