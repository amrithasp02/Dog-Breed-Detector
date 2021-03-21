# Dog-Breed-Detector
Title: Deep CNN model trained to predict dog breeds based on an image

Team Members: Amritha S Pallavoor, Ananya Shashishekar and Abhinav Vasireddy

This is a project created for PES I/O course.

Dataset used: https://www.kaggle.com/c/dog-breed-identification/data
- The dataset consists of 120 breeds of dogs with more than 10,000 images for training.
- It also has a test dataset folder with images
- CSV file with image id and breed name is also provided.
-
Model Architecture:
- This model was built using the InceptionV3 model from Keras library. 
- We loaded the pretrained weights of the Inception model by downloading the data to do transfer learning.
- Upon this, we added a global spatial average pooling layer
- Added a fully-connected layer and a logistic layer with 20 classes only
- The model is trained and compiled using Adam optimizer for 10 epochs with categorical_crossentropy.
- Results after training:
Epoch 10/10
175/175 - 48s - loss: 0.0890 - accuracy: 0.9668 - val_loss: 0.2331 - val_accuracy: 0.9222

The model is saved as 'dogbreed-model1.h5', which can be accessed using the below google drive link:
https://drive.google.com/file/d/1Ftc7fjGznYeksYx56jOfw20dVKXAeFN7/view?usp=sharing

The below video demonstrates the testing part of this model:
https://drive.google.com/file/d/1AP_j216bd9pFMIjjfQjk_Dz5sGk-HwUh/view?usp=sharing
