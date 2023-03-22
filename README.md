# Instance Segmentation with YOLOv8

A basic project to generate an instance segmentation dataset from public datasets such as OpenImagesV6 with [FiftyOne](https://docs.voxel51.com/user_guide/dataset_zoo/index.html). And that this dataset generated in YOLOv8 format is used to train a detection and segmentation model with [Ultralytics](https://github.com/ultralytics/ultralytics).

In [fiftyone/fiftyone.pdf](https://github.com/uleroboticsgroup/is_yolov8/blob/main/fiftyone/fiftyone.pdf) you can find information of how FiftyOne library works to generate datasets. In the example, a dataset with instance segmentation of 'Cats' from [OpenImagesV6](https://storage.googleapis.com/openimages/web/index.html) is downloaded. Then is exported to YOLOv5 format (only detections). And a function is included to generate also instance segmentation labels in YOLOv8 format.
All code is available in [fiftyone/data.ipynb](https://github.com/uleroboticsgroup/is_yolov8/blob/main/fiftyone/data.ipynb)

In [yolov8/yolov8.pdf](https://github.com/uleroboticsgroup/is_yolov8/blob/main/yolov8/yolov8.pdf) you can find information of some of the main functions of Ultralytics library with YOLOv8: inference, train and export model. 
[yolov8/inference.ipynb](https://github.com/uleroboticsgroup/is_yolov8/blob/main/yolov8/inference.ipynb) contains the code to inference a image with YOLOv8 and how to work with the obtained results (bounding bound, mask, category, confidence)
[yolov8/train.ipynb](https://github.com/uleroboticsgroup/is_yolov8/blob/main/yolov8/train.ipynb) contains the code to load a pretrained YOLOv8 model, train it with the custom dataset and export it in other formats.
