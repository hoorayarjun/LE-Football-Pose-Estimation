# Using Computer Vision to Estimate American Football Player Lower Extremity Key Points
### Anahita Sharma, Elizabeth Lee, Arjun Ganesh, and Stephen Baek, PhD
### University of Virginia, School of Data Science

## Abstract

Lower extremity injuries are the most prevalent injury among American football players, some of which have the capability to end an athlete’s career. This project focuses on identifying toe and ankle key points of American football players as a means of addressing this type of player injury. Specifically, we train a convolutional neural network that estimates joint positions located on the feet of football players using images temporally segmented from multi-view American football game videos. Data was acquired from a Kaggle dataset that was originally created by the NFL to study helmet impacts from video plays. We implement a top-down approach to (1) detect player proposals and generate individual player images from our sample of over 1000 field-view images using YOLOv5 and (2) perform single person pose estimation by implementing a custom DeepPose architecture. As our project is concerned with both accurately estimating the joint coordinates and also classifying whether the joint is a heel or toe, we implement a custom loss function to assess the model’s performance. This loss function uses a weighted sum of the mean squared error (MSE) aimed to assess the accuracy of the predicted x- and y-coordinates for each key point with a binary cross entropy loss used for assessing whether the joints are properly classified as a toe or heel. Our results suggest that a top down approach was capable of predicting the location of key points and classifying whether the point is a toe or heel by minimizing this custom loss function. Pose estimation for tracking lower extremities of American football players can advance research into player injury prevention, a key component in increasing player longevity.



## About


This repository stores all our data and code that was conducted in this project. We hope SSAC judges enjoy our findings!
