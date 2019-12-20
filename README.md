# faster-rcnn-keras
faster rcnn based on keras that can train your own dataset

The code is a modification of<br>
https://github.com/RockyXu66/Faster_RCNN_for_Open_Images_Dataset_Keras<br>
The original code is kind of messy and is based on Jupyter Notebook<br>
I organised it into packages with pycharm.<br>
And I added an extra cnn architecture to it - resnet50<br>

# Available feature extraction cnn architectures:<br>
1.resnet50<br>
2.vgg16<br>

# Train on your own dataset
1.generate annotation file, format as follows:<br>
image_path x1,y1,x2,y2,cls_id x1,y1,x2,y2,cls_id<br>
2.download pre-trained weights of vgg or resnet and put it into directory "weights"<br>
vgg - https://github.com/fchollet/deep-learning-models/releases/download/v0.1/vgg16_weights_tf_dim_ordering_tf_kernels.h5<br>
resnet - https://github.com/fchollet/deep-learning-models/releases/download/v0.2/resnet50_weights_tf_dim_ordering_tf_kernels_notop.h5<br>
3.run train.py<br>

# Testing
run test.py

# Results
I trained it on a tobacco detection dataset.
The results are shown in the following.<br>
![alt text](https://github.com/shadow12138/faster-rcnn-keras/blob/master/results/0.png)<br>
![alt text](https://github.com/shadow12138/faster-rcnn-keras/blob/master/results/1.png)

