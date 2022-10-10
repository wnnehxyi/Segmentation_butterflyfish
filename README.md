# Segmentation_butterflyfish
##  Summary

This is a self-study note about mask-RCNN. Use LabelMe for segmentation and pre-trained model to train mask-RCNN model on butterflyfish dataset. The following were the sources of information.

- Image source: https://www.alamy.com/ (search "butterflyfish")
- Pretrained model source: https://manishsinghrajput96.blogspot.com/2020/08/how-to-train-mask-rcnn-model-for-custom.html
- Lableme source: https://github.com/wkentaro/labelme
- Labelme tutorial: https://www.youtube.com/watch?v=mUoYFzYrVTE

## Environments:
Linux: Ubuntu 20.04.4 LTS

Train the model with colab, and download the code as notebook (.ipynb)

## Steps:
1. Labeled images and generated annotations.json. There are training set (80%) and validation set (20%), and the annotations.json files are merged separately. Data marked as butterflyfish.
![image](https://github.com/wnnehxyi/Segmentation_butterflyfish/blob/main/Steps_pic/1.png)

2. Generated groundtruth after segmentation.
![image](https://github.com/wnnehxyi/Segmentation_butterflyfish/blob/main/Steps_pic/2.png)

3. Setting number of training steps per epoch = 50, epochs = 10
![image](https://github.com/wnnehxyi/Segmentation_butterflyfish/blob/main/Steps_pic/3.png)
![image](https://github.com/wnnehxyi/Segmentation_butterflyfish/blob/main/Steps_pic/3_.png)

4. Compare the predicted and ground truth. Basically the predicted bounding boxes are in the correct position, if we need more masks on the targets, more epochs or images can be added for training.
![image](https://github.com/wnnehxyi/Segmentation_butterflyfish/blob/main/Steps_pic/4.png)
![image](https://github.com/wnnehxyi/Segmentation_butterflyfish/blob/main/Steps_pic/4_1.png)
![image](https://github.com/wnnehxyi/Segmentation_butterflyfish/blob/main/Steps_pic/4_2.png)

5. Use the trained model to predict independent dataset.
- Result 1
![image](https://github.com/wnnehxyi/Segmentation_butterflyfish/blob/main/Steps_pic/5__1.png)
![image](https://github.com/wnnehxyi/Segmentation_butterflyfish/blob/main/Steps_pic/5_1.jpg)

- Result 2
![image](https://github.com/wnnehxyi/Segmentation_butterflyfish/blob/main/Steps_pic/5__2.png)
![image](https://github.com/wnnehxyi/Segmentation_butterflyfish/blob/main/Steps_pic/5_2.jpg)

- Result 3
![image](https://github.com/wnnehxyi/Segmentation_butterflyfish/blob/main/Steps_pic/5__3.png)
![image](https://github.com/wnnehxyi/Segmentation_butterflyfish/blob/main/Steps_pic/5_3.jpg)
