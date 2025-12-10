# Vignette-Car-Vision

Vignette on identifying objects such as pedestrians, traffic lights, and other road-side objects using computer vision. This was a project for PSTAT197A.

## Contributors

Sanil Katula, Bahaar Ahuja, Shenyi Jiang, & Calder Glass

## Abstract
Self-driving cars need to be able to identify common entities on or alongside the road. The
dataset "Udacity Self-Driving Car" on Roboflow provided 15000 images of pedestrians,
cars, traffic lights, bikers, etc and labels containing the coordinates for those objects. The YOLOv7-PyTorch model classifies
the different potential roadside objects under 11 labels and assigns a probability that the object is of that given label.

## Repository Contents
The drafts folder contains the rough draft of the Jupyter Notebook used for the project. The data folder contains the general structure of the dataset when it's downloaded manually from Roboflow. The images and labels were not included because they would exceed GitHub's file limit. The scripts folder contains the final script/final draft of the Jupyter Notebook of our code.

## How to replicate computer vision on a different dataset
1.   Clone the YOLOv7 repository
2.   Load Pretrained Model
3.   Download Dataset
4.   Split test/train
5.   Sample Labeling on a image

## References for Further Learning
Learning Open CV 4 Computer Vision with Python 3: https://books.google.com/books/about/Learning_OpenCV_4_Computer_Vision_with_P.html?id=ef_RDwAAQBAJ&source=kp_book_description

Computer Vision: Algorithms and Applications, 2nd Edition: https://szeliski.org/Book/

Computer Vision, From 3D Perception to 3D Reconstruction and Beyond: D. A. Forsyth and J. Ponce. Computer Vision: A Modern Approach (2nd Edition). Prentice Hall, 2011.

## Dataset - Udacity Self-Driving Car on Roboflow
https://public.roboflow.com/object-detection/self-driving-car

