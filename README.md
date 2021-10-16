# Object_detection_ResNet_for_COCO_imageset

The purpose of this code is to detect objects of interest in the code by assigning boxes to each object. The images containing objects of interest are downloaded from the COCO database via the file "COCO_image_downloader.ipynb". 

Two different networks are used in the file "Object_detection_training.ipynb" for the object detection. The PyTorch DataLoader is used to load the images and the file "instances_train2017.json" that contains the annotation file, which contains the coordinates of the objects of ineterest. The first network is based on the ResNet structure, where the user can specifiy whether there should be a skipblock and is used for object classification. The second network is used for regression. 
