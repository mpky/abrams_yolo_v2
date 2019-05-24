# YOLO v2 Applied to M1 Abrams Tanks

#### Project Goal: Train a set of YOLO weights to detect and draw bounding boxes around given images and videos containing M1 Abrams tanks. This is a continuation of https://github.com/mpky/abrams_project.

#### Data

Largely following markjay4k's walkthrough (https://github.com/markjay4k/YOLO-series) and using thtrieu's darkflow (https://github.com/thtrieu/darkflow), I first manually annotated 1288 images of M1 Abrams tanks using the RectLabel app to produce the annotation XMLs.

#### Training

Trained the model for 5125 steps in Google Colaboratory.

#### Results

The model is able to detect M1 Abrams in all of the test photos although with a rather low degree of confidence.

Video Results:

https://youtu.be/TGagMXkKJ4E

https://youtu.be/S9IXBASPzag

Image Results:

![download (5)](https://user-images.githubusercontent.com/31871105/57265597-6a014300-7046-11e9-81ee-00c5f3886eb2.png)

![download (2)](https://user-images.githubusercontent.com/31871105/57265613-81d8c700-7046-11e9-992c-a02bb62b2e0b.png)
