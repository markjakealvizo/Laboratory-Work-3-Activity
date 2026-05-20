# CSC-Laboratory Work 3_Custom Image Classification

Google Collab link:
https://colab.research.google.com/drive/1eumyqQsP8wV1t8bFX-rUx6cakv368ei1?usp=sharing
Google Drive Saved Model: https://drive.google.com/drive/folders/1Am2FPa8AqxdIcQq3OxY3ZPKpgPmmenD4?usp=drive_link

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







# Guide Questions (Student Explanation & Reflection)

### Visualization & Overfitting
1. What signs indicated overfitting in your first model?
   
**Answer:** Overfitting was indicated because training accuracy became very high and training loss kept decreasing, while validation accuracy stopped improving and validation loss started increasing, showing the model memorized the training data but did not generalize well to new data.

2. How did data augmentation affect validation accuracy?

**Answer:** Data augmentation improved validation accuracy by helping the model generalize better and reducing overfitting on the training data.

### Model Improvement
 3. What is the purpose of dropout layers?

**Answer:** The purpose of dropout layers is to prevent overfitting by randomly turning off some neurons during training so the model learns more general features.

4. Why does data augmentation improve generalization?

**Answer:** Data augmentation improves generalization because it creates varied versions of the training images, helping the model learn more robust features instead of memorizing the original data.

### Performance Comparison
5. Compare accuracy before and after improvements.

**Answer:** Before improvements, training accuracy reached about 100% while validation accuracy stayed around 75–77%, showing overfitting, whereas after improvements training accuracy decreased to about 60% and validation accuracy stayed close to it (~55%), indicating better generalization with a smaller gap between them.

6. Which technique contributed most to improvement?

**Answer:** Data augmentation contributed most to the improvement because it increased data variation and helped the model generalize better, reducing overfitting.

### Deployment & Application

7. Why is saving the model important?

**Answer:** Saving the model is important because it allows you to reuse the trained model later for predictions without training it again.

8. How can this model be deployed in a real-world system?

**Answer:** This model can be deployed in a real-world system by exporting the trained model and integrating it into an application or server (e.g., web app, mobile app, or API) that takes new input data, runs predictions, and provides results to users in real time.
