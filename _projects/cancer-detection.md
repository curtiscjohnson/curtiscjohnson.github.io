---
title: "Cancer Detector"
layout: single-portfolio
excerpt: "For this project, I trained a CNN based on the UNET architecture on a database of labelled cancerous cell images. The goal was to predict cancer with >85% accuracy.<br/><br/><img src='/images/cancer_detection_ground_truth.png'>"
collection: projects
---

For this project, I trained a CNN based on the UNET architecture on a database of labelled cancerous cell images. The goal was to predict cancer with >85% accuracy. (Greater than 85% because that's about the score you'd get with this dataset by predicting everything was non-cancerous.)

The code for this project is [here.](https://github.com/curtiscjohnson/deep-learning/blob/main/CancerDetector.ipynb)

Here's an example of the dataset and the image that I compare against:

![Ground Truth Cancerous Cells](/images/cancer_detection_ground_truth.png "Ground Truth")

Here are some training results where I can predict with 92.5% accuracy where the cancerous cells are:

![Training Results](/images/cancer_detection_loss_accuracy.png "Loss Accuracy Plot")

and the final resulting prediction which can be compared to the ground truth:

![CNN Prediction](/images/cancer_detection_results.png "CNN Prediction")

Not perfect, but does a decent job!


