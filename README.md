# sta208-covid19-xray
Chest X-Ray classification of COVID-19 patients

## Abstract 

In this data analysis project, we will investigate different machine learning techniques for classifying healthy and infected patients based on X-Ray images. As a baseline, we will apply a classic computer vision pipeline, using Histogram of Oriented Gradients (HOG) for feature extraction and Support Vector Machines (SVM) for classification on the extracted HOG features. We will compare the SVM classifier with deep convolutional neural networks (CNNs) trained under supervised learning.  We will utilize popular pre-trained image classification residual networks, such as ResNet and Inception, as well as networks described in recent COVID-related papers, such as the ResNet Deep anomaly detection model. To make training time tractable, we will use Google Cloud’s educational credits to access GPUs/TPUs.

Initially, we will treat infection detection as a binary classification problem, discriminating between healthy and infected patients, and we will extend both approaches to multiclass classification to distinguish between more specific cases (e.g., healthy patients, viral infections, and bacterial infections). We will compare the performance of the SVM- and CNN-based classifiers using receiver operating characteristic (ROC) curves, precision recall (PR) curves, and confusion matrices. We will use the Chest X-Ray dataset ([Kaggle](https://www.kaggle.com/praveengovi/coronahack-chest-xraydataset), [GitHub](https://github.com/ieee8023/covid-chestxray-dataset)) which consists of images from healthy patients (N=1576) and pneumonia patients induced by both viral (N=1555) and bacterial (N=2777) infections. However, the number of COVID-19 cases within the dataset is relatively small (N=58), and we will need to supplement this dataset with others.

## TO-DO

- Create makefile to download/unzip file on user's local device
    - `eda.ipynb` needs the coronahack dataset to be placed into a `data` directory
- SVM
- CNNs
    - ResNet
    - Deep Anomaly Detection