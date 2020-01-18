# DL-based-bees-counting-classification-and-analytical-model
Using AI to aid the experts in discovering metadata yielded from bees counting and localization task.

<img src="https://github.com/shinw97/DL-based-bees-counting-classification-and-analytical-model/blob/master/sample-count-graph.png" width="45%"/> <img src="https://github.com/shinw97/DL-based-bees-counting-classification-and-analytical-model/blob/master/sample-heatmap.png" width="45%"/>


## Some brief intro about the project...
This project was developed in conjunction with my Academic Project I and II (final year project) during my CS degree in University of Malaya. The collaboration is made with Malaysian Agricultural Research and Development Institute (MARDI), a subdivision under the Ministry of Agriculture and Agro-based Industry Malaysia. 

The project aimed to achieve three major objectives:

1. Develop an automated computer vision-based counting and classification model.
2. Tabulate and provide visualization of the data for the domain experts to perform deeper research on bees behaviour.
3. Instead of relying on only expert's knowledge, provide a representable output data to perform data driven research on the bees.

<p align="center">
<img src="https://github.com/shinw97/DL-based-bees-counting-classification-and-analytical-model/blob/master/sample-detection.png" width="50%"/>
</p>

The project is fully developed using Python 3 programming language, and YOLO architecture together with tf.keras DL library as the object detection framework. Kudos to [experiencor](https://github.com/experiencor) for making the [sample implementation of YOLO architecture in Keras](https://github.com/experiencor/keras-yolo2) available to the community. My own adaptation and simplified version of the framework is [here at another separated repo](https://github.com/shinw97/simplified-yolo-in-keras).

## Dependencies
The training part of the project is developed in Google Colab platform (with GPU support). Most of the dependencies needed is included in the Google Colab environment, only a few more extra dependencies are needed to install if you plan to use Google Colab as the training environment:

1. [image-classifiers-1.0.0](https://pypi.org/project/image-classifiers/)
2. Upgrade the Colab's default TensorFlow version to 2.0

Else if you are more interested to train it on local Jupyter-Notebook environment, just install the dependencies from the [**requirements.txt**](https://github.com/shinw97/DL-based-bees-counting-classification-and-analytical-model/blob/master/requirements.txt) provided.

## Project Structure
### Datasets
The dataset consists of both raw (videos and images) and annotated images. The annotated images are divided into two groups, one consists of only worker bee (1002), and another one consists of both worker bee and drone bee (50). 

All annotations are made using tools from [OpenLabeling](https://github.com/Cartucho/OpenLabeling). The labelled datasets can be accessed here:

`TODO: google drive link`

### Training and Testing


### Data Visualization
Two major data visualization formats are available in this project, which are **simple graph plotting of bees count vs frame** and **frequency heatmap over n-frames**. Sample implementations are available at Demo.ipynb.

## Notes: Possible Improvements

1. Try different object detection drchitectures (M2Det, SSD, Faster R-CNN, etc)
2. Try different CNN feature extractor (VGG16, InceptionNet, RNN, etc)
3. Segment the image (e.g. focus on artificial beehive entry platform) using basic image processing methods (edge detector, binary thresholding, etc) to further clean up the datasets
4. More data labelling!
