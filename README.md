# AutoML-Modeling-Report
This dataset would eventually be used to build a product that helps doctors quickly identify cases of pneumonia in children. Remember that the goals of this product are to:

help flag serious cases,
quickly identify healthy cases,
and, generally, act as a diagnostic aid for doctors.
In this project, we are going to take the next step and build the classification model that would serve as the backbone of this product. (Don't worry, there's no coding involved!) For this task, we will use Google AutoML, an automated machine learning tool that will allow us to build the model and host it in the cloud. In order to appreciate how training data impact models, we will build models with 4 variants of the dataset. This project is designed to test your ability to

build a model using Google's AutoML Vision platform, and
understand how properties of data impact performance of models.
The Data
We'll be using the same Kaggle chest x-ray dataset that we used in the previous project, except here, we'll skip the step of using Figure Eight's platform to label the data, and just use the original labels supplied with the data on Kaggle.

The Four Parts of the Project
We will train four different models using four variants of the pneumonia dataset. Recall that the dataset contains childrens' chest x-ray images, and that they are classified into two classes, "normal" and "pneumonia". The following sections describe the steps you must take to create each model.

1. Create a binary classifier to detect pneumonia using chest x-rays
We'll start by training a model simply using 100 images from the “normal” class and 100 images from the “pneumonia” class. You will be asked to evaluate the following:

Train/test split: How much data is used for training and how much is used for testing?
Confusion matrix: What do each of the cells in the confusion matrix describe?
Precision & recall: What do these measure and how are they calculated?
2. Create an unbalanced binary classifier
Next, use 100 images from the “normal” class and add 200 "pneumonia" class images for a total of 300 images in the “pneumonia” class. The model will be trained on very unbalanced classes; this will show you what happens when the number of images in different classes is very different. You will be asked to evaluate:

Confusion matrix: What does the confusion matrix tell you about unbalanced data?
Precision & recall: How are precision and recall affected?
Unbalanced classes: How do unbalanced classes impact a machine learning model?
3. Create a binary classifier with dirty data
In this iteration, start with the original dataset of 100 "normal" and 100 "pneumonia" images. Then switch the labels of 30 images in each class. After you've done this, 30% of the data are mislabeled. You will be asked to evaluate:

Confusion matrix: How is the confusion matrix affected?
Precision & recall: How are precision and recall affected?
Dirty data: How do dirty data impact the model?
4. Create a three-class model with the classes “normal”, “bacterial pneumonia”, and “viral pneumonia”
For the final model, note that the "pneumonia" images actually have two different classes: "bacterial" pneumonia and "viral" pneumonia. These labels are indicated in the image filenames. For this model, add 100 "normal" images, 100 "bacterial pneumonia" images, and 100 "viral pneumonia" images (for a total of 3 classes). You will be asked to evaluate:

Confusion matrix: What does the 3-class confusion matrix look like?
Precision & recall: What are the model's precision and recall? How are these measures calculated?
More data: Can you continue to add data to each class (while keeping the data balanced) and get the model to 85% precision and recall? How many data did you end up using?
After you have trained each model, you will answer questions about it in the AutoML Modeling Report, which you can find linked below. You may want to download this form and have it on hand as you go through the model building steps so that you can answer questions and take screenshots as you go.
