# Object_detection_ResNet_for_COCO_imageset

The purpose of this code is to detect objects of interest in the COCO images by assigning boxes to each object. The images containing objects of interest are downloaded from the COCO database "https://cocodataset.org/#download" via the file "COCO_image_downloader.ipynb" and are saved in files for training and testing.

Two different networks are used in the file "Object_detection_training.ipynb" for object detection. The PyTorch DataLoader is used to load the images and the file "instances_train2017.json" that contains the annotation file, which can be downloaded from "https://cocodataset.org/#download". The first network is based on the ResNet structure, where the user can specify whether there should be a skipblock and is used for object classification. The second network is used for regression and predicts the coordinates of the box that encloses the object of interest.

After the training is completed, the file "Object_detection_validation.ipynb" is used for testing. The confusion matrix is plotted for measuring the accuracy of the classification. And the predicted and true coordinates of the bounding boxes are plotted for visual investigation.
