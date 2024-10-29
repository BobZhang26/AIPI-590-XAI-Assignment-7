[![Python Application Test with Github Actions](https://github.com/BobZhang26/Bob_PythonTemplate1/actions/workflows/cicd.yml/badge.svg)](https://github.com/BobZhang26/Bob_PythonTemplate1/actions/workflows/cicd.yml)
## AIPI 590 - XAI | Assignment 7
[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/BobZhang26/AIPI-590-XAI-Assignment-7/blob/main/AIPI_590_XAI_Assignment_7.ipynb)
### Instructions
Develop a hypothesis and design a study using explainable deep learning methods to test your hypothesis. You can use any deep learning method discussed during the lecture: concept activation vectors, feature visualization, saliency maps, integrated gradients, or occlusion methods.

Hypothesis must be in the form of a null/alternative hypothesis.



Share your result as a visual report. This report can be in the form of a Google Colab, webpage, blog, or PDF and should contain the H0/H1 hypothesis, a brief explanation of the approach, the visualizations and/or explanations, and a summary of your findings. If Google Colab is not your medium of choice, please include source code as a link in your report.



Note: You will NOT be graded on whether or not your null hypothesis was rejected, only on whether your experiments appropriately tested your hypothesis.

Example hypothesis:

H0: The GoogleNet model does not show a significant difference in its ability to learn the concept "striped" compared to the concept "dotted" for the class ‘zebra’.


H1: The GoogleNet model shows a significant difference in its ability to learn the concept "striped" compared to the concept "dotted" for the class ‘zebra’, specifically, it learns the concept "striped" but not the concept "dotted".

### Goal
In this assignment we will go over the vision classification model ResNet-50, and
apply the pytorch Grad-CAM package on it to explain part of image affect model's
classification.

### Formulating the Hypothesis
H0: ResNet-50 does not utilize features of a cat's body to identify a cat in an image. H1: ResNet-50 utilizes features of a cat's body to identify a cat in an image.

### Experiment Design
Grad-CAM (Gradient-weighted Class Activation Mapping) is a technique used to
visualize the parts of an input image that a convolutional neural network (CNN)
focuses on when making a decision. It essentially highlights regions in an image that
are most influential for the network’s predictions, giving us insight into what
features the model is using to identify certain classes

### Results
- ResNet-50 Classification
When we applied ResNet-50 classification model, the model identified the objects it
detected and segmented them into different color sections where each corresponds
to an object with its probability. In this case, Egyptian cat stands at 96% probability
of the cat's identity in the image. The successful classification shows that the model
is capable of classifying object in a given image.

![image](https://github.com/user-attachments/assets/495370ee-d536-4864-b528-0ab436d71db6)

- Target: Cat and Remote Control
- 
![image](https://github.com/user-attachments/assets/309fac32-6938-437b-b6fb-992a68a8fcab)


