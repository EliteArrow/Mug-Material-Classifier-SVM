# Mug Material Classifier(SVM)

This project is focused on building a classifier to predict the material of a mug, given four attributes: height, diameter, weight, and hue (color). The classifier is developed based on a "one-against-all" classification scenario, specifically considering whether the material is "Plastic" or not. For evaluation purposes, the dataset is divided into a test set and a training set.

Two types of Support Vector Machines (SVMs) have been employed:

1. Linear SVM: A linear SVM is used as the primary classifier. Due to the non-linear separability of the data, a non-zero regularization weight C is used. The trained classifier's performance is displayed through its accuracy on both the test and training sets. The decision boundary's projection is also plotted in the 3-dimensional height/diameter/weight space.
2. SVM with Gaussian Kernels: To allow a non-linear decision boundary, an SVM with Gaussian Kernels is used. Here, both the regularization weight C and the standard deviation for the Gaussian Kernels serve as parameters. The classification results are presented through data points in the 3-dimensional height/diameter/weight space, which are colored based on their class. The support vectors are identified in both scenarios.

## Prerequisites

The project requires the following packages:

- Python 3.6+
- numpy
- pandas
- matplotlib
- scikit-learn

## Data

The data directory should contain two csv files:

- `data_train.csv`: The training data, including given columns

| Height | Diameter | Weight | Hue | Type |
| --- | --- | --- | --- | --- |
- `data_test.csv`: The test data, including given columns

| Height | Diameter | Weight | Hue | Type |
| --- | --- | --- | --- | --- |
