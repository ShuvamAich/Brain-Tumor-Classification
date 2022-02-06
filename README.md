# Brain-Tumor-Classification


# Task 1: Introduction

In this project, I have created a Deep Learning model using the Supervised Learning Approach i.e. we have used labelled data. By the term "labelled data", we mean that our data has already been classified into x-rays with and without tumors, where the x-rays with tumors has further been classified into glioma, meningioma and pituitary tumor. 

When the model is over trained, the nodes have end up "memorizing" the input data. This results in a high variance, i.e. a significant difference between the error of the train set and the test set. 
Overfitting happens when a model learns the detail and noise in the training data to the extent that it negatively impacts the performance of the model on new data. The model begins to treat random fluctuations and noise as concepts.
To avoid overfitting:
Train a bigger neural network architecture and get more data.
Try out regularization.

# Task 2: Clone Dataset and Import Libraries

We clone the dataset from github. It consists of more than 3000 images. Then we import the necessary libraries required for the project.

# Task 3: Create Directory to store Training and Test Data

We make the following directories to store cropped images i.e. to crop out the little and unimportant portions of the background from the x-rays. 

# Task 4: Data Visualization

We are using the following code segment to iterate through our dataset and randomly displaying images to visualize the data.

# Task 5: Create a function to crop images

This function is used to crop the unimportant black portions in the background of the x-ray images as it is not necessary for training.

# Task 6: Save Preprocessed Data

The cropped images are then saved to the train and test directories which we created.
Here tqdm is used to show the progress bar as the files get copied to the destination directories.

# Task 7: Data Augmentation and Data Loader

In order to increase the size of the training data set we have the possibility to apply certain transformations to the existing training data. This artificial way of creating extra training images through different ways of processing is called image augmentation.

# Task 8: Creating the Model

Here, we are using transfer learning i.e. we are using a pretrained model called EfficientNet to train our model.

# Task 9: Model Training and Model Evaluation

I have trained the model upto 7 epochs  with 82 validation steps. The best model will be saved as model.h5. We get a training accuracy of 97.59% and our test accuracy reaches approximately 95%. The model is slightly overfitting.
We can overcome this by working with the larger dataset and also using various regularization techniques.

# Task 10: Prediction on Test Data

As you can see, our model works fine on the test data making most of the predictions correctly.

# Live blog post

https://shuvamaich.wixsite.com/myblogs/post/brain-tumor-classification

