# Analysis of Cytology Pap Smear Images Using Two-Stage CNNs

## Overview
Cervical cancer is a type of cancer that occurs in the
cervix. It is caused by the abnormal growth of cells in the cervix
and is often caused by the human papillomavirus. Symptoms
can include abnormal vaginal bleeding, and pelvic pain, among
others. It is usually diagnosed with a pelvic exam, biopsy, and
Papanicolaou or Pap test. Generally, during the test, a small
sample of cells is taken from the cervix and examined under a
microscope to look for any abnormal cells. The test is usually
done during a pelvic exam and can be done in a doctor’s office or
clinic, which can cause human errors to exist and lead to a deficit
of service or misdiagnosis for patients. Especially, in Ecuador,
cervix cancer is the second with the most prominent incidence
and mortality. One of the obstacles in Latin America to improve
the number of cervix cancer screens is the amount of time needed
to give results. This paper proposes a pre-trained artificial neural
network and a much larger database than its paper base, this
will allow us to obtain better results and a network with more
accurate predictions when throwing where malignant cells could
be located that could lead to cervical cancer. The process to carry
it out is similar to its original process, where the analysis of the
Papanicolaou tests is carried out in two stages. The first focused
on finding the coordinates of the anomalous cells observed within
each of the images of our dataset and the second, specializing in
being able to obtain an image with a much higher resolution for
each of these coordinates, thus obtaining an improvement and
being able to give a much more reliable diagnosis for each of the
patients.

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
The following drive link contain the classification trained model and the datasets used for training the two stages. 

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

