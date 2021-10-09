# Classifier
This repository contains the following:

Jupyter Notebook:
- Cat Dog Classifier: this notebook contains 3 parts as follows:
  - Data preparation: 
    1. The cat and dog images are first downloaded from this link: https://www.kaggle.com/arpitjain007/dog-vs-cat-fastai
    2. After which the images were read using opencv python in order to convert them into arrays
    3. This completed arrays are then saved into .npy files so they may be accessed later
  - Model Training:
    1. The first step in this section is to set up the convolutional neural network architecture by indicating the number of layers, including convolutional, maxpooling and dense layers. Appropriate activation functions are also chosen for each of these layers
    2. The model is then fitted against the training data which we stored in arrays in the previous section
    3. The model is saved as a json file in order for us to use to predict other datasets in the future (or next section)
  - Model Testing:
    1. We access another set of images that was not previously used to train the model and convert them into arrays and labels
    2. This test set is then evaluated using the model that was trained in the previous section. 
    
The model achieved 75.75% accuracy on the test set compared to the 94.10% it scores for the training set that it was trained on.
