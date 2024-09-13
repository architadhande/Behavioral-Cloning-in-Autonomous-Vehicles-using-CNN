# Autonomous Vehicle Navigation System using Behavioral Cloning with CNN

## Project Overview

This project focuses on developing an autonomous vehicle navigation system utilizing deep learning techniques. The system includes object detection and classification, obstacle avoidance, and route planning. The project evaluates the performance of various deep learning models and implements a real-time obstacle avoidance algorithm combined with sensor data.

## Objectives

1. **Develop Autonomous Navigation System:** Create a navigation system using deep learning for object detection, obstacle avoidance, and route planning.
2. **Explore Deep Learning Models:** Evaluate the performance of CNNs and RNNs for object detection and classification.
3. **Implement Obstacle Avoidance Algorithm:** Develop a real-time obstacle avoidance algorithm using sensor data and machine learning techniques.
4. **Design Route Planning Algorithm:** Create an algorithm considering traffic, road conditions, and safety for optimal route planning.
5. **Evaluate Performance:** Compare the proposed approach with state-of-the-art methods based on accuracy, speed, and safety through simulation experiments.
6. **Future Research Insights:** Provide recommendations for improving deep learning models and addressing ethical/legal challenges in autonomous driving.

## Dataset Description

Data was collected using a virtual driving simulator. Images were captured from three cameras (front hood, left mirror, right mirror) along with steering angles. The dataset includes:
- Images from three cameras.
- `driving_log.csv` containing steering angles and camera image paths.

## Data Pre-processing

1. **Image Augmentation Techniques:**
   - **Zooming:** Enlarges images for better visibility of key pixels.
   - **Panning:** Moves the image horizontally to focus on the main subject.
   - **Random Flip:** Flips images horizontally or vertically.
   - **Brightness Adjustment:** Enhances image clarity for improved training.

## System Architecture

The system uses a Convolutional Neural Network (CNN) for behavioral cloning, where each frame of video data is used to predict steering angles. Key components include:
- **CNN Model:** Detects and classifies objects.
- **Flattening:** Converts convolution outputs to a one-dimensional vector.
- **Standardization:** Adjusts images for better training.
- **Data Augmentation:** Reduces overfitting by creating modified copies of images.

## Model Training

- **Dataset:** Approximately 18,000 images.
- **Training:** 50 epochs with a batch size of 64.
- **Loss:** Training loss of 0.0099 and validation loss of 0.1126.
- **Model Performance:** Achieved 98% autonomy score with successful operation on both trained and new tracks.

## Results

The model demonstrated high autonomy with minimal deviations and successful obstacle avoidance. It performed well on both familiar and new tracks, achieving an autonomy score of 98% (1 intervention every 300 seconds).

## Conclusion

The project successfully developed an autonomous navigation system using CNN for behavioral cloning. Despite some challenges related to data and environment, the model achieved comparable performance to state-of-the-art systems with significantly less training data. Future work includes integrating object detection and real-time control based on detected objects to enhance navigation in diverse environments.

## Future Work

- **Object Detection Integration:** Develop advanced algorithms for object detection and tracking.
- **Real-time Control:** Implement dynamic control and speed adjustments based on detected objects.
- **Model Improvements:** Explore efficiency and scalability improvements, and address ethical and legal challenges in autonomous driving.

## Acknowledgments

- Special thanks to Nvidia for the DAVE-2 model and dataset references.
- Thanks to the developers of the Udacity simulator for providing the training environment.

