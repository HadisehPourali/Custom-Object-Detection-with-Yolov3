# Custom-Object-Detection-with-Yolov3
Detecting the Defects on a Marble Surface 

In this repository, a Custom Object Detection model has been created with yolov3.

Yolov3 is trained to detect objects with 80 different classes. In this case, I want to detect the defects of a Marble surface with two classes 'dot' and 'crack'. 
For this purpose, the weights of yolov3 should be re-trained.

First of all, for preparing the image for training the model and labeling each category of defects with bounding boxes, we use LabelImg software that exists in 
https://github.com/heartexlabs/labelImg. 
I put the images in a zip file and uploaded them to Google drive.

In the Marble_defects_detection_with_yolov3 code, we mount the Google Drive in Google Colab to upload the training images and save the trained weights of Yolo for custom defects detection in it.

This code trained the Yolo weights for detects the two custom objects. To detect more than 2 classes, some setting should be changed. This code can be used for every 
object detection problem with 2 classes you want. You can label your purpose image and use those images for training.

After training the Yolo weights and save the final weights in yolov3_training_final.weights and testing configuration in yolov3_testing.cfg, use 'Marble defects 
detection with yolov3-testing with openCV' code to evaluate the model with testing images and see the defects detection on the marble surface with bounding boxes.

