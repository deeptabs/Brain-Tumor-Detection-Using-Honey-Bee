# Brain-Tumor-Detection-Using-Honey-Bee
Detect the tumor using morphological operation and honey bee algorithm with Fuzzy C-means (FCM) clustering. 

Source code execution:

UI has a button on click of which an image can be uploaded, here the user uploads an image, which is either in jpg, bmp, png or tiff. Python library is used to convert image to 2 dimensional matrix which can be fed to our algorithms.

Preprocessing Button

The image may have noise, disturbances. Therefore we preprocess the image by
removing noise, converting it to grayscale, smoothing the image. We do this using Bilateral filter.
Output: Enhanced image

Processing Button

FCM : Here the enhanced image which has been Pre-processed, is fed into Fuzzy C means algorithm first.
ABC:  Then the optimisation technique of Artificial Bee algorithm is applied to the output of FCM.
Output: Image with detection of high density clusters, predicting them to be tumor.

Post-Processing Button

The image after undergoing processing, is fed to feature extraction algorithm. Hence,
here Watershed algorithm is applied, which colours the image with different colour in different density, thus providing the possible location of brain tumor.
Output: Image with Brain tumor detected.
