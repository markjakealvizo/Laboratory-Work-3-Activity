# Laboratory Work 3_Custom Image Classification

Google Collab link:
https://colab.research.google.com/drive/1eumyqQsP8wV1t8bFX-rUx6cakv368ei1?usp=sharing

# Guide Questions (Student Reflection & Explanation)
## Students must answer the following:

### 1. Dataset Preparation

○ How did you organize your dataset in Google Drive?

**Answer:** In mydrive, ImageDataset folder under ImageDataset folder are the 20 class of trees, each class have a folder and the minimum of 250 images inside of each class.

○ Why is folder structure important for TensorFlow image loading?

**Answer:** The folder structure is important because TensorFlow uses the subfolder names as class labels.


### 2. Model Training

○ What is the role of convolutional layers in image classification?

**Answer:** The convolutional layers in a CNN are like the model’s “eyes” for images. Their role is to detect patterns and features from the image.

○ Why do we split data into training and validation sets?

**Answer:** We split data into training and validation sets to teach the model and check if it’s learning correctly.


### 3. Performance Analysis

○ What accuracy did your model achieve?

**Answer:** The model achieved around 75–76% accuracy on the validation set, with similar accuracy on the training set.

○ How did the number of images affect the model’s performance?

**Answer:** With a limited number of images, the model learned the training data well but struggled on new images, so validation accuracy was lower. More images would improve its performance.

### 4. Critical Thinking

○ What challenges did you encounter while using your own dataset?

**Answer:** The main challenges were overfitting and limited data. The model learned the training images very well (high training accuracy) but performed 
less accurately on validation images (~75–78%), showing it struggled to generalize to new images

○ How can data augmentation improve your model?

**Answer:** Data augmentation can improve the model by creating more varied training images, which helps reduce overfitting.


### 5. Application
○ Suggest a real-world application for your trained model.

**Answer:** A mobile app that identifies trees or plants from a photo, helping farmers, gardeners, or students quickly recognize plant species and 
provide care instructions or information about them.


○ How can this system be integrated into a mobile or web application?

**Answer:** The trained model can be integrated into a mobile or web app by letting users upload or take a photo, preprocessing it, running it through the model, and displaying the predicted plant species.


