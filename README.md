# **Machine Learning: Traffic Sign Detection Project**


## **I. Project Description**
Traffic Sign Detection is a problem that applies algorithms related to the field of Object Detection to detect traffic signs on the road. The project involves two main parts: locating the signs and recognizing the traffic signs. This project aims to build a Traffic Sign Detection system using Support Vector Machine (SVM). 

### **Project Goals**
- **Input**: A picture of a traffic sign.
- **Output**: The location and class of the sign in the picture.

## **II. Introduction**
The Traffic Sign Detection program includes two parts: locating the signs and recognizing the traffic signs. A high-accuracy program needs to build these two parts well. In this project, we will build a Traffic Sign Detection using Support Vector Machine (SVM).

## **III. Program Installation**
This section is divided into two main modules: building a classification model using SVM and building an Object Detect model using the sliding window technique.

### **1. Traffic Sign Classification Model Using SVM**
#### **a. Import Necessary Libraries**
We start by importing all necessary libraries for this project, including `cv2`, `numpy`, `pandas`, `matplotlib`, `xml`, `skimage`, and `sklearn`.

#### **b. Data Loading**
We read and store picture files and associated labels into two different lists, corresponding to X and y in our traffic signs classification problem. The data folder includes:
- **images**: Folder with pictures.
- **annotations**: Folder with .xml files containing information about coordinates and classes of traffic signs.

#### **c. Data Preprocessing**
We preprocess the data to prepare it for training the SVM model.

#### **d. Non-Maximum Suppression Algorithm**
To address the issue of multiple overlapping bounding boxes, we implement the Non-Maximum Suppression (NMS) algorithm. The NMS technique eliminates overlapping bounding boxes, keeping only the one with the highest confidence score.

#### **e. Putting Everything Together**
We combine all the elements to create a program to detect traffic signs. This involves declaring the image path, parameters for the function, reading images, creating pyramid images, applying the sliding window function, preprocessing windows, and classifying them.

## **IV. Conclusion**
The model successfully detected and categorized the traffic signs with significant accuracy. However, there were instances where the traffic signs weren't detected, possibly due to their small size in the images or high stride value assigned to the sliding window function. Additionally, a high confidence threshold may have contributed to some missed detections. Despite a few misclassifications, the overall detection rate was satisfactory.

## **V. Usage**
1. Ensure you have all the necessary libraries installed.
2. Load the data into the appropriate folders.
3. Run the notebook cells in sequence to build and test the Traffic Sign Detection model.

## **VI. Dependencies**
- OpenCV
- NumPy
- Pandas
- Matplotlib
- XML
- Skimage
- Sklearn

## **VII. Contact**
For any questions or issues, please contact Uyen Nguyen via [nguyen_u1@denison.edu](mailto:nguyen_u1@denison.edu).
