# Single-view object recognition

Measures object recognition peroformance based on single view object recognition. Object maps are constructed for each object containing several views. Tests are conducted by discretising the object maps, which increases the space (degrees) between views.
![flow diagram](https://raw.githubusercontent.com/ldelange/object-recognition/master/Multi-view%20object%20recognition%20benchmark/svflow.png)

## Descriptors

The [vl_feat](http://www.vlfeat.org/) library for MATLAB is used for feature extraction

* Local binary patterns
* Histogram oriented gradients
* Hue, saturation, value
* Neural Networks (imagenet-vgg-verydeep-16.mat)
* Scale invariant feature transform

## Image datasets

[SOIL-47 dataset](http://www.ee.surrey.ac.uk/CVSSP/demos/colour/soil47/)
```
Objects:	22
Instances:	1
Views: 		20
Height:		Fixed
```

[RGB-D dataset](http://rgbd-dataset.cs.washington.edu/)
```
Objects: 	51
Instances:	4 ~ 8
Views: 		30 ~ 50
Height:		30, 45, 60 degrees
```

## Getting started

Place all .m files inside a directory containing the following externally downloaded libraries and run main.m

* matconvnet
* vlfeat
* soil-47(-masks) or rgbd-dataset

## Results

![Single-view object recognition results](https://raw.githubusercontent.com/ldelange/object-recognition/master/Multi-view%20object%20recognition%20benchmark/results.png)
