# Segmentation_butterflyfish
##  Summary

This is a self-study note about mask-RCNN. Use LabelMe for segmentation and pre-trained model to train mask-RCNN model on butterflyfish dataset. The following were the sources of information.

- Image source: https://www.alamy.com/ (search "butterflyfish")
- Pretrained model source: : https://manishsinghrajput96.blogspot.com/2020/08/how-to-train-mask-rcnn-model-for-custom.html
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
