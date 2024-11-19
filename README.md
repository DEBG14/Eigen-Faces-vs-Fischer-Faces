# EigenFaces vs FisherFaces

This repository contains code for the project **EigenFaces vs FisherFaces**, which is a part of the Machine Learning course (ELL 784) at IIT Delhi, taught by Prof. Sumantra Dutta Roy. The aim is to develop a facial recognition system that is highly insensitive to variations in lighting direction, intensity, and facial expressions while maintaining a good level of recognition accuracy.

## Methodology

The project focuses on addressing the challenges of facial recognition, including:

1. Variations in lighting and facial expressions.
2. Self-shadowing effects caused by facial geometry, which makes linear subspace modeling difficult.

### Approach:

1. **Linear Subspace Reduction**:  
   Faces are projected into a lower-dimensional subspace, preserving relevant information while discounting regions with large deviations (e.g., shadowed areas).
   
2. **Optimal Class Separation**:  
   Dimensionality reduction ensures the best possible separation between classes for accurate recognition.

### Techniques Compared:

- **Unsupervised Learning**: *EigenFaces Method*  
  This approach focuses on dimensionality reduction using Principal Component Analysis (PCA), emphasizing maximum variance in the data.

- **Supervised Learning**: *FisherFaces Method*  
  This approach uses Linear Discriminant Analysis (LDA) to maximize the separation between classes while reducing dimensionality.

## Dataset Details

The **AT&T Database of Faces** was used for the project.  

- **Dataset Overview**:
  - 10 different images of each of 40 distinct subjects.
  - Variations include:
    - Lighting conditions.
    - Facial expressions (e.g., open/closed eyes, smiling/not smiling).
    - Facial details (e.g., with/without glasses).
    - Small positional shifts (tolerance for side movement).

- **Credit**: AT&T Laboratories Cambridge.

## Objectives

1. **Dimensionality Reduction**: 
   Project high-dimensional face images into a linear subspace while retaining discriminative features.
2. **Comparison of Methods**: 
   Evaluate the performance of EigenFaces (unsupervised) and FisherFaces (supervised) in terms of:
   - Insensitivity to variations in lighting and facial expressions.
   - Recognition accuracy.

## Results

The project demonstrates the strengths and limitations of both approaches:
- **EigenFaces**:
  - Works well in capturing overall variance.
  - Less effective in separating classes with significant overlaps.
- **FisherFaces**:
  - Provides better class separation, leading to higher recognition accuracy.
  - Performs well under challenging lighting and expression variations.


