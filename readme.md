# HTTP Anomaly Detection Classifier
## Introduction

The classifier uses *HTTP DATASET CSIC 2010* to train the model for detection of malicious HTTP requests. 
For this purpose, the One Class SVM model is used with "_rbf_" kernel and appropriate feature extraction methods in order to obtain sufficient results.

## Feature extraction
I got inspired by [1] and [2] and chose some of the feature extraction methods mentioned in these papers in order to obtain the best results.

## Conclusion 
### Results
Given *HTTP DATASET CSIC 2010*, classifier was evaluated as follows: 
*  *Test Anomalous dataset*: precision **94.45%**
*  *Test Normal dataset*: precision **82.71%**
### Possible improvements
With correctly chosen parameters, classifier showed sufficient results for anomaly detection, however, there is still a lot to improve.  
With growing amount of data, SVM model grows with amount of support vectors, which also causes problems in performance. To reduce the time of computation, multilayer perceptron models (ANN) seems like a good option (since their "trained" weights are of fixed size and do not grow with data).
 
## Literature
1. Althubiti, Sara A.. “Analyzing HTTP requests for web intrusion detection.” (2017).
2. Epp, Nico & Funk, Ralf & Cappo, Cristian. (2017). Anomaly-based Web Application Firewall using HTTP-specific features and One-Class SVM. 