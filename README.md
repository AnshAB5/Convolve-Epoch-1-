# ReadMe

This repository contains the code for a hackathon conducted by Cisco in December 2022/January 2023. The hackathon focused on Log Anomaly Detection, specifically detecting anomalies in logs deposited by software using machine learning techniques.

## Introduction

In computing, logging is the act of keeping a log of events that occur in a computer system, such as problems, errors, or information on current operations. Log Anomaly Detection aims to identify anomalies in these logs that deviate from normal patterns. An anomaly can be defined as an occurrence of rare or unexpected events that do not fit into the usual patterns.

## Model

For this project, we utilized a machine learning model based on a sequential architecture. The model incorporates several layers and techniques to effectively learn and detect anomalies in software logs. The key components of the model include:

- Embedding Layer: We used a pre-trained GloVe word vector embedding to capture semantic information in the logs. The embedding layer maps the log text to dense vector representations.
- Lambda Layer: A lambda layer is employed to calculate the mean across the embedding dimensions, reducing the dimensionality of the input.
- Dense Layer: The model includes a dense layer with sigmoid activation to perform binary classification, distinguishing between normal and abnormal logs.
- Regularization: To prevent overfitting and improve generalization, we applied L1 regularization with a coefficient of 0.01 to the dense layer.

## Dataset

The training dataset provided for the hackathon was in JSON format, containing software logs with corresponding labels ("abnormal" or "normal"). The model was trained on this dataset to learn the patterns and characteristics of normal and abnormal logs.

## Usage

To use the model, follow the instructions provided in the code files and refer to the documentation for implementation details. Ensure that the necessary dependencies and libraries are installed in your environment.

## Acknowledgments

We would like to acknowledge the organizers of the Cisco hackathon for providing the opportunity to work on log anomaly detection. The implementation of the model builds upon the collective knowledge and advancements in machine learning and natural language processing techniques.

## Further Improvements

While the hackathon has concluded, there is always room for further improvements and enhancements to the model and in later stages we swapped out the Sequential model with a Transformer based Model

For more information, please refer to the code files and documentation provided during the hackathon.
This copy of the notebook got us a rank of 73 out of 2244 registrated participants, it had a test accuracy of 0.92555 in the hidden test dataset


