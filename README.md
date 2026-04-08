# Lumbar Disc Herniation Detection using Machine Learning

## Overview

This project develops a machine learning system to assist in detecting **lumbar disc herniation** from MRI images.
The goal is to support physicians by providing automated analysis that can help speed up diagnosis and improve accuracy.

## Problem

Lumbar disc herniation is one of the most common causes of lower back pain and neurological complications.
MRI scans are widely used for diagnosis, but interpreting large numbers of images requires time and clinical expertise.

## Approach

In this project, machine learning algorithms are applied to analyze MRI images and classify intervertebral discs into two categories:

* Normal Disc
* Herniated Disc

The workflow includes:

* Image preprocessing
* Feature extraction
* Dimensionality reduction (PCA)
* Machine learning classification

## Models Used

Several machine learning algorithms were explored and evaluated, including:

* Support Vector Machine (SVM)
* k-Nearest Neighbors (kNN)

## Results

The best performance was achieved using:

kNN + PCA

Accuracy ≈ 84.9%

## Status

Research phase – A research paper is currently being prepared based on this work

## Technologies

* Python
* Scikit-learn
* NumPy
* Pandas
* OpenCV 
