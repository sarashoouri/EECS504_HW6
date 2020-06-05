# EECS504_HW6
Object Detection
In this problem set, we will implement a single-stage object detector, based on YOLO v1 [1]
and v2 [2]. Unlike the (better-performing) R-CNN models, single-stage stage detectors predict
bounding boxes and classes without explicitly cropping region proposals out of the image or
feature map. This makes them significantly faster to run.
We’ll train and evaluate our detector on the PASCAL VOC dataset, a standard dataset for
object detection tasks. The full dataset contains a total of 11K train/val data images with
27K labeled objects, spanning 20 classes (Figure 1). To make training faster, though, we will
only use a subset that contains 2.5K images
