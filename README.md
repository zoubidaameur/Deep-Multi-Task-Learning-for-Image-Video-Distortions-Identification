### Deep-Multi-Task-Learning-for-Image-Video-Distortions-Identification

## Overview

Identifying distortions in images and videos is important and useful in various visual applications, such as image quality enhancement and assessment techniques. Instead of applying them blindly, these techniques can be applied or adjusted depending on the type of distortion identified. In this paper, we propose a deep multi-task learning (MTL) model for identifying the types of distortion in both images and videos, considering both single and multiple distortions. The proposed MTL model is composed of one convolutional neural network (CNN) shared between all tasks and N parallel classifiers, where each classifier is dedicated to identify a type of distortion. The proposed architecture also allows to adjust the number of tasks according to the number of distortion types considered, making the solution scalable. The proposed method has been evaluated on natural scene images and laparoscopic videos databases, each presenting a rich set of distortions. The experimental results demonstrate that our model achieves the best performance among the state-of-art methods for both single and multiple distortions.
![](https://github.com/zoubidaameur/Deep-Multi-Task-Learning-for-Image-Video-Distortions-Identification/blob/main/image-1.png)


## Usage
The source code is available in the notebook.
* For each dataset, upload its corresponding labels to the notebook. (Can be found in folder "data")
* Run the cells in order
1. Import required libraries :  all required packages to run the code are imported.
3. Load dataset : download a specific quality dataset; among the ones used in the paper.
4. Data generator :  extract and pre-process patches from each image to be fed into the model.
5. Build the model : build the multi-task learning model.
6. Train model : call Data generator and Build model to perform training on 80% of dataset.
7. Test model : perform test using training weights on left 20% of dataset.
8. Evaluate test : evaluate the performance of the model on test set.



