# Analysis of Cytology Pap Smear Images Using Two-Stage CNNs

## Overview
This paper proposes a solution for detection of pap smear using a pre-trained artificial neural
network and a much larger database than its paper base, this
will allow us to obtain better results and a network with more
accurate predictions when throwing where malignant cells could
be located that could lead to cervical cancer. 

## Requirements
- keras
- matplotlib 
- tqdm

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

* DB_4
   Isolated cell database. Images corresponding to liquid-based Pap smears.
   Database classified into four categories:
  
  1. High squamous intra-epithelial lesion
  2. Low squamous intra-epithelial lesion
  3. Negative for intra-epithelial malignancy
  4. Squamous cell carcinoma

With a total of 4000 training images and 800 images for validation.
