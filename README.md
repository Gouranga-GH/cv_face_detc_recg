
# Face Detection and Recognition Project

## Problem Statement

Company X owns a movie streaming application that provides content to millions of users on a subscription basis. The company wants to automate the process of providing cast and crew information for each scene in a movie. When a user pauses the movie and clicks the cast information button, the application should display details about the actors in the scene.

To achieve this, Company X needs to build two models:

1. **Face Detection**: Detect human faces in images extracted from movie scenes.
2. **Face Recognition**: Recognize and identify actors based on the detected faces.

## Objectives

The project consists of two parts:

### Part 1: Face Detection Model

- **Objective**: Build a model to detect human faces in images.
- **Data Description**: The dataset includes images and corresponding masks where human faces are present.
- **Tasks**:
  1. Import the dataset and prepare it for modeling.
  2. Create features (images) and labels (masks).
  3. Design a face mask detection model using U-Net with pre-trained transfer learning models.
  4. Implement a custom Dice Coefficient and Loss function.
  5. Train, tune, and evaluate the model using test data.
  6. Apply the trained model to a “Prediction Image” and display the output.

### Part 2: Face Recognition Model

- **Objective**: Build a model to identify human faces.
- **Data Description**: The dataset includes aligned face images of 100 individuals.
- **Tasks**:
  1. Load the dataset and generate metadata.
  2. Load a pre-trained face recognition model.
  3. Generate embedding vectors for each face.
  4. Build distance metrics to calculate the similarity between two images.
  5. Use Principal Component Analysis (PCA) for dimensionality reduction.
  6. Build an SVM classifier to map each face to the corresponding person.
  7. Test the model by predicting the identity of faces from the test set.

## Steps to Complete the Project

1. **Data Preparation**:
   - Import the dataset.
   - Clean and preprocess the data.
   - Generate features and labels.

2. **Model Building**:
   - Build the face detection model using U-Net and transfer learning.
   - Build a custom loss function.
   - Train and evaluate the model.
   - Build a face recognition model using a pre-trained model and embedding vectors.
   - Build a classifier for face recognition.

3. **Evaluation and Tuning**:
   - Tune the models to achieve optimal results.
   - Test the models using unseen data.

4. **Model Application**:
   - Apply the trained models to real-world images.
   - Build a user interface or trigger to make the models available for business use.

## Dataset Links

- [WIDER Face Dataset](http://mmlab.ie.cuhk.edu.hk/projects/WIDERFace/)
- [MobileNet Paper](https://arxiv.org/pdf/1704.04861.pdf)
