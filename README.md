# Read This First!
`Face Mask Detector with gif.ipynb` file contain a short gif that demonstrates the results. If it's doesn't open you can:
1. Copy the link and paste it on this site https://nbviewer.jupyter.org/ and it will open it.
2. Open `Face Mask Detector.ipynb` file which is without the gif therefore is lighter and supposed to open just fine!

I added a video in a separate file as well, for demonstrates the results.

The Xception model's Weights are too heavy so I uploaded the MobileNet model's Weights which received almost the same results.



# Face-Mask-Detector


Masks play a crucial role in protecting the health of individuals against respiratory diseases, as is one of the few precautions available for COVID-19 in the absence of immunization.
In this notebook, I'm going to build a real-time detector (via personal laptop webcam) which will be classified whether the person is wearing a mask or not.

This notebook is divided into two parts:

Part 1: Import, preprocess and build a few models using Keras library.\
Part 2: Chose the best model and test the result in LIVE via webcam, using OpenCV library.

The idea to do this project I took from [Kaggle](https://www.kaggle.com/search?q=mask+in%3Adatasets) and from [this guy](https://data-flair.training/blogs/face-mask-detection-with-python/).

## Data
The data contain 13,432 images of people with and without a mask. this dataset is balanced - 6,703 with mask and 6,729 without a mask.\
The data already divided into 3 separate datasets: train, validation and test.

## Data sources:
I created the datasets (train, test and validation) by combining data from a few data sources:

https://data-flair.training/blogs/download-face-mask-data/ - train and test setes.  \
https://www.kaggle.com/dhruvmak/face-mask-detection - validation set.  \
https://www.kaggle.com/prithwirajmitra/covid-face-mask-detection-dataset - train, test and validation. 

In this particular dataset, most of the images are have been processed, so I manually took only the original and non-processed images (the dataset is sorted so it's the images at the beginning): https://www.kaggle.com/ashishjangra27/face-mask-12k-images-dataset - train, test and validation.
