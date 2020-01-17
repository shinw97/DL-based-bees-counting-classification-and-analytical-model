# DL-based-bees-counting-classification-and-analytical-model
Using AI to aid the experts in discovering metadata yielded from bees counting and localization task.

<img src="https://github.com/shinw97/DL-based-bees-counting-classification-and-analytical-model/blob/master/sample-detection.png" width="50%"/> <img src="https://github.com/shinw97/DL-based-bees-counting-classification-and-analytical-model/blob/master/sample-heatmap.png" width="50%"/>


## Some brief intro about the project...
This project was developed in conjunction with my Academic Project I and II (final year project) during my CS study in University of Malaya. The project aimed to achieve three major objectives:

1. Develop an automated computer vision-based counting and classification model.
2. Tabulate and provide visualization of the data for the domain experts to perform deeper research on bees behaviour.
3. Instead of relying on only expert's knowledge, provide a representable output data to perform data driven research on the bees.

The project is fully developed using Python 3 programming language, and YOLO architecture together with tf.keras DL library as the object detection framework. Kudos to [experiencor](https://github.com/experiencor) for making the [sample implementation of YOLO architecture in Keras](https://github.com/experiencor/keras-yolo2) available to the community. My own adaptation and simplified version of the framework is [here at another separated repo](https://github.com/shinw97/simplified-yolo-in-keras).

## Dependencies
The training part of the project is developed in Google Colab platform (with GPU support). Most of the dependencies needed is included in the Google Colab environment, only a few more extra dependencies are needed to install if you plan to use Google Colab as the training environment:

1. [classification_models](https://github.com/qubvel/classification_models)
2. Upgrade the Colab's default TensorFlow version to 2.0

Else if you are more interested to train it on local Jupyter-Notebook environment, just install the dependencies from the **requirements.txt** provided.

## Project Structure
### Datasets
### Training and Testing
### Data Visualization
