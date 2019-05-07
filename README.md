# YOLO v2 Applied to M1 Abrams Tanks

##### Project Goal: Train a set of YOLO weights to detect and draw bounding boxes around given images and videos containing M1 Abrams tanks. This a continuation of https://github.com/mpky/abrams_project.

##### Data

Largely following markjay4k's walkthrough (https://github.com/markjay4k/YOLO-series), I first manually annotated 1288 images of M1 Abrams tanks using the RectLabel app to produce the annotation XMLs.

##### Training

Trained the model for 5125 steps in Google Colab.

##### Results

The model is able to detect M1 Abrams in all of the test photos although without a high degree of confidence.
