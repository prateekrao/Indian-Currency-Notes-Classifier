# Indian-Currency-Notes-Classifier

Deep Learning Model to recognize and classify Indian Currency in notes form.

  ## **Introduction**

  The model is trained to recognize 7 classes of Indian Currency in the form of notes.
  The denominations it can identify is:
   *  Rs.10
   *  Rs.20
   *  Rs.50
   *  Rs.100
   *  Rs.200
   *  Rs.500
   *  Rs.2000

  ## **Dataset**

   The dataset is imported from Kaggle, and contains several images for each of the training and validation classes in .jpg format.
   However, the images are of different resolutions, so all the images in the data have been scaled down to 190 x 190 pixels.
    
   Dataset used: https://www.kaggle.com/vishalmane109/indian-currency-note-images-dataset-2020
   
   ## **Model Features**
   
   This is a vanilla Convolutional Neural Network
