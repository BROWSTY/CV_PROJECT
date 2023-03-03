# Analysis of Cytology Pap Smear Images Using Two-Stage CNNs

## Overview
This paper proposes a solution for detection of pap smear using a pre-trained artificial neural
network and a much larger database than its paper base, this
will allow us to obtain better results and a network with more
accurate predictions when throwing where malignant cells could
be located that could lead to cervical cancer. 

## Requirements

keras

It is necessary to consider the following versions of these libraries

| Library  | Version |
| ---------| ------- |
| pytorch  | 1.10.1 |
| tensoflow| 2.9.2  |
| opencv   | 4.6.6  |

**Consideration:** pytorch==1.10.1  for CUDA 11.3 (the version depends on your CUDA version.)

Make sure that other common libraries such as numpy works correctly with the other library versions.

## Dataset
The following drive link contain both the classification and detection trained model and the datasets used for training the two stages. 

**Drive link:**  https://drive.google.com/drive/folders/1fz9-srsO7EBUKztheth8f1W_g1DAySB_?usp=sharing

--- Content --- 

* DB_3
   Database classified into two categories: 
   1. Cell images
   2. Test background images
With a total of 1600 training images and 400 images for validation.

* DB_4
   Isolated cell database. Images corresponding to liquid-based Pap smears.
   Database classified into four categories:
  
  1. High squamous intra-epithelial lesion
  2. Low squamous intra-epithelial lesion
  3. Negative for intra-epithelial malignancy
  4. Squamous cell carcinoma

With a total of 4000 training images and 800 images for validation.

## Usage
* The first stage model was trained using the FP_Cells.py file. In the file is commented the steps to train again other model or use the already trained model. Consider that the dataset that model uses is the DB_3.
* The second stage model was trained using the follow files:
  1. dataset.py: This file difene the paths where the images are retrieved. The dataset used in this file is the DB_4. 
  2. utils.py: This file generate the images and save the model. It is important to add the path where the user want to save the model and the images generated from the results. In our case, the folder outputs50 is the current path.
  3. model50.py: This file generate the ResNet50 architecture.
  4. train.py: This file calls the previous mentioned files for starting the training.
  5. inference.py: This file classify the images in the four different categories. The dataset used in this file is the DB_4.  
  6. Finally: to execute the train.py file it is required the number of epochs. Execute the following command
  
  $ python train.py --epochs "# of epochs"
