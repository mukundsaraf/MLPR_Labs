# Lab 5: Exploring Distance Metrics & Face Detection

## Overview
The main goal of this lab was to get a better understanding of how distance metrics work under the hood and how they apply to real-world Machine Learning tasks. We spent time implementing various distance formulas—like Euclidean and Manhattan—and also experimented with face detection using Haar-cascades and K-Means clustering.

## Methodology

### 1. Face Detection
I used the `cv2` library and the standard `haarcascade_frontalface_default.xml` model to detect faces within the `Plaksha_Faculty.jpg` image. After the model identified the coordinates, I visualized the results by drawing bounding boxes around each detected face.

### 2. Distance Algorithms
I wrote custom functions to calculate three distinct types of distance:
* **Euclidean Distance:** Calculating the standard straight-line path between points.
* **Manhattan Distance:** Calculating the "city block" path (grid-based).
* **Hamming Distance:** Measuring the difference in bits or characters between strings.

### 3. Clustering Implementation
I utilized `KMeans` from the sklearn library to group data points. This helped demonstrate how the choice of distance metric influences how the algorithm groups similar data.

### 4. Model Analysis
I analyzed the impact of cross-validation on model generalization. I also experimented with different "K" values in KNN to observe the trade-off between bias and variance.

## Key Takeaways
This lab really highlighted that the distance metric you choose is critical because it fundamentally changes how the algorithm interprets the data. If you pick a metric that doesn't fit the data structure, your classification or clustering results won't be accurate.

I also learned that while Haar-cascade classifiers are incredibly fast, they can be a bit inconsistent if the lighting is poor or the face is at a difficult angle. Ultimately, the biggest lesson was understanding that balancing bias and variance is the key to building a model that doesn't overfit.
