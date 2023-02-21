# Deep Learning
For full presentation, click [here.](https://github.com/riwasabri/DeepLearning/blob/master/Deep%20Learning.key)

## Design

The goal of this project is to guess the artist of a given artworks by
leveraging images of artworks created by a variety of artists in terms of
style and technique.
The complete dataset consists of 5000+ artworks created by 11 different
artists.
Given the classes are imbalanced, I assessed performance by looking at
recall. The graph below shows class imbalance.

![picture alt](https://github.com/riwasabri/DeepLearning/blob/master/img1.png)


## Data

The data is gathered from Kaggle and consists of 8000+ rs, with one row corresponding
to one URL that StumpleUpon recommended to their users. Each URL in the dataset is
labeled as evergreen (1) or not (0) - this is the target.
Initial cleaning consisted of checking for , imputing null values where needed, renaming
columns for clarity.
Algorithm
Transfer Learning
* Tested out several transfer learning models:
  * VGG16
  * ResNet50
  * MobilnetV2
* Tuning
  * Tested out different top layers configurations, adding dropout to reduce overfitting
  * Tested out adjusting class_weights to assess effect on recall
  * Early stopping based on recall
* Image Augmentation
 * Performed image augmentation in order to reduce overfitting and increase data.
    Find examples below.
    ![picture alt](https://github.com/riwasabri/DeepLearning/blob/master/img2.png)

## Tools
* Google Colab
* OS for files manipulation
* Tensorflow Keras for modeling
* Scikit Learn for results analysis
* Matplotlib/Seaborn for Data visualization
