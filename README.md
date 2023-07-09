# Synthetic Image Generation

This repository contains code for synthetic image generation using various techniques and libraries. The code is written in Python and utilizes libraries such as OpenCV, Matplotlib, and Albumentations. The purpose of this code is to generate synthetic images by combining objects with different backgrounds and performing data augmentation.

## Table of Contents

- [Imports](#imports)
- [Uploading Files from Google Drive](#uploading-files-from-google-drive)
- [Data Augmentation](#data-augmentation)
- [Append Objects to Background](#append-objects-to-background)
- [Web Scraping](#web-scraping)
- [Bounding Box Calculation](#bounding-box-calculation)
- [Path to Files](#path-to-files)
- [Usage](#usage)
- [License](#license)

## Imports <a name="imports"></a>

The following libraries are imported in the code:

- cv2: OpenCV library for computer vision tasks
- matplotlib.pyplot: Library for plotting and visualization
- os: Library for interacting with the operating system
- numpy: Library for numerical operations
- albumentations: Library for image augmentation techniques
- time: Library for measuring time
- tqdm: Library for creating progress bars
- google.colab.drive: Library for mounting Google Drive
- re: Library for regular expressions
- PIL: Library for image processing
- keras.preprocessing.image: Library for image data generation
- random: Library for generating random values
- requests: Library for making HTTP requests
- io.BytesIO: Library for handling binary data
- bs4.BeautifulSoup: Library for web scraping
- urllib: Library for handling URLs
- string: Library for working with string operations

## Uploading Files from Google Drive <a name="uploading-files-from-google-drive"></a>

The code includes a function `drive.mount('/content/gdrive')` to mount Google Drive and upload files from it.

## Data Augmentation <a name="data-augmentation"></a>

The code includes a function `Data_Augmentation()` that performs data augmentation on images. It uses the `ImageDataGenerator` class from the Keras library to apply rotation, brightness, and zoom augmentation to the images.

## Append Objects to Background <a name="append-objects-to-background"></a>

The code includes a function `append_to_bg()` that appends objects to background images. It takes an object image and a background image, resizes and positions the object image randomly on the background image, and applies alpha blending to combine the images.

## Web Scraping <a name="web-scraping"></a>

The code includes a function `webscrape()` that performs web scraping to extract image URLs from a given URL. It uses the BeautifulSoup library to parse the HTML content and extract the image URLs.

## Bounding Box Calculation <a name="bounding-box-calculation"></a>

The code includes a function `BBox()` that calculates the bounding box coordinates of an image. It uses the OpenCV library to threshold the image and find the contours to determine the bounding box.

## Path to Files <a name="path-to-files"></a>

The code contains variables `PATH_real_pics` and `PATH_bg` that specify the paths to the real pictures and background images.

## Usage <a name="usage"></a>

1. Ensure that the required libraries are installed.
2. Run the code by executing the cells or running the script.
3. The code will perform synthetic image generation by combining objects with backgrounds, performing data augmentation, and saving the generated images.
4. The generated images will be saved in the "final_data" folder.
5. The generated images can be downloaded as a zip file by executing the command `!zip -r final_data.zip final_data/` and then downloading the zip file.
