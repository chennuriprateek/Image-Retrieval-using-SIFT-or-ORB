# Image-Retrieval-using-SIFT-or-ORB
Using SIFT or ORB keypoints from images, retrieve the corresponding images based on the reference image.  

## Problem Statement
1. Capture 6 images of 10 different scenes of your choice using a hand-held camera like cellphone's camera without using a tripod. Resize the images so that max(row,column)<=1024 while keeping the aspect ratio of the image intact.  
2. Make sure there are no moving objects present in the scene and there should be some angle variation between the images.  
3. Using SIFT and ORB feature matching, given a query image retrieve the top-5 similar images from the pool of remaining 59 images. (built-in functions for feature extraction is allowed but for matching are not allowed)  
4. Use sum of euclidean distances between top-k matches of the features of a pair of images as the ranking criteria. (value of k should be decided by you but it should be more than 10.)  
5. To obtain the accuracy consider each image in your dataset as a query once and check how many of the other 5 images of the same scene you are able to retrieve among the top-5 images from the step 3. For e.g.- for a query image if you are able to retrieve 4 out of 5 images of the same scene, then it is 80% accuracy. Do this for all the images present in your dataset.  
6. Report the average image retrieval accuracy with a value of k of your choice for both SIFT and ORB features.  
7.  Plot a graph of the average retrieval accuracy for the values of k = 1,5,10,20,40,60,80 and max matches.  
Note: The assignment will not be graded solely based on the final retrieval accuracy. The complexity of the dataset and the complete implementation will be considered for the evaluation of the assignment.  

THE CODE IS PRESENT IN 'image_retrieval_code.ipynb'   

the data used for assignment is available in 3 folders:  
1. 256 size grayscale images in 256_imgs folder  
2. 512 size grayscale images in 512_imgs folder  
3. 1024 size grayscale images in 1024_imgs folder  

The images collected is present in the 'dataset' folder  

The results are available in the 'results' folder  

STEPS TO RUN THE CODE:  
open the file containing the code and move to the "RUN THE CODE HERE" location.  
Give the appropriate inputs as described in the comments at the corresponding functions.  
