# Comprehensive Image Processing Toolkit in MATLAB

In this project, I developed a comprehensive script using MATLAB and its Image Processing Toolbox to explore and implement a wide array of fundamental and advanced image processing techniques. The script serves as a hands-on demonstration of various methods, from basic manipulation to complex image segmentation and object detection.

## 📝 Overview

My script takes a single input image and applies a sequential series of processing operations to it. Each step is visualized in a separate figure window, allowing for a clear comparison of the effects of each technique. I've covered image enhancement, filtering, edge detection, morphological operations, and segmentation, culminating in the identification of objects within the image.

## ✨ Techniques I Implemented

I've organized the project to cover the following key areas of image processing:

#### 1\. Basic Image Handling

  * Loaded an image from a local directory using `imread`.
  * Displayed images using `imshow` and checked properties like size and class.
  * Converted RGB images to both grayscale and binary formats.

#### 2\. Geometric Transformations

  * **Resizing:** Changed image dimensions both by a scale factor and to specific pixel dimensions.
  * **Rotation:** Rotated the image by a specified angle (e.g., 45 degrees).
  * **Flipping:** Performed both horizontal and vertical flips of the image.

#### 3\. Image Enhancement

  * **Brightness Adjustment:** Increased and decreased image brightness by scalar multiplication.
  * **Contrast Adjustment:** Modified the image contrast using `imadjust`.

#### 4\. Filtering and Noise Removal

  * **Gaussian Blur:** Applied a Gaussian filter to smooth the image.
  * **Median Filtering:** Used a median filter, which is effective for salt-and-pepper noise.
  * **Sharpening:** Enhanced image details and edges using `imsharpen` and a Laplacian filter.

#### 5\. Edge Detection

I implemented five different classical algorithms to detect and highlight edges:

  * Sobel
  * Prewitt
  * Canny
  * Roberts
  * Laplacian of Gaussian (LoG)

#### 6\. Morphological Operations

Working with binary images, I performed several morphological transformations:

  * **Dilation:** Expanded the boundaries of objects.
  * **Erosion:** Shrank the boundaries of objects.
  * **Opening:** Smoothed object contours and removed small protrusions (erosion followed by dilation).
  * **Closing:** Filled small holes and connected nearby objects (dilation followed by erosion).
  * **Hole Filling:** Filled enclosed background regions within objects.

#### 7\. Image Segmentation and Feature Extraction

  * **Otsu's Thresholding:** Performed automatic image thresholding to create a binary image.
  * **Watershed Segmentation:** Implemented the watershed algorithm to separate touching objects in an image.
  * **Object Detection:** Used `regionprops` to identify properties (like area and bounding box) of objects in the binary image and drew rectangles around them to visualize detection.

## 🚀 Getting Started

### Prerequisites

  * MATLAB installed on your machine.
  * MATLAB Image Processing Toolbox.

### Usage

1.  Clone this repository or download the `image_processing.m` file.
2.  Open the `image_processing.m` file in your MATLAB editor.
3.  **Important:** Change the file path in the first line to the location of your own image:
    ```matlab
    img = imread("C:\path\to\your\image.jpg"); % <-- CHANGE THIS LINE
    ```
4.  Run the script by clicking the "Run" button or pressing `F5`.
5.  Observe the multiple figure windows that open, each displaying the result of a different image processing operation.
