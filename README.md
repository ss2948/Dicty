# Dicty
(c) 2022 Siddhartha Saha

We develop a machine learning pipeline for learning spatio-temporal features and performing the task of classification in video datasets of actin dynamics exhibited by Dictyostelium cells in various environments. The video dataset primarily consists of cell motion in 4 different environments: Cells moving on 1)flat surface with no electric field, 2) ridged surface with no electric field, 3) flat surface in the presence of electric field and 4) ridged surface in the presence of electric field. We present three different data analysis pipelines that we have developed, namely 1) sparse coding/ dictionary learning, 2) wavelet analysis/ scattering transform and 3) optical flow. Both Dictionary learning/ sparse coding and Wavelets/ Scattering transform lead to a latent lower dimensional representation of the video frames in our dataset and these feature vectors are used as input to a classifier (SVM) to perform classification. To track motion of the cells we use Optical flow which leads to the construction of velocity based features - these feature vectors are then used for classification using a classifier (SVM)

# Installation

 For the sparse coding based analysis, we use various in-built tools from scikit-learn (https://scikit-learn.org/stable/). For the analysis based on scattering transform, we use a package named Kymatio (https://www.kymat.io/) along with scikit-learn. For the optical flow based analysis we use some in-built tools from OpenCV (https://opencv.org/). The scripts have been tested with python 3.8.5.
 
 Required Modules:
 - numpy
 - scipy
 - sklearn
 - seaborn
 - pandas
 - Kymatio
 - OpenCV
 - Matplotlib

# Overview

Here is an overview of the files included in the repository:

1. ```dictionary_sparsecoding-upload.ipynb```: Jupyter notebook file that contains the analysis done using dictionary learning/ sparse coding

2. ```wavelets_scatteringtransform -upload.ipynb```: Jupyter notebook file that contains the analysis done using wavelets/ scattering transform 

3. ```optflow-upload.ipynb```: Jupyter notebook file that contains the analysis done using wavelets/ scattering transform 

We upload the data, then perform the analysis and show the classification results obtained via each pipeline in each of the notebooks.
