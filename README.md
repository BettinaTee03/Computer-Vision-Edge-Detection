# Computer-Vision-Edge-Detection
This is our group project for Ewha Womans University, Computer Vision course 39154

**This project is completed by:**   
Qin Tong Bettina Tee, Daso Jung, Yan Renyu  

# Project description
The project aim is to develop an edge detection method to produce a predicted boundary score map given an image. We have developed an approach which optimises the image preprocessing steps before applying the Sobel operator to obtain the predicted boundary score map.

The brief outline of our method is as follows:
1. Feature extraction 
2. Target extraction (optimal parameters for the preprocessing steps)
3. Parameter prediction (using a random forest classifier)
4. Image preprocessing (using Gaussian Blurring and Contrast Enhancement)
5. Edge Detection (using Sobel Operator)

# Files in this respository
## Code files:  
1. predict.ipynb: This file details the approach we have taken to create develop our edge detection algorithm
2. evaluate_train.ipynb: This file presents the evaluation results for our train dataset
3. live_demo.ipynb: This file was used to demonstrate the prediction process during our presentation
4. testing_other_methods.ipynb: This file presents the empirical reasoning as to why we selected sobel operator. It also demonstrates how our preprocessing steps have improved the accuracy of the model
## Result files: 
1. predictions_train.npy: This file is the resultant predicted boundary score maps for the train dataset.
2. predictions.npy: This file is the resultant predicted boundary score maps for the test dataset.
## Data folders:
1. project_data: contains train folder (train images and ground truth boundaries), and test folder (test images)
2. cv_project_tools: tools used in the evaluation code
3. saved_variables: intermediate variables used in predict.ipynb
4. method_experiment_results: results from testing_other_methods.ipynb file, namely the results on 10 images from sobel, laplacian and prewitt without preprocessing the images.  
