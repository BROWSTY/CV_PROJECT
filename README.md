# Analysis of Cytology Pap Smear Images Using Two-Stage CNNs

## Overview
This project proposes a pre-trained artificial neural network and a much larger database than its paper base, this
will allow us to obtain better results and a network with more accurate predictions when throwing where malignant cells could
be located that could lead to cervical cancer.

## Requirements
- pytorch13+CUDA (the version depends on your CUDA version.)
- tensoflow 2.9.2
- keras
- opencv 4.6.6
- matplotlib 
- tqdm

Make sure that other common libraries such as numpy works correctly with the other library versions.

## Dataset
The following drive link contain the classification trained model and the datasets used for training the two stages. 

**Drive link:**  https://drive.google.com/drive/folders/1fz9-srsO7EBUKztheth8f1W_g1DAySB_?usp=sharing

--- Content --- 

* DB_4
   Isolated cell database. Images corresponding to liquid-based Pap smears.
   Database classified into four categories:
  
  1 -> High squamous intra-epithelial lesion
  2 -> Low squamous intra-epithelial lesion
  3 -> Negative for intra-epithelial malignancy
  4 -> Squamous cell carcinoma

With a total of 4000 training images and 800 images for validation.

**Important:** The detection trained model is not provided because it not takes more than five minutes to train.

