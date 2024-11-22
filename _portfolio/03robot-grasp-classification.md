---
title: "Robot Grasp Validation Classifier"
excerpt: "Ensuring stable and safe robot manipulator operation using Gazebo simulation data<br/><img src='/images/robot_grasp.png'>"
collection: portfolio
---

[The Shadow Robotics Grasping Dataset](https://www.freecodecamp.org/news/teaching-my-robot-to-think-my-grasp-sucks-5e3d5a908745) provides a set of simulated robotic manipulator grasping trials. Using the [Gazebo robotics simulator](http://gazebosim.org/), over 53,000 experiments were ran, with a total of 992,000 data points. A manipulator with 9 joints (3 fingers, each with 3 joints) was tasked with picking up a sphere from a flat surface and shaking it. The position, velocity, and torque at each joint was recorded various times throughout the trial.

Our goal is to use these features to predict whether the manipulator has a robust grip on the object or if it will drop the object. This has applications in human-robot interaction, where robotic manipulators need to interact in spaces designed for human operation. We implement a logistic regression model, a K-nearest neighbors model, and a random forest for this classification task. We also test various data cleaning methods, such as outlier handling and coercing our data to be IID. 

We achieve 97% accuarcy with our random forest and k-nearest neighbors model when winsorizing to handle outliers, while other models perform marginally worse but still significantly above baseline.

We note that there are strong inter-sample dependencies, as samples in our dataset are a single measurement from a
trajectory of movements. Future work should apply a model capable of better learning long-range dependencies across a
sequence of measurements, such as a BiLSTM or Transformer model.

![a table of accuracy, precision, and recall values](/images/robot_results.png)

You can see the code for this experiment [here](https://github.com/Aidan-B1409/robot_grasping_classifier).

This project was completed as part of the requirements for [AI-539 Machine Learning Challenges in the Real World](https://www.wkiri.com/ai539-w22/) at OSU.
