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
   
   The data has been scaled down to resolution of 190 x 190 for ease of training the CNN.
   
   ## **Model Features**
   
*  This is an implementation of a vanilla Convolutional Neural Network, which consists of 3 convolutional layers with 32, 64 and 64 filters each with size of (3,3)
   and pooling is done with MaxPooling.
*  Artificial Deep Neural Network is used for classification, and consists of a Dropout Layer as well as a layer for flattening the input given through the CNN.
*  It has two Hidden Layers with 32 and 64 neurons each, and an output layer with 8 neurons (representing the 8 classes) with activation softmax, to give the output 
   in the form of distribution of probabilities, which makes it easier to classify.
*  Activation functions of all the other Convolutional Layers and Hidden Layers is *relu*
*  Optimizer used is *adam*, loss function is *categorical crossentropy* 

  ## **Overfitting and Accuracy**
  
  Since this is a vanilla CNN, it's tough to get a great accuracy on the set. 
  Approach to overcome overfitting and increase accuracy:
  
    *  Using Dropout Layer to reset neurons
    *  Using Data Augmentation to increase size of dataset
    
##  **Training and Validation Accuracy**
The table gives validation and training accuracy at the end of training of the model.

Training Accuracy | Validation Accuracy 
------------------|--------------------
82.28 %           |             76.81 %
