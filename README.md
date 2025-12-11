# Vignette-Car-Vision

Vignette on identifying objects such as pedestrians, traffic lights, and other road-side objects using computer vision. This was a project for PSTAT197A.

## Contributors

Sanil Katula, Bahaar Ahuja, Shenyi Jiang, & Calder Glass

## Abstract
Self-driving cars need to be able to identify common entities on or alongside the road. The
dataset "Udacity Self-Driving Car" on Roboflow provided 15000 images of pedestrians,
cars, traffic lights, bikers, etc and labels containing the coordinates for those objects. The YOLOv7-PyTorch model classifies
the different potential roadside objects under 11 labels and assigns a probability that the object is of that given label.

## Why use YOLOv7?

The YOLOv7 model was chosen as it's better at precision of small objects such as traffic lights and pedestrians, when the objects are either a long distance away or captured with a low-resolution camera. The model is also more robust when dealing with day/night lighting, weather, and information-dense images. Additionally, implementing it via PyTorch allowed for the model to be easier to fine-tune to the given traffic dataset in this vignette.

## Repository Contents

* `data/` - Contains the general structure of the dataset when it's downloaded manually from Roboflow. The images and labels were not included because they would exceed GitHub's file limit.
  * `export/`
    * `images/` - Contains the images of road-side objects that the model is trained on.
    * `labels/` - Contains the labels for each given image, where the integer is represents the given classification of an object in that image.
  * `README.dataset.txt` - Gives a brief overview of the dataset and its differences from the original version on GitHub.
  * `README.roboflow.txt` - Mentions that the dataset was exported from Roboflow, the number of images in the dataset, and the preprocessing applied to the images.
  * `data.yaml` - Denotes that training and validation subfolders of the images folder and the 11 classes of objects that can appear in the images.

* `draft/` - Contains the rough draft of the Jupyter Notebook used for the project.
  * `197_car_vision.ipynb` - Rough draft of the Jupyter Notebook of the vignette.
  * `Jupyter Notebook -- generated with runcell.pdf` - Pdf render of the rough draft of the vignette.

* `scripts/` - Contains the final script/final draft of the Jupyter Notebook of our code.
  * `197_car_vision_notebook_final_annotations.ipynb` - Final draft/script with some line annotations of the Jupyter Notebook used for the vignette.
  * `197_car_vision_final.pdf` - Pdf form of the final draft of the vignette.


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

