# GatesDetection
Introduction
This project aims to train YOLO v3 for gate detection on google colab utilizing the free GPU resources which can identify any gate from the given robust data set of multiple number of gates
The software stacks implemented in this project are google colab,Python and google drive used as an external storage device. We also made use of OpenCV  and CNN for the gate detection part.
The Goal of this project is to give intel to the microprocessor by identifying the gates( a specific area through which drone has to pass) in front of it by using the camera feed as its input source.

Installations
Pre-Requisites :
Python equipped with matplotlib libraries.
A  google drive which acts as an external storage ,which contains all the test and training models 
A labeled data set of gates
https://pjreddie.com/media/files/darkn...  From here  we downloaded pre-trained weights for the convolutional layers 

Preparing the data set and uploading it in the drive
So first download the images from google and label it using https://github.com/developer0hye/Yolo_Label this labeling tool after labeling and renaming all the photos in the data set compress it in a zip file and upload it on your drive .The data set should contain jpg files i.e photos of the gates and .txt files which contains the coordinates of the given label and a class file which identifies the label.rename the class.txt along with this add the python files which trains text and labels the data set
Google colab
Mount your drive on google colab execute your python files in it give darknet executable permissions and use the GPU feature of google colab and train the given data set using the knowledge of pretrained data set and convoluted neural network after this the drive will contain trained weights which showcases the end of training of yolo
Code explained in detail
Creating_files-data-and-name.py : - This codes’s purpose is to compile the name and the data of the labels of the data set into one single text file known as labelled_data
Creating_train-and-text-files.py:- This code’s purpose is to set up full paths by scanning list of paths and extracting 15% of paths to save into folders train.txt and text.txt  The result of this code will create 2 files train.txt and test.txt with full paths to images
Test.py:- This code is the soul of the project . It uses the data of the pretrained weights which have been applied while training the bot and finally tests it and simulates it using an open cv source. The result of the code will be that the machine will be able to label the unlabeled picture easily using webcam
xPurpose of this project
Our end goal is to create an autonomous racing drone and for that to happen the drone should automatically detect the gates and pass through it  so as to stay on the correct trajectory what we did is the first step of the project which is identifying the gates .The simulations and the tests were successful and the video recordings will be attached with this document.



https://user-images.githubusercontent.com/93365067/210038002-582968df-21e2-4dee-a818-321d7233216d.mp4

Dataset and trained weights model.
https://drive.google.com/drive/folders/1J0DSgiO9jisL7jjlKhxI50574_-ytOfn?usp=sharing
